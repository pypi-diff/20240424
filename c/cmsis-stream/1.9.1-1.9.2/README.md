# Comparing `tmp/cmsis_stream-1.9.1-py3-none-any.whl.zip` & `tmp/cmsis_stream-1.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 92668 bytes, number of entries: 72
+Zip file size: 93606 bytes, number of entries: 72
 -rw-rw-rw-  2.0 fat      298 b- defN 23-May-11 12:29 cmsis_stream/__init__.py
 -rw-rw-rw-  2.0 fat      546 b- defN 23-Jun-02 06:34 cmsis_stream/cmsis_stream.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-11 12:29 cmsis_stream/cg/__init__.py
 -rw-rw-rw-  2.0 fat     9124 b- defN 23-Aug-24 05:45 cmsis_stream/cg/types.py
 -rw-rw-rw-  2.0 fat     1925 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/CFFT.py
 -rw-rw-rw-  2.0 fat     1990 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/Duplicate.py
 -rw-rw-rw-  2.0 fat     1930 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/ICFFT.py
@@ -23,18 +23,18 @@
 -rw-rw-rw-  2.0 fat     2029 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/WavSink.py
 -rw-rw-rw-  2.0 fat     2092 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/WavSource.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/__init__.py
 -rw-rw-rw-  2.0 fat     4018 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/message.py
 -rw-rw-rw-  2.0 fat      118 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/__init__.py
 -rw-rw-rw-  2.0 fat     1691 b- defN 23-Jun-02 05:41 cmsis_stream/cg/scheduler/args.py
 -rw-rw-rw-  2.0 fat     3921 b- defN 23-Aug-16 11:23 cmsis_stream/cg/scheduler/ccode.py
--rw-rw-rw-  2.0 fat     7431 b- defN 23-Aug-16 08:37 cmsis_stream/cg/scheduler/config.py
--rw-rw-rw-  2.0 fat    49788 b- defN 23-Sep-06 12:40 cmsis_stream/cg/scheduler/description.py
+-rw-rw-rw-  2.0 fat     7592 b- defN 24-Apr-11 09:10 cmsis_stream/cg/scheduler/config.py
+-rw-rw-rw-  2.0 fat    52934 b- defN 24-Apr-11 09:38 cmsis_stream/cg/scheduler/description.py
 -rw-rw-rw-  2.0 fat    10924 b- defN 23-Aug-22 13:41 cmsis_stream/cg/scheduler/graphviz.py
--rw-rw-rw-  2.0 fat    38980 b- defN 23-Aug-23 07:53 cmsis_stream/cg/scheduler/node.py
+-rw-rw-rw-  2.0 fat    38980 b- defN 24-Apr-03 11:29 cmsis_stream/cg/scheduler/node.py
 -rw-rw-rw-  2.0 fat     1868 b- defN 23-Jul-18 10:59 cmsis_stream/cg/scheduler/pythoncode.py
 -rw-rw-rw-  2.0 fat     7610 b- defN 23-Aug-23 11:31 cmsis_stream/cg/scheduler/standard.py
 -rw-rw-rw-  2.0 fat      188 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/example/ARMCM55_FP_MVE_config.txt
 -rw-rw-rw-  2.0 fat      192 b- defN 23-Jun-02 06:56 cmsis_stream/cg/scheduler/example/Makefile.linux
 -rw-rw-rw-  2.0 fat      267 b- defN 23-Jun-02 06:56 cmsis_stream/cg/scheduler/example/Makefile.mac
 -rw-rw-rw-  2.0 fat      369 b- defN 23-Jun-02 06:57 cmsis_stream/cg/scheduler/example/Makefile.windows
 -rw-rw-rw-  2.0 fat      566 b- defN 23-Jun-06 06:05 cmsis_stream/cg/scheduler/example/README.md
@@ -43,32 +43,32 @@
 -rw-rw-rw-  2.0 fat      598 b- defN 23-Jul-20 11:15 cmsis_stream/cg/scheduler/example/simple.cproject.yml
 -rw-rw-rw-  2.0 fat     1416 b- defN 23-Jun-02 07:20 cmsis_stream/cg/scheduler/example/simple_ac6.csolution.yml
 -rw-rw-rw-  2.0 fat     2178 b- defN 23-Jun-02 06:48 cmsis_stream/cg/scheduler/example/start_project_appnodes.h
 -rw-rw-rw-  2.0 fat       73 b- defN 23-Jun-02 06:10 cmsis_stream/cg/scheduler/example/start_project_custom.h
 -rw-rw-rw-  2.0 fat     1798 b- defN 23-Jun-02 06:26 cmsis_stream/cg/scheduler/example/start_project_graph.py
 -rw-rw-rw-  2.0 fat      197 b- defN 23-Jun-02 06:05 cmsis_stream/cg/scheduler/example/start_project_main.c
 -rw-rw-rw-  2.0 fat      878 b- defN 23-Jul-20 11:15 cmsis_stream/cg/scheduler/example/vht.clayer.yml
--rw-rw-rw-  2.0 fat    22424 b- defN 23-Sep-06 12:55 cmsis_stream/cg/scheduler/templates/GenericNodes.h
--rw-rw-rw-  2.0 fat     2006 b- defN 23-Sep-06 12:55 cmsis_stream/cg/scheduler/templates/cg_status.h
+-rw-rw-rw-  2.0 fat    22424 b- defN 24-Apr-11 10:05 cmsis_stream/cg/scheduler/templates/GenericNodes.h
+-rw-rw-rw-  2.0 fat     2006 b- defN 24-Apr-11 10:05 cmsis_stream/cg/scheduler/templates/cg_status.h
 -rw-rw-rw-  2.0 fat      434 b- defN 23-Jun-12 07:09 cmsis_stream/cg/scheduler/templates/cmsis.cpp
 -rw-rw-rw-  2.0 fat      287 b- defN 23-Jun-12 06:56 cmsis_stream/cg/scheduler/templates/cmsis.py
 -rw-rw-rw-  2.0 fat      682 b- defN 23-Jun-12 06:56 cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp
 -rw-rw-rw-  2.0 fat     1274 b- defN 23-Aug-16 10:29 cmsis_stream/cg/scheduler/templates/code.cpp
