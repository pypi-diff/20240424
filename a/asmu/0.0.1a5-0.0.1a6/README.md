# Comparing `tmp/asmu-0.0.1a5.tar.gz` & `tmp/asmu-0.0.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asmu-0.0.1a5.tar", last modified: Tue Apr  9 15:01:18 2024, max compression
+gzip compressed data, was "asmu-0.0.1a6.tar", last modified: Wed Apr 24 09:15:14 2024, max compression
```

## Comparing `asmu-0.0.1a5.tar` & `asmu-0.0.1a6.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:01:18.195669 asmu-0.0.1a5/
--rw-rw-rw-   0 root         (0) root         (0)    35148 2024-04-09 15:01:06.000000 asmu-0.0.1a5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1617 2024-04-09 15:01:18.195669 asmu-0.0.1a5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      939 2024-04-09 15:01:06.000000 asmu-0.0.1a5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:01:18.193668 asmu-0.0.1a5/asmu/
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-04-09 15:01:06.000000 asmu-0.0.1a5/asmu/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2084 2024-04-09 15:01:06.000000 asmu-0.0.1a5/asmu/afile.py
--rw-rw-rw-   0 root         (0) root         (0)     2538 2024-04-09 15:01:06.000000 asmu-0.0.1a5/asmu/analyzer.py
--rw-rw-rw-   0 root         (0) root         (0)     2404 2024-04-09 15:01:06.000000 asmu-0.0.1a5/asmu/asetup.py
--rw-rw-rw-   0 root         (0) root         (0)     5557 2024-04-09 15:01:06.000000 asmu-0.0.1a5/asmu/generator.py
--rw-rw-rw-   0 root         (0) root         (0)     2132 2024-04-09 15:01:06.000000 asmu-0.0.1a5/asmu/inout.py
--rw-rw-rw-   0 root         (0) root         (0)     3790 2024-04-09 15:01:06.000000 asmu-0.0.1a5/asmu/interface.py
--rw-rw-rw-   0 root         (0) root         (0)     4112 2024-04-09 15:01:06.000000 asmu-0.0.1a5/asmu/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:01:18.195669 asmu-0.0.1a5/asmu.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1617 2024-04-09 15:01:18.000000 asmu-0.0.1a5/asmu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      297 2024-04-09 15:01:18.000000 asmu-0.0.1a5/asmu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 15:01:18.000000 asmu-0.0.1a5/asmu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-09 15:01:18.000000 asmu-0.0.1a5/asmu.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-09 15:01:18.000000 asmu-0.0.1a5/asmu.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      739 2024-04-09 15:01:06.000000 asmu-0.0.1a5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 15:01:18.195669 asmu-0.0.1a5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:15:14.773004 asmu-0.0.1a6/
+-rw-rw-rw-   0 root         (0) root         (0)    35148 2024-04-24 09:15:01.000000 asmu-0.0.1a6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      777 2024-04-24 09:15:14.773004 asmu-0.0.1a6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       99 2024-04-24 09:15:01.000000 asmu-0.0.1a6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:15:14.772004 asmu-0.0.1a6/asmu/
+-rw-rw-rw-   0 root         (0) root         (0)      551 2024-04-24 09:15:01.000000 asmu-0.0.1a6/asmu/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3485 2024-04-24 09:15:01.000000 asmu-0.0.1a6/asmu/afile.py
+-rw-rw-rw-   0 root         (0) root         (0)     2786 2024-04-24 09:15:01.000000 asmu-0.0.1a6/asmu/analyzer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3207 2024-04-24 09:15:01.000000 asmu-0.0.1a6/asmu/asetup.py
+-rw-rw-rw-   0 root         (0) root         (0)     6150 2024-04-24 09:15:01.000000 asmu-0.0.1a6/asmu/generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    10972 2024-04-24 09:15:01.000000 asmu-0.0.1a6/asmu/io.py
+-rw-rw-rw-   0 root         (0) root         (0)     4130 2024-04-24 09:15:01.000000 asmu-0.0.1a6/asmu/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:15:14.773004 asmu-0.0.1a6/asmu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      777 2024-04-24 09:15:14.000000 asmu-0.0.1a6/asmu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      276 2024-04-24 09:15:14.000000 asmu-0.0.1a6/asmu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 09:15:14.000000 asmu-0.0.1a6/asmu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-24 09:15:14.000000 asmu-0.0.1a6/asmu.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-24 09:15:14.000000 asmu-0.0.1a6/asmu.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      739 2024-04-24 09:15:02.000000 asmu-0.0.1a6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 09:15:14.774004 asmu-0.0.1a6/setup.cfg
```

### Comparing `asmu-0.0.1a5/LICENSE` & `asmu-0.0.1a6/LICENSE`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1a5/asmu/afile.py` & `asmu-0.0.1a6/asmu/analyzer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,96 @@
-import soundfile
-import tempfile
-import shutil
-import os
-import json
-from datetime import datetime
-
-
-class AFile(soundfile.SoundFile):
-    def __init__(self, signal_path, mode="r", samplerate=None, channels=None):
-        self._signal_path = signal_path
-        if mode == "r":
-            super().__init__(signal_path)
-        else:
-            _name = os.path.split(signal_path)[1].replace(".wav", "")
-            self._tmp = tempfile.NamedTemporaryFile(prefix=_name, suffix='.wav', dir="", delete=True)
-            super().__init__(self._tmp, mode=mode, samplerate=samplerate, channels=channels, subtype="PCM_24", format="WAV")
-            now = datetime.now()
-            # set wav metadata
-            self.title = _name
-            self.date = now.strftime("%d/%m/%Y %H:%M:%S")
+import numpy as np
+import scipy as sp
+import queue
+import threading
+
+class Analyzer():
+    def __init__(self, queuesize):
+        """_summary_
+
+        Args:
+            queuesize (_type_): _description_
+        """
+        self._q = queue.Queue(queuesize)
+
+    def reset(self):
+        # process full queue
+        while not self._q.empty():
+            self._process_queue()
+
+    def put_queue(self, data):
+        self._q.put(data.copy())
+
+    def _process_queue(self):
+        raise NotImplementedError("Subclass has to define a process_queue function!")
+
+    def start_process_thread(self, stream):
+        def runner(self, stream):
+            while stream.active:
+                try:
+                    self._process_queue()
+                except queue.Empty:
+                    pass
+        threading.Thread(target=runner, args=(self, stream, )).start()
+
+
+    def _get_fft(self) -> np.ndarray:
+        raise NotImplementedError() # TODO: Move this to helper function
+        return np.fft.rfft(self._q.get()*self._w, axis=0, norm="forward")*2/np.mean(self._w)
     
-    # store settings as json string in metadata "comment"
-    @property
-    def settings(self):
-        if not self.comment:
-            return {}
-        else:
-            return json.loads(self.comment)
-    @settings.setter
-    def settings(self, value):
-        self.comment = json.dumps(value)
-
-    @property
-    def latency(self):
-        try:
-            return int(self.settings["latency"])
-        except KeyError:
-            return None
-    @latency.setter
-    def latency(self, value):
-        self.settings = {"latency": int(value)}
-
-    @property
-    def data(self):
-        self.flush()
-        self.seek(0)
-        return self.read(dtype="float32", always_2d=True)
+class Recorder(Analyzer):
+    def __init__(self, signal, queuesize=10):
+        """_summary_
+
+        Args:
+            signal (_type_): _description_
+            queuesize (int, optional): _description_. Defaults to 10.
+        """
+        self._signal = signal
+        super().__init__(queuesize)
+        
+    def _process_queue(self):
+        self._signal.write(self._q.get(timeout=0.2))
+
+class calSPL(Analyzer):
+    def __init__(self, queuesize: int=10):
+        self._uks = []
+        self._ks = []
+        super().__init__(queuesize)
+
+    def _process_queue(self):
+        ukm = self._get_fft()
+
+        kmax = np.argmax(np.abs(ukm))
+        self._uks.append(np.abs(ukm[kmax]))
+        self._ks.append(kmax)
+
+    def get_cSPL(self, spl):
+        self.reset()
+
+        p0 = 2e-5                           # [Pa]Rms
+        p = p0 * 10 ** (spl / 20)           # [Pa]Rms
+        pcal = p * np.sqrt(2)               # [Pa]
+
+        return pcal/np.mean(self._uks[2:]) # dont use the first three measurements
+
+    def get_kSPL(self):
+        return round(np.mean(self._ks))
     
-    def __getattr__(self, name):
-        try:
-            return super().__getattr__(name)
-        except AttributeError:
-            return object.__getattribute__(self, name)
-
-    def cal_latency(self, time):
-       self.latency = round((time.outputBufferDacTime-time.inputBufferAdcTime)*self.samplerate + 1) # the +1 was measured experimentally (could be the cable?)
-
-    def save_file(self):
-        # persist temporary file in specified recording location
-        self.flush()
-        self._tmp.seek(0)
-        with open(self._signal_path, 'wb') as file:
-            shutil.copyfileobj(self._tmp, file)
+def get_corrs_sampleshifts(indata: np.ndarray, refdata: np.ndarray, burstLength: int) -> tuple[np.ndarray, np.ndarray]:
+    corrs = []
+    sampleshifts = []
+    n = int(np.size(refdata))
+    for cidx in range(np.ma.size(indata, axis=1)):
+        v = indata[:, cidx]
+        corr = sp.signal.correlate(v, refdata)
+        corr /= np.max(corr)
+        peaks, _ = sp.signal.find_peaks(corr, prominence=0.8, distance=burstLength, height=0.5)
+
+        # shift correlation correctly
+        corrs.append(corr[n-1:])
+        sampleshifts.append(peaks[0]-(n-1))
+    return np.array(corrs).T, np.array(sampleshifts)
 
 
+            
+
```