--rw-rw-rw-  2.0 fat     1587 b- defN 23-Jul-25 13:03 cmsis_stream/cg/scheduler/templates/code.h
+-rw-rw-rw-  2.0 fat     1777 b- defN 24-Apr-11 09:23 cmsis_stream/cg/scheduler/templates/code.h
 -rw-rw-rw-  2.0 fat     2202 b- defN 23-Jul-19 09:25 cmsis_stream/cg/scheduler/templates/code.py
 -rw-rw-rw-  2.0 fat     3414 b- defN 23-Aug-16 11:22 cmsis_stream/cg/scheduler/templates/codeSwitch.cpp
--rw-rw-rw-  2.0 fat     5758 b- defN 23-Aug-22 05:33 cmsis_stream/cg/scheduler/templates/commonc.cpp
--rw-rw-rw-  2.0 fat     1395 b- defN 23-Aug-17 07:53 cmsis_stream/cg/scheduler/templates/defineConfig.h
+-rw-rw-rw-  2.0 fat     6539 b- defN 24-Apr-11 09:41 cmsis_stream/cg/scheduler/templates/commonc.cpp
+-rw-rw-rw-  2.0 fat     1576 b- defN 24-Apr-11 09:22 cmsis_stream/cg/scheduler/templates/defineConfig.h
 -rw-rw-rw-  2.0 fat     7858 b- defN 23-Aug-23 07:53 cmsis_stream/cg/scheduler/templates/dot_template.dot
 -rw-rw-rw-  2.0 fat     7555 b- defN 23-Jun-09 12:52 cmsis_stream/cg/scheduler/templates/precompute_dot_template.dot
 -rw-rw-rw-  2.0 fat       26 b- defN 23-Jul-17 05:58 cmsis_stream/cg/sds/__init__.py
 -rw-rw-rw-  2.0 fat     3923 b- defN 23-Jul-18 08:03 cmsis_stream/cg/sds/sds_nodes.py
 -rw-rw-rw-  2.0 fat      104 b- defN 23-Jul-18 08:25 cmsis_stream/cg/yaml/__init__.py
 -rw-rw-rw-  2.0 fat    15372 b- defN 23-Aug-24 05:39 cmsis_stream/cg/yaml/exportyaml.py
 -rw-rw-rw-  2.0 fat    17272 b- defN 23-Aug-24 05:40 cmsis_stream/cg/yaml/importyaml.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Sep-06 12:55 cmsis_stream-1.9.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     5676 b- defN 23-Sep-06 12:55 cmsis_stream-1.9.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Sep-06 12:55 cmsis_stream-1.9.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       59 b- defN 23-Sep-06 12:55 cmsis_stream-1.9.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       13 b- defN 23-Sep-06 12:55 cmsis_stream-1.9.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     6920 b- defN 23-Sep-06 12:55 cmsis_stream-1.9.1.dist-info/RECORD
-72 files, 302120 bytes uncompressed, 81380 bytes compressed:  73.1%
+-rw-rw-rw-  2.0 fat    11558 b- defN 24-Apr-11 10:05 cmsis_stream-1.9.2.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     5881 b- defN 24-Apr-11 10:05 cmsis_stream-1.9.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-11 10:05 cmsis_stream-1.9.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       59 b- defN 24-Apr-11 10:05 cmsis_stream-1.9.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-11 10:05 cmsis_stream-1.9.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     6920 b- defN 24-Apr-11 10:05 cmsis_stream-1.9.2.dist-info/RECORD
+72 files, 306784 bytes uncompressed, 82318 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -192,26 +192,26 @@
 
 Filename: cmsis_stream/cg/yaml/exportyaml.py
 Comment: 
 
 Filename: cmsis_stream/cg/yaml/importyaml.py
 Comment: 
 
-Filename: cmsis_stream-1.9.1.dist-info/LICENSE.txt
+Filename: cmsis_stream-1.9.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: cmsis_stream-1.9.1.dist-info/METADATA
+Filename: cmsis_stream-1.9.2.dist-info/METADATA
 Comment: 
 
-Filename: cmsis_stream-1.9.1.dist-info/WHEEL
+Filename: cmsis_stream-1.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: cmsis_stream-1.9.1.dist-info/entry_points.txt
+Filename: cmsis_stream-1.9.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: cmsis_stream-1.9.1.dist-info/top_level.txt
+Filename: cmsis_stream-1.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cmsis_stream-1.9.1.dist-info/RECORD
+Filename: cmsis_stream-1.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cmsis_stream/cg/scheduler/config.py

```diff
@@ -150,16 +150,20 @@
         # synchronous scheduling.
         self.FIFOIncrease = 0
 
         # Default asynchronous more for pure functions 
         # like CMSIS-DSP
         self.asyncDefaultSkip = True
 
+        # Objects are allocated on the heap rather than stack
         self.heapAllocation = False
 
+        # Buffer are allocated through memory allocator
+        self.bufferAllocation = False
+
         # When true, create a new C++ header only
         # with an array allowing to access the identified
         # nodes (identified is a node creation option true by default)
         # Macros are also generated to give indexes into this array
         # It implies heapAllocation true because nodes
         # must be available before the scheduler is started.
         self.nodeIdentification = False
```

## cmsis_stream/cg/scheduler/description.py

```diff
@@ -78,41 +78,45 @@
 class DupDestination:
     def __init__(self,
                  node,
                  delay,
                  fifoClass,
                  fifoScale,
                  fifoAsyncLength,
-                 fifoWeak):
+                 fifoWeak,
+                 fifoCustomBuffer):
         self.node = node
         self.delay = delay 
         self.fifoClass = fifoClass 
         self.fifoScale = fifoScale 
         self.fifoAsyncLength = fifoAsyncLength 
         self.fifoWeak = fifoWeak 
+        self.fifoCustomBuffer = fifoCustomBuffer
 
 
 class FifoBuffer:
     """Buffer used by a FIFO"""
     def __init__(self,bufferID,theType,length):
         self._length=length 
         self._theType=theType 
         self._bufferID=bufferID
 
 class FIFODesc:
     """A FIFO connecting two nodes"""
-    def __init__(self,fifoid,fifoClass,fifoScale,fifoAsyncLength=0,weak=False):
+    def __init__(self,fifoid,fifoClass,fifoScale,fifoAsyncLength=0,weak=False,customBuffer=None):
         # The FIFO is in fact just an array
         self.isArray=False 
         # FIFO length
         self.length=0
         # FIFO type
         self.theType=None 
-        # Buffer used by FIFO
+        # Buffer used by FIFO (allocated by the scheduler)
         self.buffer=None 
+        # Custom buffer assigned to FIFO 
+        self.customBuffer = customBuffer
         # Used for plot in graphviz
         self.bufferID=-1
         self._fifoID=fifoid 
         # Source IO
         self.src = None 
         # Dest IO
         self.dst = None 
@@ -171,14 +175,22 @@
             self._liveInterval=(theTime,stop)
 
     def recordRead(self,theTime):
         start,stop=self._liveInterval 
         if (theTime > stop):
             self._liveInterval=(start,theTime)
 
+    def bufName(self,config):
+        if not self.customBuffer is None:
+            return(self.customBuffer)
+        if config.bufferAllocation:
+           return(f"buffers.buf{self.buffer._bufferID}")
+        else:
+           return(f"{config.prefix}buf{self.buffer._bufferID}")
+
 
 def analyzeStep(vec,allFIFOs,theTime):
     """Analyze an evolution step to know which FIFOs are read and written to"""
     fifoID = 0 
     for fifo in (vec > 0):
         if fifo:
             allFIFOs[fifoID].recordWrite(theTime) 
@@ -206,14 +218,18 @@
         # In async mode, scaling factor for a given
         # FIFO to override the global scaling factor
         self._FIFOScale = {}
         # In fully asynchronous the fifo length
         # and weak state
         self._FIFOAsyncLength = {}
         self._FIFOWeak = {}
+        # If FIFO must be mapped on a custom buffer
+        # It prevents memory optimization from bein applied to
+        # this FIFO
+        self._FIFOCustomBuffer = {}
         # Topological sorting of nodes
         # computed during topology matrix
         # and used for some scheduling
         # (prioritizing the scheduling of nodes
         # close to the graph output)
         self._topologicalSort=[]
         self.defaultFIFOClass = "FIFO"
@@ -301,22 +317,24 @@
         if (destination[theId].delay!=0):
             self.connectWithDelay(outputIO,destination[theId].node,
                                            destination[theId].delay,
                                            dupAllowed=False,
                                            fifoClass=destination[theId].fifoClass,
                                            fifoScale=destination[theId].fifoScale,
                                            fifoAsyncLength=destination[theId].fifoAsyncLength,
-                                           weak=destination[theId].fifoWeak)
+                                           weak=destination[theId].fifoWeak,
+                                           buffer=destination[theId].fifoCustomBuffer)
         else:
             self.connect(outputIO,destination[theId].node,
                                   dupAllowed=False,
                                   fifoClass=destination[theId].fifoClass,
                                   fifoScale=destination[theId].fifoScale,
                                   fifoAsyncLength=destination[theId].fifoAsyncLength,
-                                  weak=destination[theId].fifoWeak
+                                  weak=destination[theId].fifoWeak,
+                                  buffer=destination[theId].fifoCustomBuffer
                                   )
 
 
 
     def insertDuplicates(self,config):
         # Insert dup nodes (Duplicate2 and Duplicate3) to
         # ensure that an output is connected to only one input
@@ -377,37 +395,42 @@
                         nodea = f[0]
                         nodeb = f[1]
 
                         fifoClass = self.defaultFIFOClass
                         fifoScale = 1.0
                         fifoAsyncLength = 0
                         fifoWeak = False
+                        fifoCustomBuffer = None
                         if (nodea,nodeb) in self._FIFOClasses:
                             fifoClass = self._FIFOClasses[(nodea,nodeb)]
 
                         if (nodea,nodeb) in self._FIFOScale:
                             fifoScale = self._FIFOScale[(nodea,nodeb)]
 
                         if (nodea,nodeb) in self._FIFOAsyncLength:
                             fifoAsyncLength = self._FIFOAsyncLength[(nodea,nodeb)]
 
                         if (nodea,nodeb) in self._FIFOWeak:
                             fifoWeak = self._FIFOWeak[(nodea,nodeb)]
 
+                        if (nodea,nodeb) in self._FIFOCustomBuffer:
+                            fifoCustomBuffer = self._FIFOCustomBuffer[(nodea,nodeb)]
+
                         if (nodea,nodeb) in self._delays:
                            delay = self._delays[(nodea,nodeb)]
                         else:
                            delay = 0
 
                         destination=DupDestination(nodeb,
                             delay,
                             fifoClass,
                             fifoScale,
                             fifoAsyncLength,
-                            fifoWeak)
+                            fifoWeak,
+                            fifoCustomBuffer)
 
                         destinations.append(destination)
 
                         nodea.fifo=None 
                         nodeb.fifo=None
                         # Since we are not using a multi graph
                         # and there no parallel edges, it will
@@ -427,14 +450,16 @@
                         if (nodea,nodeb) in self._FIFOScale:
                             del self._FIFOScale[(nodea,nodeb)]
 
                         if (nodea,nodeb) in self._FIFOAsyncLength:
                             del self._FIFOAsyncLength[(nodea,nodeb)]
                         if (nodea,nodeb) in self._FIFOWeak:
                             del self._FIFOWeak[(nodea,nodeb)]
+                        if (nodea,nodeb) in self._FIFOCustomBuffer:
+                            del self._FIFOCustomBuffer[(nodea,nodeb)]
 
                         if (nodea,nodeb) in self._delays:
                            del self._delays[(nodea,nodeb)]
 
                         
                     
                     # Now for each fifo destination b_i we need 
@@ -463,15 +488,16 @@
                
 
     def connect(self,nodea,nodeb,
         dupAllowed=True,
         fifoClass=None,
         fifoScale = 1.0,
         fifoAsyncLength=0,
-        weak=False):
+        weak=False,
+        buffer=None):
         if fifoClass is None:
             fifoClass = self.defaultFIFOClass
         # When connecting to a constant node we do nothing
         # since there is no FIFO in this case
         # and it does not participate to the scheduling.
         if (isinstance(nodea,Constant)):
             nodeb.constantNode = nodea
@@ -491,14 +517,16 @@
                    nodeb.fifo=(nodea,nodeb)
                 self._edges[(nodea,nodeb)]=True
 
                 self._FIFOClasses[(nodea,nodeb)] = fifoClass
                 self._FIFOScale[(nodea,nodeb)] = fifoScale
                 self._FIFOAsyncLength[(nodea,nodeb)] = fifoAsyncLength
                 self._FIFOWeak[(nodea,nodeb)] = weak
+                if not buffer is None:
+                    self._FIFOCustomBuffer[(nodea,nodeb)] = buffer
 
 
                 if not (nodea.owner in self._nodes):
                    self._nodes[nodea.owner]=True
                 if not (nodeb.owner in self._nodes):
                    self._nodes[nodeb.owner]=True
  
@@ -509,27 +537,29 @@
                                      nodea.theType,nodeb.theType)
 
     def connectWithDelay(self,nodea,nodeb,delay,
         dupAllowed=True,
         fifoClass=None,
         fifoScale=1.0,
         fifoAsyncLength=0,
-        weak=False):
+        weak=False,
+        buffer=None):
         if fifoClass is None:
             fifoClass = self.defaultFIFOClass
         # We cannot connect with delay to a constant node
         if (isinstance(nodea,Constant)):
             raise CannotDelayConstantError
         else:
             self.connect(nodea,nodeb,
                 dupAllowed=dupAllowed,
                 fifoClass=fifoClass,
                 fifoScale = fifoScale,
                 fifoAsyncLength=fifoAsyncLength,
-                weak=weak)
+                weak=weak,
+                buffer=buffer)
             self._delays[(nodea,nodeb)] = delay
     
     def __str__(self):
         res=""
         for (a,b) in self._edges: 
             nodea = a.owner
             nodeb = b.owner 
@@ -567,39 +597,47 @@
             src,dst = edge
             if edge in self._FIFOClasses:
                fifoClass = self._FIFOClasses[edge]
                fifo.fifoClass = fifoClass
             fifo.src=src
             fifo.dst=dst 
 
+            if edge in self._FIFOCustomBuffer:
+                fifo.customBuffer = self._FIFOCustomBuffer[edge]
+
             # To ensure dst node use same FIFO type as source
             # node. There is no implicit typecast of pointer
             # But the C++ template can typecast on elements
             # so the shared status is imposed by the source
             # and the destination node will adapt through C++
             # when it make senses (like a const input can also 
             # receive a non const pointer)
             dst.theType._shared = src.theType._shared
 
             fifo.delay=self.getDelay(edge)
             # When a FIFO is working as an array then its buffer may
-            # potentially be shared with other FIFOs workign as arrays
-            if src.nbSamples == dst.nbSamples:
+            # potentially be shared with other FIFOs working as arrays
+            # If fifo length is bigger it means we may have
+            # double write, double read and so the FIFO is not used
+            # as an array.
+            # The scheduling try to interleave read / write so this
+            # case may nto occur too often.
+            if src.nbSamples == dst.nbSamples and src.nbSamples == fifo.length:
                 if fifo.delay==0:
                    if not config.asynchronous and not config.fullyAsynchronous:
                       fifo.isArray = True 
             # Type of FIFO is coming from the SRC.
             # It is an important property for the
             # change of type in duplicate insertion
             fifo.theType = src.theType
             #fifo.dump()
 
 
         bufferID=0
-        allBuffers=[]
+        allBuffers={}
 
         # Compute a graph describing when FIFOs are used at the same time
         # Then use graph coloring to allocate buffer to those FIFOs.
         # Then size the buffer based on the longest FIFO using it
         # Memory optimizations are disabled by the asynchronous mode
         # because the execution is no more periodic.
         # So anything deduced from a synchronous period
@@ -607,14 +645,24 @@
         if config.memoryOptimization and not config.asynchronous and not config.fullyAsynchronous:
             G = nx.Graph()
 
             for fifo in allFIFOs: 
                     if fifo.isArray:
                         G.add_node(fifo)
 
+            # FIFO with an assigned external buffer
+            # are interfering 
+            for fifo in allFIFOs: 
+                if not fifo.customBuffer is None:
+                    if fifo.isArray:
+                        for other in allFIFOs:
+                            if other != fifo and other.isArray:
+                                if not G.has_edge(fifo,other) and not G.has_edge(other,fifo):
+                                   G.add_edge(fifo,other)
+
             # Create the interference graph
 
             # Dictionary of active FIFOs at a given time.
             # The time is a scheduling step
             active={}
             currentTime=0
             while currentTime<=maxTime:
@@ -644,15 +692,16 @@
                         # cannot be used again until it has been read.
                         # So, src and dst are both live at this time.
                         # Which means the condition on the stop time must be 
                         # stop >= currentTime and not a strict comparison
                         if start<=currentTime and stop >= currentTime:
                             if not (fifo in active):
                                 for k in active:
-                                    G.add_edge(k,fifo)
+                                    if not G.has_edge(k,fifo) and not G.has_edge(fifo,k):
+                                       G.add_edge(k,fifo)
                                 active[fifo]=True 
     
                 currentTime = currentTime + 1
 
             # To debug and display the graph
             if False:
                import matplotlib.pyplot as plt
@@ -672,60 +721,73 @@
             # Graph coloring
             d = nx.coloring.greedy_color(G, strategy="largest_first")
 
             # Allocate the colors (buffer ID) to the FIFO
             # and keep track of the max color number
             # Since other buffers (for real FIFOs) will have their
             # numbering start after this one.
+            
+            # Remap to continuous buffer number starting from 0
+            # since the Jinja templates assume that buffers are
+            # continuous
+            continuousNumber = 0
+            sharedToContinuous={}
             for fifo in d:
-                fifo.sharedNB=d[fifo]
-                bufferID=max(bufferID,fifo.sharedNB)
+                if fifo.customBuffer is None:
+                   if not d[fifo] in sharedToContinuous:
+                       sharedToContinuous[d[fifo]] = continuousNumber
+                       continuousNumber = continuousNumber + 1
+                   fifo.sharedNB=sharedToContinuous[d[fifo]]
+                   bufferID=max(bufferID,fifo.sharedNB)
 
 
 
             # Compute the max size for each shared buffer
             maxSizes={} 
             for fifo in d:
-                lengthInBytes = fifo.theType.bytes * fifo.length
-                if fifo.sharedNB in maxSizes:
-                    maxSizes[fifo.sharedNB] = max(maxSizes[fifo.sharedNB],lengthInBytes) 
-                else:
-                    maxSizes[fifo.sharedNB]=lengthInBytes
+                # No custom buffer assigned so can use a shared buffer
+                if fifo.customBuffer is None:
+                   lengthInBytes = fifo.theType.bytes * fifo.length
+                   if fifo.sharedNB in maxSizes:
+                       maxSizes[fifo.sharedNB] = max(maxSizes[fifo.sharedNB],lengthInBytes) 
+                   else:
+                       maxSizes[fifo.sharedNB]=lengthInBytes
 
             # Create the buffers
             for theID in maxSizes:
               sharedA = FifoBuffer(theID,CType(UINT8),maxSizes[theID])
-              allBuffers.append(sharedA)
-
+              allBuffers[theID]=sharedA
 
         # bufferID must start after all shared buffers
         bufferID = bufferID + 1
         for fifo in allFIFOs:
             # Use shared buffer if memory optimization
             if fifo.isArray and (config.memoryOptimization and not config.asynchronous and not config.fullyAsynchronous):
-                fifo.buffer=allBuffers[fifo.sharedNB] 
-                fifo.bufferID=fifo.sharedNB
+                if fifo.customBuffer is None:
+                   fifo.buffer=allBuffers[fifo.sharedNB] 
+                   fifo.bufferID=fifo.sharedNB
             # Create a new buffer for a real FIFO
             # Use bufferID which is starting after the numbers allocated
             # to shared buffers
             else:
                 buf = FifoBuffer(bufferID,fifo.theType,fifo.length)
-                allBuffers.append(buf)
+                allBuffers[bufferID]=buf
                 fifo.buffer=buf
                 fifo.bufferID = bufferID
                 bufferID = bufferID + 1
 
+        allBuffers = allBuffers.values()
+
         # Compute the total memory used in bytes
         self._totalMemory = 0
         for buf in allBuffers:
             self._totalMemory = self._totalMemory + buf._theType.bytes * buf._length
 
         #for fifo in allFIFOs:
         #    fifo.dump()
-        
         return(allBuffers)
 
 
 
 
     @property
     def constantEdges(self):
```