### Comparing `asmu-0.0.1a5/asmu/generator.py` & `asmu-0.0.1a6/asmu/generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import numpy as np
 import scipy as sp
 import threading
 import queue
 
 class Generator():
     def __init__(self, queuesize) -> None:
+        """_summary_
+
+        Args:
+            queuesize (_type_): _description_
+        """
         self._q = queue.Queue(queuesize)
         self._prefill_queue()
 
     def get_queue(self) -> queue.Queue:
         return self._q.get_nowait()
 
     def _prefill_queue(self) -> None:
@@ -29,148 +34,155 @@
                     pass
         threading.Thread(target=runner, args=(self, stream, )).start()
     
     def _gen(self):
         raise NotImplementedError("Subclass has to define a _gen function!")
 
 class Player(Generator):
-    def __init__(self, asfile, chunk, queuesize=10):
+    def __init__(self, asfile, blocksize, queuesize=10):
+        """_summary_
+
+        Args:
+            asfile (_type_): _description_
+            blocksize (_type_): _description_
+            queuesize (int, optional): _description_. Defaults to 10.
+        """
         self._asfile = asfile
-        self._chunk = chunk
+        self._blocksize = blocksize
         super().__init__(queuesize)
 
     def _gen(self):
-        data = self._asfile.read(self._chunk, dtype="float32", always_2d=True)
+        data = self._asfile.read(self._blocksize, dtype="float32", always_2d=True)
         length = np.ma.size(data, axis=0)
         if data.size == 0:
             return None