## cmsis_stream/cg/scheduler/templates/code.h

```diff
@@ -41,14 +41,19 @@
 {% if config.CAPI -%}
 extern void *get_{{config.schedName}}_node(int32_t nodeID);
 {% else %}
 extern NodeBase *get_{{config.schedName}}_node(int32_t nodeID);
 {% endif %}
 {% endif %}
 
+{% if config.bufferAllocation %}
+extern int init_buffer_{{config.schedName}}({{optionalargs(True)}});
+extern void free_buffer_{{config.schedName}}({{optionalargs(True)}});
+{% endif %}
+
 {% if config.heapAllocation %}
 extern int init_{{config.schedName}}({{optionalargs(True)}});
 extern void free_{{config.schedName}}({{optionalargs(True)}});
 {% endif %}
 extern uint32_t {{config.schedName}}(int *error{{optionalargs(False)}});
 
 {% if config.CAPI -%}
```

## cmsis_stream/cg/scheduler/templates/commonc.cpp

```diff
@@ -62,20 +62,54 @@
 FIFO buffers
 
 ************/
 {% for fifo in fifos %}
 #define FIFOSIZE{{fifo.fifoID}} {{fifo.length}}
 {% endfor %}
 
+{% if config.bufferAllocation %}
+typedef struct {
+{% for buf in sched._graph._allBuffers %}
+{{buf._theType.ctype}}  *buf{{buf._bufferID}};
+{% endfor %}
+} buffers_t;
+
+CG_BEFORE_BUFFER
+static buffers_t buffers={0};
+
+int init_buffer_{{config.schedName}}({{optionalargs(True)}})
+{
+{% for buf in sched._graph._allBuffers %}
+    buffers.buf{{buf._bufferID}} = ({{buf._theType.ctype}} *)CG_MALLOC({{buf._length}} * sizeof({{buf._theType.ctype}}));
+    if (buffers.buf{{buf._bufferID}}==NULL)
+    {
+        return(CG_MEMORY_ALLOCATION_FAILURE);
+    }
+{% endfor %}
+    return(CG_SUCCESS);
+}
+
+void free_buffer_{{config.schedName}}({{optionalargs(True)}})
+{
+{% for buf in sched._graph._allBuffers %}
+    if (buffers.buf{{buf._bufferID}}!=NULL)
+    {
+        CG_FREE(buffers.buf{{buf._bufferID}});
+    }
+{% endfor %}
+}
+
+{% else %}
 {% for buf in sched._graph._allBuffers %}
 #define BUFFERSIZE{{buf._bufferID}} {{buf._length}}
 CG_BEFORE_BUFFER
 {{buf._theType.ctype}} {{config.prefix}}buf{{buf._bufferID}}[BUFFERSIZE{{buf._bufferID}}]={0};
 
 {% endfor %}
+{% endif %}
 
 {% if config.heapAllocation %}
 typedef struct {
 {% for id in range(nbFifos) %}
 {{fifos[id].fifoClass}}<{{fifos[id].theType.ctype}},FIFOSIZE{{id}},{{fifos[id].isArrayAsInt}},{{async()}}> *fifo{{id}};
 {% endfor %}
 } fifos_t;
@@ -114,21 +148,21 @@
 {% endif %}
 
 int init_{{config.schedName}}({{optionalargs(True)}})
 {
     CG_BEFORE_FIFO_INIT;
 {% for id in range(nbFifos) %}
 {% if fifos[id].hasDelay %}
-    fifos.fifo{{id}} = new {{fifos[id].fifoClass}}<{{fifos[id].theType.ctype}},FIFOSIZE{{id}},{{fifos[id].isArrayAsInt}},{{async()}}>({{config.prefix}}buf{{fifos[id].buffer._bufferID}},{{fifos[id].delay}});
+    fifos.fifo{{id}} = new {{fifos[id].fifoClass}}<{{fifos[id].theType.ctype}},FIFOSIZE{{id}},{{fifos[id].isArrayAsInt}},{{async()}}>({{fifos[id].bufName(config)}},{{fifos[id].delay}});
     if (fifos.fifo{{id}}==NULL)
     {
         return(CG_MEMORY_ALLOCATION_FAILURE);
     }
 {% else %}
-    fifos.fifo{{id}} = new {{fifos[id].fifoClass}}<{{fifos[id].theType.ctype}},FIFOSIZE{{id}},{{fifos[id].isArrayAsInt}},{{async()}}>({{config.prefix}}buf{{fifos[id].buffer._bufferID}});
+    fifos.fifo{{id}} = new {{fifos[id].fifoClass}}<{{fifos[id].theType.ctype}},FIFOSIZE{{id}},{{fifos[id].isArrayAsInt}},{{async()}}>({{fifos[id].bufName(config)}});
     if (fifos.fifo{{id}}==NULL)
     {
         return(CG_MEMORY_ALLOCATION_FAILURE);
     }
 {% endif %}
 {% endfor %}
 
@@ -190,17 +224,17 @@
 {% if not config.heapAllocation %}
     CG_BEFORE_FIFO_INIT;
     /*
     Create FIFOs objects
     */
 {% for id in range(nbFifos) %}
 {% if fifos[id].hasDelay %}
-    {{fifos[id].fifoClass}}<{{fifos[id].theType.ctype}},FIFOSIZE{{id}},{{fifos[id].isArrayAsInt}},{{async()}}> fifo{{id}}({{config.prefix}}buf{{fifos[id].buffer._bufferID}},{{fifos[id].delay}});
+    {{fifos[id].fifoClass}}<{{fifos[id].theType.ctype}},FIFOSIZE{{id}},{{fifos[id].isArrayAsInt}},{{async()}}> fifo{{id}}({{fifos[id].bufName(config)}},{{fifos[id].delay}});
 {% else %}
-    {{fifos[id].fifoClass}}<{{fifos[id].theType.ctype}},FIFOSIZE{{id}},{{fifos[id].isArrayAsInt}},{{async()}}> fifo{{id}}({{config.prefix}}buf{{fifos[id].buffer._bufferID}});
+    {{fifos[id].fifoClass}}<{{fifos[id].theType.ctype}},FIFOSIZE{{id}},{{fifos[id].isArrayAsInt}},{{async()}}> fifo{{id}}({{fifos[id].bufName(config)}});
 {% endif %}
 {% endfor %}
 
     CG_BEFORE_NODE_INIT;
     /* 
     Create node objects
     */
```

## cmsis_stream/cg/scheduler/templates/defineConfig.h

```diff
@@ -2,14 +2,24 @@
 #define CHECKERROR       if (cgStaticError < 0) \
        {\
          goto errorHandling;\
        }
 
 #endif
 
+{% if config.bufferAllocation %}
+#if !defined(CG_MALLOC)
+#define CG_MALLOC(A) malloc((A))
+#endif 
+
+#if !defined(CG_FREE)
+#define CG_FREE(A) free((A))
+#endif 
+{% endif %}
+
 #if !defined(CG_BEFORE_ITERATION)
 #define CG_BEFORE_ITERATION
 #endif 
 
 #if !defined(CG_AFTER_ITERATION)
 #define CG_AFTER_ITERATION
 #endif
```

## Comparing `cmsis_stream-1.9.1.dist-info/LICENSE.txt` & `cmsis_stream-1.9.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `cmsis_stream-1.9.1.dist-info/METADATA` & `cmsis_stream-1.9.2.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmsis-stream
-Version: 1.9.1
+Version: 1.9.2
 Summary: CMSIS-Stream graph description
 Home-page: https://github.com/ARM-software/CMSIS-Stream
 Author: Copyright (C) 2010-2023 ARM Limited or its affiliates. All rights reserved.
 Author-email: christophe.favergeon@arm.com
 License: License :: OSI Approved :: Apache Software License
 Project-URL: Bug Reports, https://github.com/ARM-software/CMSIS-Stream/issues
 Project-URL: Source, https://github.com/ARM-software/CMSIS-Stream