-        elif length < self._chunk:
-            pad = np.zeros((self._chunk, self._asfile.channels))
+        elif length < self._blocksize:
+            pad = np.zeros((self._blocksize, self._asfile.channels))
             pad[:length, :] = data
             return pad
         else:
             return data
 
 class Chirp(Generator):
-    def __init__(self, rate: int, chunk: int, f0: float, f1: float, duration: int, queuesize: int=10) -> None:
-        self._rate = rate
-        self._chunk = chunk
+    def __init__(self, samplerate: int, blocksize: int, f0: float, f1: float, duration: int, queuesize: int=10) -> None:
+        self._samplerate = samplerate
+        self._blocksize = blocksize
         
-        t = np.arange(0, int(duration*rate)) / rate
+        t = np.arange(0, int(duration*samplerate)) / samplerate
         self._chirp = sp.signal.chirp(t, f0=f0, t1=duration, f1=f1, method="logarithmic")
         self._idx = 0
         super().__init__(queuesize)
     
     def _gen(self) -> np.ndarray:
-        data = self._chirp[self._idx:self._idx+self._chunk]
-        self._idx += self._chunk
+        data = self._chirp[self._idx:self._idx+self._blocksize]
+        self._idx += self._blocksize
 
         length = np.ma.size(data, axis=0)
         if data.size == 0:
             return None