@@ -42,14 +42,19 @@
 
 * Define new compute nodes
 * Connect them into a dataflow graph to process streams
 * Generate at build time a static C scheduler to run the graph on your target (no need of an RTOS)
 
 # Change history
 
+## Version 1.9.2:
+
+* A specific memory buffer can now be assigned to a FIFO (so buffer external to this framework)
+* New option to dynamically allocate the FIFO buffers using custom memory allocator
+
 ## Version 1.9.1:
 
 * Correction to the management of sharing buffer states. It makes it easier to use this feature from the Python
 
 ## Version 1.9.0:
 
 * Introduced a C++ namespace for the nodes
```

## Comparing `cmsis_stream-1.9.1.dist-info/RECORD` & `cmsis_stream-1.9.2.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 cmsis_stream/cg/nodes/host/WavSink.py,sha256=ldo5e9wjaIp0Ef6GvRgZIICuuk3H1V7B-hn1et6S7Wo,2029
 cmsis_stream/cg/nodes/host/WavSource.py,sha256=KywcbHsrCqrAQD6HuZaxOxVj_ekYDYIgzx_6Nh2R4Gk,2092
 cmsis_stream/cg/nodes/host/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cmsis_stream/cg/nodes/host/message.py,sha256=e2hto5-Ly08sUCKN8F94qH3O3lAxcGGIGBLkf6cLJCY,4018
 cmsis_stream/cg/scheduler/__init__.py,sha256=-GMWFk8b3LpReDjD7yHF_SLrFDu5PRZuxN1RbjkY6nk,118
 cmsis_stream/cg/scheduler/args.py,sha256=mepFm7CJa2wnB-21a-h1FrufP5KtI78l_B3HNb87ayk,1691
 cmsis_stream/cg/scheduler/ccode.py,sha256=mx6xqg3JMDUu6BTjJK0rRXa1vRMautDGHhSQ_I51p-A,3921