-        elif length < self._chunk:
-            pad = np.zeros(self._chunk)
+        elif length < self._blocksize:
+            pad = np.zeros(self._blocksize)
             pad[:length] = data
             return pad
         else:
             return data
 
 
 class SineBurst(Generator):
-    def __init__(self, rate: int, chunk: int, f: float, n: int, loop: float=-1, queuesize: int=10) -> None:
-        self._rate = rate
-        self._chunk = chunk
+    def __init__(self, samplerate: int, blocksize: int, f: float, n: int, loop: float=-1, queuesize: int=10) -> None:
+        self._samplerate = samplerate
+        self._blocksize = blocksize
         self._freq = f
 
         # generate wave parameters
-        self._omegas = np.linspace(0, 2*np.pi*f*chunk/rate, chunk, endpoint=False, dtype=np.float32)
+        self._omegas = np.linspace(0, 2*np.pi*f*blocksize/samplerate, blocksize, endpoint=False, dtype=np.float32)
         self._phi = 0
         self._maxang = 2*np.pi*n
         self._loopang = 2*np.pi*loop*f
 
         super().__init__(queuesize)
 
     @property
     def burstlen(self):
-        return self._rate/(2*np.pi*self._freq)*self._maxang
+        return self._samplerate/(2*np.pi*self._freq)*self._maxang
 
     def _gen(self) -> np.ndarray:
         ang = self._omegas + self._phi
         if self._loopang > 0: ang = np.mod(ang, self._loopang)
         sineburst = np.sin(ang)
         sineburst[ang > self._maxang] = 0
-        self._phi += 2*np.pi*self._freq*self._chunk/self._rate
+        self._phi += 2*np.pi*self._freq*self._blocksize/self._samplerate
         return sineburst
     
 class SincBurst(Generator):
-    def __init__(self, rate: int, chunk: int, f: float, n: int, loop: float=-1, queuesize: int=10) -> None:
-        self._rate = rate
-        self._chunk = chunk
+    def __init__(self, samplerate: int, blocksize: int, f: float, n: int, loop: float=-1, queuesize: int=10) -> None:
+        self._samplerate = samplerate
+        self._blocksize = blocksize
         self._freq = f
 
         # generate wave parameters
-        self._omegas = np.linspace(0, 2*np.pi*f*chunk/rate, chunk, endpoint=False, dtype=np.float32)
+        self._omegas = np.linspace(0, 2*np.pi*f*blocksize/samplerate, blocksize, endpoint=False, dtype=np.float32)
         self._phi = 0
         self._maxang = 2*np.pi*n
         self._loopang = 2*np.pi*loop*f
 
         super().__init__(queuesize)
 
     @property
     def burstlen(self):
-        return self._rate/(2*np.pi*self._freq)*self._maxang
+        return self._samplerate/(2*np.pi*self._freq)*self._maxang
 
     def _gen(self) -> np.ndarray:
         ang = self._omegas + self._phi
         if self._loopang > 0: ang = np.mod(ang, self._loopang)
         sincburst = np.sinc((ang-self._maxang/2)/np.pi)
         sincburst[ang > self._maxang] = 0