-cmsis_stream/cg/scheduler/config.py,sha256=Fyyt0qau1yn8ENrNrNIxaRU5epbuJIpFQcJBGIzcHps,7431
-cmsis_stream/cg/scheduler/description.py,sha256=M3cXQMpx2YntdtN5DaliSXn9dr11XF828iTObPYOK2Q,49788
+cmsis_stream/cg/scheduler/config.py,sha256=Bj7wNY6aA0yJPtpiFuBLHwe3Ce4u5zXvZTZJnLlSRds,7592
+cmsis_stream/cg/scheduler/description.py,sha256=h7Kr78hf8uo8-IDqSZAuQmIqnTHHwkg1zSjPz5ciP-s,52934
 cmsis_stream/cg/scheduler/graphviz.py,sha256=BYqJZAR9Tk3kWCRuxe8G1RzAc2-3wKsV_9TpCG-TV54,10924
 cmsis_stream/cg/scheduler/node.py,sha256=QsV2V_g8sGidTcsiGqPP_9LKANmMZveqn83FWNG0Rlw,38980
 cmsis_stream/cg/scheduler/pythoncode.py,sha256=A5iuUMvzgDJCe7uNyeuhtZA0wZfc4PeSeDXDymeCaKc,1868
 cmsis_stream/cg/scheduler/standard.py,sha256=glYjUqpve4sIevS-lecnQyNUo184yeSQkQ38Zpwn06g,7610
 cmsis_stream/cg/scheduler/example/ARMCM55_FP_MVE_config.txt,sha256=Yn4YtMgyACdeesvFcPkP1xZ9Q8rIEarIAIrJeQNn3sw,188
 cmsis_stream/cg/scheduler/example/Makefile.linux,sha256=4x9Z6tbRIswUvBQuTuD9t0Co-DCwEGevAnaMc3CC5NU,192
 cmsis_stream/cg/scheduler/example/Makefile.mac,sha256=-2ldN02pnOEKwS1QqxY9-97qnUse6MEDZO9Ru1CkplQ,267