-        self._phi += 2*np.pi*self._freq*self._chunk/self._rate
+        self._phi += 2*np.pi*self._freq*self._blocksize/self._samplerate
         return sincburst
         
 class WhiteNoise(Generator):
-    def __init__(self, chunk: int, queuesize: int=10) -> None:
-        self._chunk = chunk
+    def __init__(self, blocksize: int, queuesize: int=10) -> None:
+        self._blocksize = blocksize
 
         super().__init__(queuesize)
 
     def _gen(self) -> np.ndarray:
-        fwhite = np.fft.rfft(np.random.randn(self._chunk))
+        fwhite = np.fft.rfft(np.random.randn(self._blocksize))
         return np.clip(np.fft.irfft(fwhite)/4, -1, 1)
     
 class PinkNoise(Generator):
-    def __init__(self, chunk: int, queuesize: int=10) -> None:
-        self._chunk = chunk
+    def __init__(self, blocksize: int, queuesize: int=10) -> None:
+        self._blocksize = blocksize
 
         super().__init__(queuesize)
 
     def _gen(self) -> np.ndarray:
-        fwhite = np.fft.rfft(np.random.randn(self._chunk))
+        fwhite = np.fft.rfft(np.random.randn(self._blocksize))
 
         # apply noise color and normalize for power
-        f = np.fft.rfftfreq(self._chunk)
+        f = np.fft.rfftfreq(self._blocksize)
         S = 1/np.where(f == 0, float('inf'), np.sqrt(f))
         S = S / np.sqrt(np.mean(S**2))
         fpink = fwhite * S
 
         return np.clip(np.fft.irfft(fpink)/4, -1, 1)
 
 class Sine(Generator):
-    def __init__(self, rate: int, chunk: int, f: float, queuesize: int=10) -> None:
-        self._rate = rate
-        self._chunk = chunk
+    def __init__(self, samplerate: int, blocksize: int, f: float, queuesize: int=10) -> None:
+        self._samplerate = samplerate
+        self._blocksize = blocksize
         self._freq = f
 
         # generate wave parameters
-        self._omegas = np.linspace(0, 2*np.pi*f*chunk/rate, chunk, endpoint=False, dtype=np.float32)
+        self._omegas = np.linspace(0, 2*np.pi*f*blocksize/samplerate, blocksize, endpoint=False, dtype=np.float32)
         self._phi = 0
 
         super().__init__(queuesize)
 
     def _gen(self) -> np.ndarray:
         ang = self._omegas + self._phi
-        self._phi += 2*np.pi*self._freq*self._chunk/self._rate
+        self._phi += 2*np.pi*self._freq*self._blocksize/self._samplerate
         self._phi %= 2*np.pi
         return np.sin(ang)
```

### Comparing `asmu-0.0.1a5/asmu/view.py` & `asmu-0.0.1a6/asmu/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 import queue
 import threading
 
 pg.setConfigOption('background', 'k')
 pg.setConfigOption('foreground', 'w')
 
 class TimeView(pg.PlotWidget):
-    def __init__(self, ioNames, ioColors, rate, queuesize:int=10, parent=None):
+    def __init__(self, ioNames, ioColors, samplerate, queuesize:int=10, parent=None):
         super(TimeView, self).__init__(parent)
         # TODO give list of input classes instead?
         self.ioNames = ioNames
         self.ioQColors = [QtGui.QColor(ioColor) for ioColor in ioColors]
 
-        self._rate = rate
+        self._samplerate = samplerate
         self.initPlots()
 
         self._q = queue.Queue(queuesize)
 
     def put_queue(self, data):
         self._q.put(data.copy())
```

### Comparing `asmu-0.0.1a5/pyproject.toml` & `asmu-0.0.1a6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.2.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asmu"
-version = "v0.0.1a5"
+version = "v0.0.1a6"
 authors = [
     {name = "felhub", email = "felhub@net4us.at"},
 ]
 description = "Acoustic Signal Measurement Utilities"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