@@ -48,25 +48,25 @@
 cmsis_stream/cg/scheduler/example/vht.clayer.yml,sha256=BOZ44mIcb3P2r43vAyff5QkI8r75I5HIzwLOBqcyu2g,878
 cmsis_stream/cg/scheduler/templates/GenericNodes.h,sha256=JO6PF1X1gxjiEFk_VDA1derwg_K4ONOQeVMGUjCwoyY,22424
 cmsis_stream/cg/scheduler/templates/cg_status.h,sha256=1ZBdMG2s9FMyTzdvFtxpPIK624-jnfRd_Q2Qxe_MwTM,2006
 cmsis_stream/cg/scheduler/templates/cmsis.cpp,sha256=Fw5MHQqCZt2srXAuJjvXSHS1m-78DGdT4sGHDEQgG28,434
 cmsis_stream/cg/scheduler/templates/cmsis.py,sha256=iC5sSkuZ01iGT0dBfqNPUbMKE86y10-0Gj8fLOfbgi8,287
 cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp,sha256=JMn_nIJiPYSnu7qVKHS8jKEtAjktGpWSyzxg-r2olgw,682
 cmsis_stream/cg/scheduler/templates/code.cpp,sha256=gzv7k291BlfmcLhsyv8YxW7gJkAd-OvEPN_2oCYNweM,1274
-cmsis_stream/cg/scheduler/templates/code.h,sha256=HrtY5jfNiiAAduF5WsOjHVr8HC9JLvt_MoO-y0tLJdU,1587
+cmsis_stream/cg/scheduler/templates/code.h,sha256=rb5itEroL7bxDCRtMhv0EXZnpDpd8ZuwqjBusvqGYHI,1777
 cmsis_stream/cg/scheduler/templates/code.py,sha256=K77zYiYQdqMGynPVABcWNmxqdGFx9cMfV1yOvuc4u8M,2202
 cmsis_stream/cg/scheduler/templates/codeSwitch.cpp,sha256=0V3Pulno2dA3F4knBRGuzR5crrdncHx5bvgw4h3a7hM,3414
-cmsis_stream/cg/scheduler/templates/commonc.cpp,sha256=87cUOHSVoKXHcn9Ho6ARAAutR58YrOKqvxXQ7M4NmV0,5758
-cmsis_stream/cg/scheduler/templates/defineConfig.h,sha256=3M6qKVSS592DFcic-J3z7820vptCWxoTxBMdU72YBwo,1395
+cmsis_stream/cg/scheduler/templates/commonc.cpp,sha256=bM5AOWd72o4QQL6jRcplm4QkF5C-jIUdd08jVNUk5Ho,6539
+cmsis_stream/cg/scheduler/templates/defineConfig.h,sha256=wF0Of4H1ZL1YsarbDFQyhNhvHi88vV6qYAaG-ccPPNM,1576
 cmsis_stream/cg/scheduler/templates/dot_template.dot,sha256=VGyUY_ze-mMkX-TPn1lrwVemc2jIsNIJk04sxSpfZCs,7858
 cmsis_stream/cg/scheduler/templates/precompute_dot_template.dot,sha256=wLfhZpZS0VHm43dpaQYZBSd8ftd0KdUS_hSo2cSHwLU,7555
 cmsis_stream/cg/sds/__init__.py,sha256=TCh0rypl6S4qKWie66n0ZGYaUGznTLIWOFl_1-2XvLE,26
 cmsis_stream/cg/sds/sds_nodes.py,sha256=NiOBo0gIGYdb9Am0RyFvivrQbDJKpnvMHl4iOZ7zDbc,3923
 cmsis_stream/cg/yaml/__init__.py,sha256=nv4KwU4bqDQoREFYliOSnL98MkQxwMh40Kmy8aGfReY,104
 cmsis_stream/cg/yaml/exportyaml.py,sha256=WyxnvUecO2iV7NspfpcTE3KQ0D_NPU7JqbrC8Vn7Gzc,15372
 cmsis_stream/cg/yaml/importyaml.py,sha256=8BY2eUoZTkkJwSta9B5_4LIcMltLh-C1GHX_aIB1cLo,17272
-cmsis_stream-1.9.1.dist-info/LICENSE.txt,sha256=4DukHX-rIHAHaf5BGLq1DYAMt0-ZA1OgXS9f_xwig2M,11558
-cmsis_stream-1.9.1.dist-info/METADATA,sha256=XNiBiGJTlI0g3f1TBxJK8SXZ9txbVTuFOg0q8fFKmto,5676
-cmsis_stream-1.9.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-cmsis_stream-1.9.1.dist-info/entry_points.txt,sha256=WOEqwaMTN0K5CT8Yfd-z53mE82xfyzsM16a0eR4Ipds,59
-cmsis_stream-1.9.1.dist-info/top_level.txt,sha256=a7ZhPCd-XkrgWSSuOstN5Jgqe60MV4q7-tWximJBomA,13
-cmsis_stream-1.9.1.dist-info/RECORD,,
+cmsis_stream-1.9.2.dist-info/LICENSE.txt,sha256=4DukHX-rIHAHaf5BGLq1DYAMt0-ZA1OgXS9f_xwig2M,11558
+cmsis_stream-1.9.2.dist-info/METADATA,sha256=l9CAzlKVjkNMQldtt7ni3lHAIkAqHwZYnYPj3wtJlAs,5881
+cmsis_stream-1.9.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+cmsis_stream-1.9.2.dist-info/entry_points.txt,sha256=WOEqwaMTN0K5CT8Yfd-z53mE82xfyzsM16a0eR4Ipds,59
+cmsis_stream-1.9.2.dist-info/top_level.txt,sha256=a7ZhPCd-XkrgWSSuOstN5Jgqe60MV4q7-tWximJBomA,13
+cmsis_stream-1.9.2.dist-info/RECORD,,
```

