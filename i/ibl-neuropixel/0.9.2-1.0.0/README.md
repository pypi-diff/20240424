# Comparing `tmp/ibl-neuropixel-0.9.2.tar.gz` & `tmp/ibl_neuropixel-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibl-neuropixel-0.9.2.tar", last modified: Thu Feb  8 18:31:34 2024, max compression
+gzip compressed data, was "ibl_neuropixel-1.0.0.tar", last modified: Wed Apr 24 15:06:49 2024, max compression
```

## Comparing `ibl-neuropixel-0.9.2.tar` & `ibl_neuropixel-1.0.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 18:31:34.216475 ibl-neuropixel-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-02-08 18:31:34.216475 ibl-neuropixel-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 18:31:34.216475 ibl-neuropixel-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 18:31:34.212475 ibl-neuropixel-0.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 18:31:34.216475 ibl-neuropixel-0.9.2/src/ibl_neuropixel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-02-08 18:31:34.000000 ibl-neuropixel-0.9.2/src/ibl_neuropixel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-02-08 18:31:34.000000 ibl-neuropixel-0.9.2/src/ibl_neuropixel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 18:31:34.000000 ibl-neuropixel-0.9.2/src/ibl_neuropixel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-08 18:31:34.000000 ibl-neuropixel-0.9.2/src/ibl_neuropixel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-08 18:31:34.000000 ibl-neuropixel-0.9.2/src/ibl_neuropixel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 18:31:34.216475 ibl-neuropixel-0.9.2/src/ibldsp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/cadzow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/cuda_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/destripe_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/filter_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)    10529 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/fourier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/raw_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/spiketrains.py
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34333 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/voltage.py
--rw-r--r--   0 runner    (1001) docker     (127)    22161 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/waveforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 18:31:34.216475 ibl-neuropixel-0.9.2/src/neurodsp/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/neurodsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36357 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/neuropixel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 18:31:34.216475 ibl-neuropixel-0.9.2/src/neurowaveforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/neurowaveforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/neurowaveforms/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    34528 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/spikeglx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:06:49.379966 ibl_neuropixel-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-24 15:06:49.379966 ibl_neuropixel-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:06:49.379966 ibl_neuropixel-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:06:49.375966 ibl_neuropixel-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:06:49.379966 ibl_neuropixel-1.0.0/src/ibl_neuropixel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-24 15:06:49.000000 ibl_neuropixel-1.0.0/src/ibl_neuropixel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-24 15:06:49.000000 ibl_neuropixel-1.0.0/src/ibl_neuropixel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:06:49.000000 ibl_neuropixel-1.0.0/src/ibl_neuropixel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-24 15:06:49.000000 ibl_neuropixel-1.0.0/src/ibl_neuropixel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 15:06:49.000000 ibl_neuropixel-1.0.0/src/ibl_neuropixel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:06:49.375966 ibl_neuropixel-1.0.0/src/ibldsp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/cadzow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/cuda_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/destripe_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/filter_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/fourier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/raw_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/spiketrains.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10073 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37561 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/voltage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14015 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/waveform_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28777 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/waveforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:06:49.379966 ibl_neuropixel-1.0.0/src/neurodsp/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/neurodsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36748 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/neuropixel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:06:49.379966 ibl_neuropixel-1.0.0/src/neurowaveforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/neurowaveforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/neurowaveforms/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37250 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/spikeglx.py
```

### Comparing `ibl-neuropixel-0.9.2/LICENSE` & `ibl_neuropixel-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.9.2/PKG-INFO` & `ibl_neuropixel-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibl-neuropixel
-Version: 0.9.2
+Version: 1.0.0
 Summary: Collection of tools for Neuropixel 1.0 and 2.0 probes data
 Home-page: https://github.com/int-brain-lab/ibl-neuropixel
 Author: The International Brain Laboratory
 Project-URL: Bug Tracker, https://github.com/int-brain-lab/ibl-neuropixel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -43,15 +43,15 @@
 ```
 
 ### Viewer
 
 The best way to look at the results is to use [viewephys](https://github.com/oliche/viewephys),
 open an ephys viewer on the raw data.
 
-- tick the destipe box.
+- tick the destripe box.
 - move to a desired location in the file
 - ctr+P will make the gain and axis the same on both windows
 
 ![alt text](./docs/raw_bin_viewer_destripe.png "Ephys viewer")
 
 You can then move within the raw data file.
```

### Comparing `ibl-neuropixel-0.9.2/README.md` & `ibl_neuropixel-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ```
 
 ### Viewer
 
 The best way to look at the results is to use [viewephys](https://github.com/oliche/viewephys),
 open an ephys viewer on the raw data.
 
-- tick the destipe box.
+- tick the destripe box.
 - move to a desired location in the file
 - ctr+P will make the gain and axis the same on both windows
 
 ![alt text](./docs/raw_bin_viewer_destripe.png "Ephys viewer")
 
 You can then move within the raw data file.
```

### Comparing `ibl-neuropixel-0.9.2/setup.py` & `ibl_neuropixel-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-with open('requirements.txt') as f:
-    require = [x.strip() for x in f.readlines() if not x.startswith('git+')]
+with open("requirements.txt") as f:
+    require = [x.strip() for x in f.readlines() if not x.startswith("git+")]
 
 setuptools.setup(
     name="ibl-neuropixel",
-    version="0.9.2",
+    version="1.0.0",
     author="The International Brain Laboratory",
     description="Collection of tools for Neuropixel 1.0 and 2.0 probes data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/int-brain-lab/ibl-neuropixel",
     project_urls={
         "Bug Tracker": "https://github.com/int-brain-lab/ibl-neuropixel/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=require,
-    package_dir={'': 'src'},
-    packages=setuptools.find_packages(where="src", exclude=['tests']),
+    package_dir={"": "src"},
+    packages=setuptools.find_packages(where="src", exclude=["tests"]),
     include_package_data=True,
-    py_modules=['spikeglx', 'neuropixel'],
+    py_modules=["spikeglx", "neuropixel"],
     python_requires=">=3.8",
 )
```

### Comparing `ibl-neuropixel-0.9.2/src/ibl_neuropixel.egg-info/PKG-INFO` & `ibl_neuropixel-1.0.0/src/ibl_neuropixel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibl-neuropixel
-Version: 0.9.2
+Version: 1.0.0
 Summary: Collection of tools for Neuropixel 1.0 and 2.0 probes data
 Home-page: https://github.com/int-brain-lab/ibl-neuropixel
 Author: The International Brain Laboratory
 Project-URL: Bug Tracker, https://github.com/int-brain-lab/ibl-neuropixel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -43,15 +43,15 @@
 ```
 
 ### Viewer
 
 The best way to look at the results is to use [viewephys](https://github.com/oliche/viewephys),
 open an ephys viewer on the raw data.
 
-- tick the destipe box.
+- tick the destripe box.
 - move to a desired location in the file
 - ctr+P will make the gain and axis the same on both windows
 
 ![alt text](./docs/raw_bin_viewer_destripe.png "Ephys viewer")
 
 You can then move within the raw data file.
```

### Comparing `ibl-neuropixel-0.9.2/src/ibl_neuropixel.egg-info/SOURCES.txt` & `ibl_neuropixel-1.0.0/src/ibl_neuropixel.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -16,11 +16,12 @@
 src/ibldsp/filter_gpu.py
 src/ibldsp/fourier.py
 src/ibldsp/raw_metrics.py
 src/ibldsp/smooth.py
 src/ibldsp/spiketrains.py
 src/ibldsp/utils.py
 src/ibldsp/voltage.py
+src/ibldsp/waveform_extraction.py
 src/ibldsp/waveforms.py
 src/neurodsp/__init__.py
 src/neurowaveforms/__init__.py
 src/neurowaveforms/model.py
```

### Comparing `ibl-neuropixel-0.9.2/src/ibldsp/cadzow.py` & `ibl_neuropixel-1.0.0/src/ibldsp/cadzow.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,15 +95,25 @@
             WAV_[:, ind_f] = np.bincount(itr, weights=np.real(T_[it]))
             WAV_[:, ind_f] += 1j * np.bincount(itr, weights=np.imag(T_[it]))
             WAV_[:, ind_f] /= trcount
 
     return WAV_
 
 
-def cadzow_np1(wav, fs=30000, rank=5, niter=1, fmax=7500, h=None, ovx=int(16), nswx=int(32), npad=int(0)):
+def cadzow_np1(
+    wav,
+    fs=30000,
+    rank=5,
+    niter=1,
+    fmax=7500,
+    h=None,
+    ovx=int(16),
+    nswx=int(32),
+    npad=int(0),
+):
     """
     Apply Fxy rank-denoiser to a full recording of Neuropixel 1 probe geometry
     ntr - nswx has to be a multiple of (nswx - ovx)
     Examples of working set of parameters:
         ovx = int(5); nswx = int(33); ovx = int(6))
         ovx = int(16); nswx = int(32); ovx = int(0))
         ovx = int(32); nswx = int(64); ovx = int(0))
@@ -120,19 +130,25 @@
     ntr, ns = wav.shape
     h = h or neuropixel.trace_header(version=1)
     nwinx = int(np.ceil((ntr + npad * 2 - ovx) / (nswx - ovx)))
     fscale = scipy.fft.rfftfreq(ns, d=1 / fs)
     imax = np.searchsorted(fscale, fmax)
     WAV = scipy.fft.rfft(wav[:, :])
     padgain = scipy.signal.windows.hann(npad * 2)[:npad]
-    WAV = np.r_[np.flipud(WAV[1:npad + 1, :]) * padgain[:, np.newaxis],
-                WAV,
-                np.flipud(WAV[-npad - 2: - 1, :]) * np.flipud(np.r_[padgain, 1])[:, np.newaxis]]  # apply padding
-    x = np.r_[np.flipud(h['x'][1:npad + 1]), h['x'], np.flipud(h['x'][-npad - 2: - 1])]
-    y = np.r_[np.flipud(h['y'][1:npad + 1]) - 120, h['y'], np.flipud(h['y'][-npad - 2: - 1]) + 120]
+    WAV = np.r_[
+        np.flipud(WAV[1: npad + 1, :]) * padgain[:, np.newaxis],
+        WAV,
+        np.flipud(WAV[-npad - 2: -1, :]) * np.flipud(np.r_[padgain, 1])[:, np.newaxis],
+    ]  # apply padding
+    x = np.r_[np.flipud(h["x"][1: npad + 1]), h["x"], np.flipud(h["x"][-npad - 2: -1])]
+    y = np.r_[
+        np.flipud(h["y"][1: npad + 1]) - 120,
+        h["y"],
+        np.flipud(h["y"][-npad - 2: -1]) + 120,
+    ]
     WAV_ = np.zeros_like(WAV)
     gain = np.zeros(ntr + npad * 2 + 1)
     hanning = scipy.signal.windows.hann(ovx * 2 - 1)[0:ovx]
     assert np.all(np.isclose(hanning + np.flipud(hanning), 1))
     gain_window = np.r_[hanning, np.ones(nswx - ovx * 2), np.flipud(hanning)]
     for firstx in np.arange(nwinx) * (nswx - ovx):
         lastx = int(firstx + nswx)
@@ -140,13 +156,15 @@
             gw = np.r_[hanning * 0 + 1, np.ones(nswx - ovx * 2), np.flipud(hanning)]
         elif lastx == ntr:
             gw = np.r_[hanning, np.ones(nswx - ovx * 2), hanning * 0 + 1]
         else:
             gw = gain_window
         gain[firstx:lastx] += gw
         array = WAV[firstx:lastx, :]
-        array = denoise(array, x=x[firstx:lastx], y=y[firstx:lastx], r=rank, imax=imax, niter=niter)
+        array = denoise(
+            array, x=x[firstx:lastx], y=y[firstx:lastx], r=rank, imax=imax, niter=niter
+        )
         WAV_[firstx:lastx, :] += array * gw[:, np.newaxis]
 
-    WAV_ = WAV_[npad:-npad - 1]  # remove padding
+    WAV_ = WAV_[npad: -npad - 1]  # remove padding
     wav_ = scipy.fft.irfft(WAV_)
     return wav_
```

### Comparing `ibl-neuropixel-0.9.2/src/ibldsp/cuda_tools.py` & `ibl_neuropixel-1.0.0/src/ibldsp/cuda_tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,75 @@
 import re
 from pathlib import Path
 
 from iblutil.util import Bunch
 
 
-REGEX_PATTERN = r'const int\s+\S+\s+=\s+\S+.+'
+REGEX_PATTERN = r"const int\s+\S+\s+=\s+\S+.+"
 
 
 def get_cuda(fn, **constants):
     """
     Finds the CUDA code for a function and optionally changes the default constants
     :param fn: String, name of cuda function
     :param constants: Integer constants to replace
     :return: code: String
              constants: Bunch
     """
-    path = Path(__file__).parent / (fn + '.cu')
+    path = Path(__file__).parent / (fn + ".cu")
     assert path.exists
     code = path.read_text()
-    code = code.replace('__global__ void', 'extern "C" __global__ void')
+    code = code.replace("__global__ void", 'extern "C" __global__ void')
     if not constants:
         return code, Bunch(extract_constants_from_cuda(code))
     return change_cuda_constants(code, constants)
 
 
 def extract_constants_from_cuda(code):
     """
     Find integer constants in the CUDA function
     :param code: String, CUDA function
     :return: names and values of integer constants
     """
     r = re.compile(REGEX_PATTERN)
     m = r.search(code)
     if m:
-        constants = m.group(0).replace('const int', '').replace(';', '').split(',')
+        constants = m.group(0).replace("const int", "").replace(";", "").split(",")
         for const in constants:
-            a, b = const.strip().split('=')
+            a, b = const.strip().split("=")
             yield a.strip(), int(b.strip())
 
 
 def change_cuda_constants(code, constants):
     """
     Changes default integer constants in the CUDA function with any that are passed
     :param code: String, CUDA function
     :param constants: dict, constants to change
     :return: code: String
              constants: Bunch
     """
     r = re.compile(REGEX_PATTERN)
     m = r.match(code)
-    assert m, 'No constants found in CUDA code'
+    assert m, "No constants found in CUDA code"
     pattern_length = m.span(0)[1] - 1
-    default_constants_string = m.group(0).replace('const int', '').replace(';', '').split(',')
+    default_constants_string = (
+        m.group(0).replace("const int", "").replace(";", "").split(",")
+    )
     code_constants = {}
 
     # Find default constants in CUDA code
     for default_constants_string in default_constants_string:
-        name, value = default_constants_string.split('=')
+        name, value = default_constants_string.split("=")
         code_constants[name.strip()] = int(value.strip())
 
     # Replace default constants with the new user constants
     for name, value in constants.items():
         code_constants[name] = value
 
     new_strings = []
     for name, value in code_constants.items():
-        new_strings.append(f'{name} = {value}')
-    new_constants_string = ', '.join(new_strings)
+        new_strings.append(f"{name} = {value}")
+    new_constants_string = ", ".join(new_strings)
 
-    new_code = f'const int  {new_constants_string}{code[pattern_length:]}'
+    new_code = f"const int  {new_constants_string}{code[pattern_length:]}"
 
     return new_code, Bunch(code_constants)
```

### Comparing `ibl-neuropixel-0.9.2/src/ibldsp/destripe_gpu.py` & `ibl_neuropixel-1.0.0/src/ibldsp/destripe_gpu.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,24 @@
 from scipy.signal import butter
 
 from .filter_gpu import sosfiltfilt_gpu
 from .fourier import channel_shift
 from .voltage import _get_destripe_parameters, interpolate_bad_channels, kfilt
 
 
-def destripe_array(data, fs=30000, fshigh=300., taper_size=64, sample_shifts=None, channel_labels=None,
-                   channel_xcoords=None, channel_ycoords=None):
+def destripe_array(
+    data,
+    fs=30000,
+    fshigh=300.0,
+    taper_size=64,
+    sample_shifts=None,
+    channel_labels=None,
+    channel_xcoords=None,
+    channel_ycoords=None,
+):
     """
     Applies de-striping to a cupy array
     :param data: float32 cupy array, shape (n_channels, n_times)
     :param fs: Int, sampling rate
     :param fshigh: Float, high pass frequency
     :param taper_size: Int, length of cosine taper applied either side of data
     :param sample_shifts: Time shifts of channels, array with shape (n_channels)
@@ -35,25 +43,29 @@
         data[:, -taper_size:] *= taper[taper_size:]
 
     # butterworth filter along time axis
     data = sosfiltfilt_gpu(sos, data)
 
     # align channels if the time shifts are provided
     if sample_shifts is not None:
-        sample_shifts = cp.array(sample_shifts, dtype='float32')
+        sample_shifts = cp.array(sample_shifts, dtype="float32")
         data = channel_shift(data, sample_shifts)
 
     # apply spatial filter
     # TODO: Currently using default settings, should allow user to change this in function arguments
     kfilt_kwargs = _get_destripe_parameters(fs, None, None, True)[1]
 
     if channel_labels is not None:
-        data = interpolate_bad_channels(data, channel_labels, channel_xcoords, channel_ycoords, gpu=True)
+        data = interpolate_bad_channels(
+            data, channel_labels, channel_xcoords, channel_ycoords, gpu=True
+        )
         inside_brain = cp.where(channel_labels != 3)[0]
-        data[inside_brain, :] = kfilt(data[inside_brain, :], gpu=True, **kfilt_kwargs)  # apply the k-filter / CAR
+        data[inside_brain, :] = kfilt(
+            data[inside_brain, :], gpu=True, **kfilt_kwargs
+        )  # apply the k-filter / CAR
     else:
         data = kfilt(data, gpu=True, **kfilt_kwargs)  # apply the k-filter / CAR
 
     return data
 
 
 def get_sos(fs, fshigh, fslow=None):
@@ -61,10 +73,10 @@
     Get second-order sections for the butterworth filter
     :param fs: Int, sampling frequency
     :param fshigh: Int, high pass filter frequency
     :param fslow: Int, low pass filter frequency
     :return: sos, second-order sections
     """
     if fslow and fslow < fs / 2:
-        return butter(3, (2 * fshigh / fs, 2 * fslow / fs), 'bandpass', output='sos')
+        return butter(3, (2 * fshigh / fs, 2 * fslow / fs), "bandpass", output="sos")
     else:
-        return butter(3, 2 * fshigh / fs, 'high', output='sos')
+        return butter(3, 2 * fshigh / fs, "high", output="sos")
```

### Comparing `ibl-neuropixel-0.9.2/src/ibldsp/filter_gpu.py` & `ibl_neuropixel-1.0.0/src/ibldsp/filter_gpu.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     :return: Filtered array
     """
 
     sos = cp.asnumpy(sos)
 
     n_sections, m = sos.shape
     if m != 6:
-        raise ValueError('sos array must be shape (n_sections, 6)')
+        raise ValueError("sos array must be shape (n_sections, 6)")
 
     ntaps = 2 * n_sections + 1
     ntaps -= min((sos[:, 2] == 0).sum(), (sos[:, 5] == 0).sum())
 
     x_pad, edge = default_pad(x, axis=axis, ntaps=ntaps)
 
     zi_cpu = sosfilt_zi(sos)  # shape (n_sections, 2) --> (n_sections, ..., 2, ...)
@@ -60,50 +60,50 @@
     :param axis: Axis along which the filter is applied
     :param zi: Initial conditions for the cascaded filter delays.
     :return:
     """
 
     n_sections, m = sos.shape
     if m != 6:
-        raise ValueError('sos array must be shape (n_sections, 6)')
+        raise ValueError("sos array must be shape (n_sections, 6)")
 
     x_zi_shape = list(x.shape)
     x_zi_shape[axis] = 2
     x_zi_shape = tuple([n_sections] + x_zi_shape)
 
     if zi is not None:
-        assert zi.shape == x_zi_shape, f'zi has shape {zi.shape}, expected {x_zi_shape}'
-        zi = cp.array(zi, dtype='float32')
+        assert zi.shape == x_zi_shape, f"zi has shape {zi.shape}, expected {x_zi_shape}"
+        zi = cp.array(zi, dtype="float32")
     else:
-        zi = cp.zeros(x_zi_shape, dtype='float32')
+        zi = cp.zeros(x_zi_shape, dtype="float32")
 
-    sos = cp.array(sos, dtype='float32')
-    assert x.dtype == 'float32', f'Expected float32 data, got {x.dtype}'
+    sos = cp.array(sos, dtype="float32")
+    assert x.dtype == "float32", f"Expected float32 data, got {x.dtype}"
 
     axis = axis % x.ndim
     x = cp.ascontiguousarray(cp.moveaxis(x, axis, -1))
     zi = cp.ascontiguousarray(cp.moveaxis(zi, [0, axis + 1], [-2, -1]))
 
     _cuda_sosfilt(sos, x, zi)
 
     x = cp.moveaxis(x, -1, axis)
 
     return x
 
 
 def _cuda_sosfilt(sos, x, zi):
-
     n_signals, n_samples = x.shape
     n_sections = sos.shape[0]
 
     n_blocks, n_threads = sosfilt_kernel_params(n_signals)
 
-    code, consts = get_cuda('sosfilt', n_signals=n_signals, n_samples=n_samples,
-                            n_sections=n_sections)
-    kernel = cp.RawKernel(code, 'sosfilt')
+    code, consts = get_cuda(
+        "sosfilt", n_signals=n_signals, n_samples=n_samples, n_sections=n_sections
+    )
+    kernel = cp.RawKernel(code, "sosfilt")
     kernel((n_blocks,), (n_threads,), (sos, x, zi))
 
 
 N_THREADS_BLOCK = 1024
 MIN_GPU_BLOCKS = 8
 
 
@@ -148,25 +148,28 @@
     :param n: Padding length, int
     :param axis: Axis to pad
     :return: Padded array
     """
     if n < 1:
         return x
     if n > x.shape[axis] - 1:
-        raise ValueError(("The extension length n (%d) is too big. " +
-                          "It must not exceed x.shape[axis]-1, which is %d.")
-                         % (n, x.shape[axis] - 1))
+        raise ValueError(
+            (
+                "The extension length n (%d) is too big. "
+                + "It must not exceed x.shape[axis]-1, which is %d."
+            )
+            % (n, x.shape[axis] - 1)
+        )
     left_end = axis_slice(x, start=0, stop=1, axis=axis)
     left_ext = axis_slice(x, start=n, stop=0, step=-1, axis=axis)
     right_end = axis_slice(x, start=-1, axis=axis)
     right_ext = axis_slice(x, start=-2, stop=-(n + 2), step=-1, axis=axis)
-    ext = cp.concatenate((2 * left_end - left_ext,
-                          x,
-                          2 * right_end - right_ext),
-                         axis=axis)
+    ext = cp.concatenate(
+        (2 * left_end - left_ext, x, 2 * right_end - right_ext), axis=axis
+    )
     return ext
 
 
 def axis_slice(a, start=None, stop=None, step=None, axis=-1):
     """
     Take slice along array
     """
```

### Comparing `ibl-neuropixel-0.9.2/src/ibldsp/fourier.py` & `ibl_neuropixel-1.0.0/src/ibldsp/fourier.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,24 +15,24 @@
     :param sample_shifts: channel shifts, cupy array with shape (n_channels)
     :return: Aligned data, cupy array with shape (n_channels, n_times)
     """
     import cupy as cp
 
     n_channels, n_times = data.shape
 
-    dephas = cp.tile(- 2 * pi / n_times * cp.arange(n_times), (n_channels, 1))
-    dephas += 2 * pi * (dephas < - pi)  # angles in the range (-pi,pi)
+    dephas = cp.tile(-2 * pi / n_times * cp.arange(n_times), (n_channels, 1))
+    dephas += 2 * pi * (dephas < -pi)  # angles in the range (-pi,pi)
     dephas = cp.exp(1j * dephas * sample_shifts[:, cp.newaxis])
 
     data_shifted = cp.real(cp.fft.ifft(cp.fft.fft(data) * dephas))
 
-    return cp.array(data_shifted, dtype='float32')
+    return cp.array(data_shifted, dtype="float32")
 
 
-def convolve(x, w, mode='full', gpu=False):
+def convolve(x, w, mode="full", gpu=False):
     """
     Frequency domain convolution along the last dimension (2d arrays)
     Will broadcast if a matrix is convolved with a vector
     :param x:
     :param w:
     :param mode:
     :param gpu: bool
@@ -42,21 +42,27 @@
         import cupy as gp
     else:
         gp = np
 
     nsx = x.shape[-1]
     nsw = w.shape[-1]
     ns = ns_optim_fft(nsx + nsw)
-    x_ = gp.concatenate((x, gp.zeros([*x.shape[:-1], ns - nsx], dtype=x.dtype)), axis=-1)
-    w_ = gp.concatenate((w, gp.zeros([*w.shape[:-1], ns - nsw], dtype=w.dtype)), axis=-1)
-    xw = gp.real(gp.fft.irfft(gp.fft.rfft(x_, axis=-1) * gp.fft.rfft(w_, axis=-1), axis=-1))
-    xw = xw[..., :(nsx + nsw)]  # remove 0 padding
-    if mode == 'full':
+    x_ = gp.concatenate(
+        (x, gp.zeros([*x.shape[:-1], ns - nsx], dtype=x.dtype)), axis=-1
+    )
+    w_ = gp.concatenate(
+        (w, gp.zeros([*w.shape[:-1], ns - nsw], dtype=w.dtype)), axis=-1
+    )
+    xw = gp.real(
+        gp.fft.irfft(gp.fft.rfft(x_, axis=-1) * gp.fft.rfft(w_, axis=-1), axis=-1)
+    )
+    xw = xw[..., : (nsx + nsw)]  # remove 0 padding
+    if mode == "full":
         return xw
-    elif mode == 'same':
+    elif mode == "same":
         first = int(gp.floor(nsw / 2)) - ((nsw + 1) % 2)
         last = int(gp.ceil(nsw / 2)) + ((nsw + 1) % 2)
         return xw[..., first:-last]
 
 
 def ns_optim_fft(ns):
     """
@@ -74,15 +80,15 @@
     dephas a signal by a given angle in degrees
     :param w:
     :param phase: phase in degrees
     :param axis:
     :return:
     """
     ns = w.shape[axis]
-    W = freduce(np.fft.fft(w, axis=axis), axis=axis) * np.exp(- 1j * phase / 180 * np.pi)
+    W = freduce(np.fft.fft(w, axis=axis), axis=axis) * np.exp(-1j * phase / 180 * np.pi)
     return np.real(np.fft.ifft(fexpand(W, ns=ns, axis=axis), axis=axis))
 
 
 def fscale(ns, si=1, one_sided=False):
     """
     numpy.fft.fftfreq returns Nyquist as a negative frequency so we propose this instead
 
@@ -138,72 +144,74 @@
 
     :param ts: time serie
     :param si: sampling interval in seconds
     :param b: cutout frequencies: 4 elements vector or list
     :param axis: axis along which to perform reduction (last axis by default)
     :return: filtered time serie
     """
-    return _freq_filter(ts, si, b, axis=axis, typ='bp')
+    return _freq_filter(ts, si, b, axis=axis, typ="bp")
 
 
 def lp(ts, si, b, axis=None):
     """
     Low-pass filter in frequency domain
 
     :param ts: time serie
     :param si: sampling interval in seconds
     :param b: cutout frequencies: 2 elements vector or list
     :param axis: axis along which to perform reduction (last axis by default)
     :return: filtered time serie
     """
-    return _freq_filter(ts, si, b, axis=axis, typ='lp')
+    return _freq_filter(ts, si, b, axis=axis, typ="lp")
 
 
 def hp(ts, si, b, axis=None):
     """
     High-pass filter in frequency domain
 
     :param ts: time serie
     :param si: sampling interval in seconds
     :param b: cutout frequencies: 2 elements vector or list
     :param axis: axis along which to perform reduction (last axis by default)
     :return: filtered time serie
     """
-    return _freq_filter(ts, si, b, axis=axis, typ='hp')
+    return _freq_filter(ts, si, b, axis=axis, typ="hp")
 
 
-def _freq_filter(ts, si, b, axis=None, typ='lp'):
+def _freq_filter(ts, si, b, axis=None, typ="lp"):
     """
-        Wrapper for hp/lp/bp filters
+    Wrapper for hp/lp/bp filters
     """
     if axis is None:
         axis = ts.ndim - 1
     ns = ts.shape[axis]
     f = fscale(ns, si=si, one_sided=True)
-    if typ == 'bp':
-        filc = _freq_vector(f, b[0:2], typ='hp') * _freq_vector(f, b[2:4], typ='lp')
+    if typ == "bp":
+        filc = _freq_vector(f, b[0:2], typ="hp") * _freq_vector(f, b[2:4], typ="lp")
     else:
         filc = _freq_vector(f, b, typ=typ)
     if axis < (ts.ndim - 1):
         filc = filc[:, np.newaxis]
-    return np.real(np.fft.ifft(np.fft.fft(ts, axis=axis) * fexpand(filc, ns, axis=0), axis=axis))
+    return np.real(
+        np.fft.ifft(np.fft.fft(ts, axis=axis) * fexpand(filc, ns, axis=0), axis=axis)
+    )
 
 
-def _freq_vector(f, b, typ='lp'):
+def _freq_vector(f, b, typ="lp"):
     """
-        Returns a frequency modulated vector for filtering
+    Returns a frequency modulated vector for filtering
 
-        :param f: frequency vector, uniform and monotonic
-        :param b: 2 bounds array
-        :return: amplitude modulated frequency vector
+    :param f: frequency vector, uniform and monotonic
+    :param b: 2 bounds array
+    :return: amplitude modulated frequency vector
     """
     filc = fcn_cosine(b)(f)
-    if typ.lower() in ['hp', 'highpass']:
+    if typ.lower() in ["hp", "highpass"]:
         return filc
-    elif typ.lower() in ['lp', 'lowpass']:
+    elif typ.lower() in ["lp", "lowpass"]:
         return 1 - filc
 
 
 def fshift(w, s, axis=-1, ns=None):
     """
     Shifts a 1D or 2D signal in frequency domain, to allow for accurate non-integer shifts
     :param w: input signal (if complex, need to provide ns too)
@@ -252,16 +260,21 @@
     """
     if fmax is None:
         fmax = 1 / si / 2
     ns = w.shape[axis]
     freqs = freduce(fscale(ns, si=si))
     phi = np.unwrap(np.angle(freduce(np.fft.fft(w, axis=axis), axis=axis)))
     indf = np.logical_and(fmin < freqs, freqs < fmax)
-    dt = - np.polyfit(freqs[indf],
-                      np.swapaxes(phi.compress(indf, axis=axis), axis, 0), 1)[0] / np.pi / 2
+    dt = (
+        -np.polyfit(
+            freqs[indf], np.swapaxes(phi.compress(indf, axis=axis), axis, 0), 1
+        )[0]
+        / np.pi
+        / 2
+    )
     return dt
 
 
 def dft(x, xscale=None, axis=-1, kscale=None):
     """
     1D discrete fourier transform. Vectorized.
     :param x: 1D numpy array to be transformed
@@ -280,15 +293,15 @@
         nk = kscale.size
     if axis != 0:
         # the axis of the transform always needs to be the first
         x = np.swapaxes(x, axis, 0)
     shape = np.array(x.shape)
     x = np.reshape(x, (ns, int(np.prod(x.shape) / ns)))
     # compute fourier coefficients
-    exp = np.exp(- 1j * 2 * np.pi / ns * xscale * kscale[:, np.newaxis])
+    exp = np.exp(-1j * 2 * np.pi / ns * xscale * kscale[:, np.newaxis])
     X = np.matmul(exp, x)
     shape[0] = int(nk)
     X = X.reshape(shape)
     if axis != 0:
         X = np.swapaxes(X, axis, 0)
     return X
 
@@ -302,12 +315,18 @@
     :param nk: output size along axis 0
     :param nl: output size along axis 1
     :return: Matrix X (nk, nl, nt)
     """
     # it would be interesting to compare performance with numba straight loops (easier to write)
     # GPU/C implementation should implement straight loops
     nt = x.shape[-1]
-    k, h = [v.flatten() for v in np.meshgrid(np.arange(nk), np.arange(nl), indexing='ij')]
+    k, h = [
+        v.flatten() for v in np.meshgrid(np.arange(nk), np.arange(nl), indexing="ij")
+    ]
     # exp has dimension (kh, rc)
-    exp = np.exp(- 1j * 2 * np.pi * (r[np.newaxis] * k[:, np.newaxis] +
-                                     c[np.newaxis] * h[:, np.newaxis]))
+    exp = np.exp(
+        -1j
+        * 2
+        * np.pi
+        * (r[np.newaxis] * k[:, np.newaxis] + c[np.newaxis] * h[:, np.newaxis])
+    )
     return np.matmul(exp, x).reshape((nk, nl, nt))
```

### Comparing `ibl-neuropixel-0.9.2/src/ibldsp/raw_metrics.py` & `ibl_neuropixel-1.0.0/src/ibldsp/raw_metrics.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.9.2/src/ibldsp/smooth.py` & `ibl_neuropixel-1.0.0/src/ibldsp/smooth.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,20 +13,20 @@
     :param fac: 2 element vector of the frequency edges relative to Nyquist: [0.15, 0.2] keeps
     everything up to 15% of the full band tapering down to 20%
     :param pad: padding on the edges of the time serie, between 0 and 1 (0.2 means 20% of the size)
     :return: smoothed time series
     """
     # keep at least two periods for the padding
     lpad = int(np.ceil(ts.shape[0] * pad))
-    ts_ = np.pad(ts, lpad, mode='edge')
+    ts_ = np.pad(ts, lpad, mode="edge")
     ts_ = ft.lp(ts_, 1, np.array(fac) / 2)
     return ts_[lpad:-lpad]
 
 
-def rolling_window(x, window_len=11, window='blackman'):
+def rolling_window(x, window_len=11, window="blackman"):
     """
     Smooth the data using a window with requested size.
 
     This method is based on the convolution of a scaled window with the signal.
     The signal is prepared by introducing reflected copies of the signal
     (with the window size) in both ends so that transient parts are minimized
     in the beginning and end part of the output signal.
@@ -58,27 +58,29 @@
 
     if x.size < window_len:
         raise ValueError("Input vector needs to be bigger than window size.")
 
     if window_len < 3:
         return x
 
-    if window not in ['flat', 'hanning', 'hamming', 'bartlett', 'blackman']:
-        raise ValueError("Window is not one of 'flat', 'hanning', 'hamming',\
-'bartlett', 'blackman'")
+    if window not in ["flat", "hanning", "hamming", "bartlett", "blackman"]:
+        raise ValueError(
+            "Window is not one of 'flat', 'hanning', 'hamming',\
+'bartlett', 'blackman'"
+        )
 
-    s = np.r_[x[window_len - 1:0:-1], x, x[-1:-window_len:-1]]
+    s = np.r_[x[window_len - 1: 0: -1], x, x[-1:-window_len:-1]]
     # print(len(s))
-    if window == 'flat':  # moving average
-        w = np.ones(window_len, 'd')
+    if window == "flat":  # moving average
+        w = np.ones(window_len, "d")
     else:
-        w = eval('np.' + window + '(window_len)')
+        w = eval("np." + window + "(window_len)")
 
-    y = np.convolve(w / w.sum(), s, mode='valid')
-    return y[round((window_len / 2 - 1)):round(-(window_len / 2))]
+    y = np.convolve(w / w.sum(), s, mode="valid")
+    return y[round((window_len / 2 - 1)): round(-(window_len / 2))]
 
 
 def non_uniform_savgol(x, y, window, polynom):
     """Applies a Savitzky-Golay filter to y with non-uniform spacing as defined in x.
     This is based on
     https://dsp.stackexchange.com/questions/1676/savitzky-golay-smoothing-filter-for-not-equally-spaced-data
     The borders are interpolated like scipy.signal.savgol_filter would do
@@ -98,15 +100,15 @@
     np.array
         The smoothed y values
     """
 
     if len(x) != len(y):
         raise ValueError('"x" and "y" must be of the same size')
     if len(x) < window:
-        raise ValueError('The data size must be larger than the window size')
+        raise ValueError("The data size must be larger than the window size")
     if type(window) is not int:
         raise TypeError('"window" must be an integer')
     if window % 2 == 0:
         raise ValueError('The "window" must be an odd integer')
     if type(polynom) is not int:
         raise TypeError('"polynom" must be an integer')
     if polynom >= window:
@@ -173,15 +175,15 @@
         for j in range(0, polynom, 1):
             y_smoothed[i] += last_coeffs[j] * x_i
             x_i *= x[i] - x[-half_window - 1]
 
     return y_smoothed
 
 
-def smooth_interpolate_savgol(signal, window=31, order=3, interp_kind='cubic'):
+def smooth_interpolate_savgol(signal, window=31, order=3, interp_kind="cubic"):
     """Run savitzy-golay filter on signal, interpolate through nan points.
 
     Parameters
     ----------
     signal : np.ndarray
         original noisy signal of shape (t,), may contain nans
     window : int
@@ -197,16 +199,24 @@
     """
 
     signal_noisy_w_nans = np.copy(signal)
     timestamps = np.arange(signal_noisy_w_nans.shape[0])
     good_idxs = np.where(~np.isnan(signal_noisy_w_nans))[0]
     # perform savitzky-golay filtering on non-nan points
     signal_smooth_nonans = non_uniform_savgol(
-        timestamps[good_idxs], signal_noisy_w_nans[good_idxs], window=window, polynom=order)
+        timestamps[good_idxs],
+        signal_noisy_w_nans[good_idxs],
+        window=window,
+        polynom=order,
+    )
     signal_smooth_w_nans = np.copy(signal_noisy_w_nans)
     signal_smooth_w_nans[good_idxs] = signal_smooth_nonans
     # interpolate nan points
     interpolater = interp1d(
-        timestamps[good_idxs], signal_smooth_nonans, kind=interp_kind, fill_value='extrapolate')
+        timestamps[good_idxs],
+        signal_smooth_nonans,
+        kind=interp_kind,
+        fill_value="extrapolate",
+    )
     signal = interpolater(timestamps)
 
     return signal
```

### Comparing `ibl-neuropixel-0.9.2/src/ibldsp/spiketrains.py` & `ibl_neuropixel-1.0.0/src/ibldsp/spiketrains.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.9.2/src/ibldsp/utils.py` & `ibl_neuropixel-1.0.0/src/ibldsp/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,27 +18,33 @@
      float: drift in ppm
      numpy array: of indices ia
      numpy array: of indices ib
     """
 
     def _interp_fcn(tsa, tsb, ib):
         # now compute the bpod/fpga drift and precise time shift
-        drift_ppm = np.polyfit(tsa[ib >= 0], tsb[ib[ib >= 0]] - tsa[ib >= 0], 1)[0] * 1e6
-        fcn_a2b = scipy.interpolate.interp1d(tsa[ib >= 0], tsb[ib[ib >= 0]], fill_value="extrapolate")
+        drift_ppm = (
+            np.polyfit(tsa[ib >= 0], tsb[ib[ib >= 0]] - tsa[ib >= 0], 1)[0] * 1e6
+        )
+        fcn_a2b = scipy.interpolate.interp1d(
+            tsa[ib >= 0], tsb[ib[ib >= 0]], fill_value="extrapolate"
+        )
         return fcn_a2b, drift_ppm
 
     # assert sorted inputs
     tmin = np.min([np.min(tsa), np.min(tsb)])
     tmax = np.max([np.max(tsa), np.max(tsb)])
     # brute force correlation to get an estimate of the delta_t between series
     x = np.zeros(int(np.ceil(tmax - tmin) / tbin))
     y = np.zeros_like(x)
     x[np.int32(np.floor((tsa - tmin) / tbin))] = 1
     y[np.int32(np.floor((tsb - tmin) / tbin))] = 1
-    delta_t = (parabolic_max(scipy.signal.correlate(x, y, mode='full'))[0] - x.shape[0] + 1) * tbin
+    delta_t = (
+        parabolic_max(scipy.signal.correlate(x, y, mode="full"))[0] - x.shape[0] + 1
+    ) * tbin
     # do a first assignment at a DT threshold
     ib = np.zeros(tsa.shape, dtype=np.int32) - 1
     threshold = tbin
     for m in np.arange(tsa.shape[0]):
         dt = np.abs(tsa[m] - delta_t - tsb)
         inds = np.where(dt < threshold)[0]
         if inds.size == 1:
@@ -81,20 +87,24 @@
     axis = -1
     imax = np.argmax(x, axis=axis)
 
     if x.ndim == 1:
         v010 = x[np.maximum(np.minimum(imax + np.array([-1, 0, 1]), ns - 1), 0)]
         v010 = v010[:, np.newaxis]
     else:
-        v010 = np.vstack((x[..., np.arange(x.shape[0]), np.maximum(imax - 1, 0)],
-                          x[..., np.arange(x.shape[0]), imax],
-                          x[..., np.arange(x.shape[0]), np.minimum(imax + 1, ns - 1)]))
-    poly = np.matmul(.5 * np.array([[1, -2, 1], [-1, 0, 1], [0, 2, 0]]), v010)
-    ipeak = - poly[1] / (poly[0] + np.double(poly[0] == 0)) / 2
-    maxi = poly[2] + ipeak * poly[1] + ipeak ** 2. * poly[0]
+        v010 = np.vstack(
+            (
+                x[..., np.arange(x.shape[0]), np.maximum(imax - 1, 0)],
+                x[..., np.arange(x.shape[0]), imax],
+                x[..., np.arange(x.shape[0]), np.minimum(imax + 1, ns - 1)],
+            )
+        )
+    poly = np.matmul(0.5 * np.array([[1, -2, 1], [-1, 0, 1], [0, 2, 0]]), v010)
+    ipeak = -poly[1] / (poly[0] + np.double(poly[0] == 0)) / 2
+    maxi = poly[2] + ipeak * poly[1] + ipeak**2.0 * poly[0]
     ipeak += imax
     # handle edges
     iedges = np.logical_or(imax == 0, imax == ns - 1)
     if x.ndim == 1:
         maxi = v010[1, 0] if iedges else maxi[0]
         ipeak = imax if iedges else ipeak[0]
     else:
@@ -129,14 +139,15 @@
     if gpu:
         import cupy as gp
     else:
         gp = np
 
     def _cos(x):
         return (1 - gp.cos((x - bounds[0]) / (bounds[1] - bounds[0]) * gp.pi)) / 2
+
     func = lambda x: _fcn_extrap(x, _cos, bounds)  # noqa
     return func
 
 
 def fronts(x, axis=-1, step=1):
     """
     Detects Rising and Falling edges of a voltage signal, returns indices and
@@ -196,26 +207,53 @@
     """
     Root mean square of array along axis
 
     :param x: array on which to compute RMS
     :param axis: (optional, -1)
     :return: numpy array
     """
-    return np.sqrt(np.mean(x ** 2, axis=axis))
+    return np.sqrt(np.mean(x**2, axis=axis))
+
+
+def make_channel_index(geom, radius=200.0, pad_val=384):
+    """
+    Given a neuropixels geometry dict `geom`, returns an array with nc rows
+    where the i'th row contains the channel ids that fall within `radius` um
+    of channel i. The number of columns is the maximum number of neighbors a
+    channel can have and will depend on the geometry and the radius chosen.
+
+    For channels at the edges of the probe which have less than the maximum possible
+    number of neighbors, the remaining indices in the row are filled with `pad_val`.
+    """
+    neighbors = (
+        scipy.spatial.distance.squareform(scipy.spatial.distance.pdist(geom)) <= radius
+    )
+    n_nbors = np.max(np.sum(neighbors, 0))
+
+    nc = geom.shape[0]
+    if pad_val is None:
+        pad_val = nc
+    channel_idx = np.full((nc, n_nbors), pad_val, dtype=int)
+    for c in range(nc):
+        ch_idx = np.flatnonzero(neighbors[c, :])
+        channel_idx[c, : ch_idx.shape[0]] = ch_idx
+
+    return channel_idx
 
 
 class WindowGenerator(object):
     """
     `wg = WindowGenerator(ns, nswin, overlap)`
 
     Provide sliding windows indices generator for signal processing applications.
     For straightforward spectrogram / periodogram implementation, prefer scipy methods !
 
     Example of implementations in test_dsp.py.
     """
+
     def __init__(self, ns, nswin, overlap):
         """
         :param ns: number of sample of the signal along the direction to be windowed
         :param nswin: number of samples of the window
         :return: dsp.WindowGenerator object:
         """
         self.ns = int(ns)
@@ -266,8 +304,10 @@
 
     def tscale(self, fs):
         """
         Returns the time scale associated with Window slicing (middle of window)
         :param fs: sampling frequency (Hz)
         :return: time axis scale
         """
-        return np.array([(first + (last - first - 1) / 2) / fs for first, last in self.firstlast])
+        return np.array(
+            [(first + (last - first - 1) / 2) / fs for first, last in self.firstlast]
+        )
```

### Comparing `ibl-neuropixel-0.9.2/src/ibldsp/voltage.py` & `ibl_neuropixel-1.0.0/src/ibldsp/voltage.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import spikeglx
 import neuropixel
 
 import ibldsp.fourier as fourier
 import ibldsp.utils as utils
 
 
-def agc(x, wl=.5, si=.002, epsilon=1e-8, gpu=False):
+def agc(x, wl=0.5, si=0.002, epsilon=1e-8, gpu=False):
     """
     Automatic gain control
     w_agc, gain = agc(w, wl=.5, si=.002, epsilon=1e-8)
     such as w_agc * gain = w
     :param x: seismic array (sample last dimension)
     :param wl: window length (secs)
     :param si: sampling interval (secs)
@@ -32,26 +32,36 @@
     if gpu:
         import cupy as gp
     else:
         gp = np
     ns_win = int(gp.round(wl / si / 2) * 2 + 1)
     w = gp.hanning(ns_win)
     w /= gp.sum(w)
-    gain = fourier.convolve(gp.abs(x), w, mode='same', gpu=gpu)
+    gain = fourier.convolve(gp.abs(x), w, mode="same", gpu=gpu)
     gain += (gp.sum(gain, axis=1) * epsilon / x.shape[-1])[:, gp.newaxis]
     dead_channels = np.sum(gain, axis=1) == 0
     x[~dead_channels, :] = x[~dead_channels, :] / gain[~dead_channels, :]
     if gpu:
-        return (x * gain).astype('float32'), gain.astype('float32')
+        return (x * gain).astype("float32"), gain.astype("float32")
 
     return x, gain
 
 
-def fk(x, si=.002, dx=1, vbounds=None, btype='highpass', ntr_pad=0, ntr_tap=None, lagc=.5,
-       collection=None, kfilt=None):
+def fk(
+    x,
+    si=0.002,
+    dx=1,
+    vbounds=None,
+    btype="highpass",
+    ntr_pad=0,
+    ntr_tap=None,
+    lagc=0.5,
+    collection=None,
+    kfilt=None,
+):
     """Frequency-wavenumber filter: filters apparent plane-waves velocity
     :param x: the input array to be filtered. dimension, the filtering is considering
     axis=0: spatial dimension, axis=1 temporal dimension. (ntraces, ns)
     :param si: sampling interval (secs)
     :param dx: spatial interval (usually meters)
     :param vbounds: velocity high pass [v1, v2], cosine taper from 0 to 1 between v1 and v2
     :param btype: {‘lowpass’, ‘highpass’}, velocity filter : defaults to highpass
@@ -64,16 +74,24 @@
     on which the FK filter will run separately (shot gaters, receiver gathers)
     :return:
     """
     if collection is not None:
         xout = np.zeros_like(x)
         for c in np.unique(collection):
             sel = collection == c
-            xout[sel, :] = fk(x[sel, :], si=si, dx=dx, vbounds=vbounds, ntr_pad=ntr_pad,
-                              ntr_tap=ntr_tap, lagc=lagc, collection=None)
+            xout[sel, :] = fk(
+                x[sel, :],
+                si=si,
+                dx=dx,
+                vbounds=vbounds,
+                ntr_pad=ntr_pad,
+                ntr_tap=ntr_tap,
+                lagc=lagc,
+                collection=None,
+            )
         return xout
 
     assert vbounds
     nx, nt = x.shape
 
     # lateral padding left and right
     ntr_pad = int(ntr_pad)
@@ -81,22 +99,22 @@
     nxp = nx + ntr_pad * 2
 
     # compute frequency wavenumber scales and deduce the velocity filter
     fscale = fourier.fscale(nt, si)
     kscale = fourier.fscale(nxp, dx)
     kscale[0] = 1e-6
     v = fscale[np.newaxis, :] / kscale[:, np.newaxis]
-    if btype.lower() in ['highpass', 'hp']:
+    if btype.lower() in ["highpass", "hp"]:
         fk_att = fourier.fcn_cosine(vbounds)(np.abs(v))
-    elif btype.lower() in ['lowpass', 'lp']:
-        fk_att = (1 - fourier.fcn_cosine(vbounds)(np.abs(v)))
+    elif btype.lower() in ["lowpass", "lp"]:
+        fk_att = 1 - fourier.fcn_cosine(vbounds)(np.abs(v))
 
     # if a k-filter is also provided, apply it
     if kfilt is not None:
-        katt = fourier._freq_vector(np.abs(kscale), kfilt['bounds'], typ=kfilt['btype'])
+        katt = fourier._freq_vector(np.abs(kscale), kfilt["bounds"], typ=kfilt["btype"])
         fk_att *= katt[:, np.newaxis]
 
     # import matplotlib.pyplot as plt
     # plt.imshow(np.fft.fftshift(np.abs(v), axes=0).T, aspect='auto', vmin=0, vmax=1e5,
     #            extent=[np.min(kscale), np.max(kscale), 0, np.max(fscale) * 2])
     # plt.imshow(np.fft.fftshift(np.abs(fk_att), axes=0).T, aspect='auto', vmin=0, vmax=1,
     #            extent=[np.min(kscale), np.max(kscale), 0, np.max(fscale) * 2])
@@ -108,15 +126,17 @@
     else:
         xf, gain = agc(x, wl=lagc, si=si)
     if ntr_pad > 0:
         # pad the array with a mirrored version of itself and apply a cosine taper
         xf = np.r_[np.flipud(xf[:ntr_pad]), xf, np.flipud(xf[-ntr_pad:])]
     if ntr_tap > 0:
         taper = fourier.fcn_cosine([0, ntr_tap])(np.arange(nxp))  # taper up
-        taper *= 1 - fourier.fcn_cosine([nxp - ntr_tap, nxp])(np.arange(nxp))   # taper down
+        taper *= 1 - fourier.fcn_cosine([nxp - ntr_tap, nxp])(
+            np.arange(nxp)
+        )  # taper down
         xf = xf * taper[:, np.newaxis]
     xf = np.real(np.fft.ifft2(fk_att * np.fft.fft2(xf)))
 
     if ntr_pad > 0:
         xf = xf[ntr_pad:-ntr_pad, :]
     return xf * gain
 
@@ -128,35 +148,42 @@
     axis=0: spatial dimension, axis=1 temporal dimension. (ntraces, ns)
     :param collection:
     :param lagc: window size for time domain automatic gain control (no agc otherwise)
     :param butter_kwargs: filtering parameters: defaults: {'N': 3, 'Wn': 0.1, 'btype': 'highpass'}
     :return:
     """
     if butter_kwargs is None:
-        butter_kwargs = {'N': 3, 'Wn': 0.1, 'btype': 'highpass'}
+        butter_kwargs = {"N": 3, "Wn": 0.1, "btype": "highpass"}
     if collection is not None:
         xout = np.zeros_like(x)
         for c in np.unique(collection):
             sel = collection == c
-            xout[sel, :] = kfilt(x=x[sel, :], ntr_pad=0, ntr_tap=None, collection=None,
-                                 butter_kwargs=butter_kwargs)
+            xout[sel, :] = kfilt(
+                x=x[sel, :],
+                ntr_pad=0,
+                ntr_tap=None,
+                collection=None,
+                butter_kwargs=butter_kwargs,
+            )
         return xout
 
     # apply agc and keep the gain in handy
     if not lagc:
         xf = np.copy(x)
         gain = 1
     else:
         xf, gain = agc(x, wl=lagc, si=1.0)
     # apply CAR and then un-apply the gain
     xf = xf - np.median(xf, axis=0)
     return xf * gain
 
 
-def kfilt(x, collection=None, ntr_pad=0, ntr_tap=None, lagc=300, butter_kwargs=None, gpu=False):
+def kfilt(
+    x, collection=None, ntr_pad=0, ntr_tap=None, lagc=300, butter_kwargs=None, gpu=False
+):
     """
     Applies a butterworth filter on the 0-axis with tapering / padding
     :param x: the input array to be filtered. dimension, the filtering is considering
     axis=0: spatial dimension, axis=1 temporal dimension. (ntraces, ns)
     :param collection:
     :param ntr_pad: traces added to each side (mirrored)
     :param ntr_tap: n traces for apodizatin on each side
@@ -167,21 +194,26 @@
     """
     if gpu:
         import cupy as gp
     else:
         gp = np
 
     if butter_kwargs is None:
-        butter_kwargs = {'N': 3, 'Wn': 0.1, 'btype': 'highpass'}
+        butter_kwargs = {"N": 3, "Wn": 0.1, "btype": "highpass"}
     if collection is not None:
         xout = gp.zeros_like(x)
         for c in gp.unique(collection):
             sel = collection == c
-            xout[sel, :] = kfilt(x=x[sel, :], ntr_pad=0, ntr_tap=None, collection=None,
-                                 butter_kwargs=butter_kwargs)
+            xout[sel, :] = kfilt(
+                x=x[sel, :],
+                ntr_pad=0,
+                ntr_tap=None,
+                collection=None,
+                butter_kwargs=butter_kwargs,
+            )
         return xout
     nx, nt = x.shape
 
     # lateral padding left and right
     ntr_pad = int(ntr_pad)
     ntr_tap = ntr_pad if ntr_tap is None else ntr_tap
     nxp = nx + ntr_pad * 2
@@ -193,29 +225,61 @@
     else:
         xf, gain = agc(x, wl=lagc, si=1.0, gpu=gpu)
     if ntr_pad > 0:
         # pad the array with a mirrored version of itself and apply a cosine taper
         xf = gp.r_[gp.flipud(xf[:ntr_pad]), xf, gp.flipud(xf[-ntr_pad:])]
     if ntr_tap > 0:
         taper = fourier.fcn_cosine([0, ntr_tap], gpu=gpu)(gp.arange(nxp))  # taper up
-        taper *= 1 - fourier.fcn_cosine([nxp - ntr_tap, nxp], gpu=gpu)(gp.arange(nxp))   # taper down
+        taper *= 1 - fourier.fcn_cosine([nxp - ntr_tap, nxp], gpu=gpu)(
+            gp.arange(nxp)
+        )  # taper down
         xf = xf * taper[:, gp.newaxis]
-    sos = scipy.signal.butter(**butter_kwargs, output='sos')
+    sos = scipy.signal.butter(**butter_kwargs, output="sos")
     if gpu:
         from .filter_gpu import sosfiltfilt_gpu
+
         xf = sosfiltfilt_gpu(sos, xf, axis=0)
     else:
         xf = scipy.signal.sosfiltfilt(sos, xf, axis=0)
 
     if ntr_pad > 0:
         xf = xf[ntr_pad:-ntr_pad, :]
     return xf * gain
 
 
-def interpolate_bad_channels(data, channel_labels=None, x=None, y=None, p=1.3, kriging_distance_um=20, gpu=False):
+def saturation(data, max_voltage, v_per_sec=1e-8, fs=30_000, proportion=0.2, mute_window_samples=7):
+    """
+    Computes
+    :param data: [nc, ns]: voltage traces array
+    :param max_voltage: maximum value of the voltage: scalar or array of size nc (same units as data)
+    :param v_per_sec: maximum derivative of the voltage in V/s (or units/s)
+    :param fs: sampling frequency Hz (defaults to 30kHz)
+    :param proportion: 0 < proportion <1  of channels above threshold to consider the sample as saturated (0.2)
+    :param mute_window_samples=7: number of samples for the cosine taper applied to the saturation
+    :return:
+        saturation [ns]: boolean array indicating the saturated samples
+        mute [ns]: float array indicating the mute function to apply to the data [0-1]
+    """
+    # first computes the saturated samples
+    max_voltage = np.atleast_1d(max_voltage)[:, np.newaxis]
+    saturation = np.mean(np.abs(data) > max_voltage * 0.98, axis=0)
+    # then compute the derivative of the voltage saturation
+    n_diff_saturated = np.mean(np.abs(np.diff(data, axis=-1)) / fs >= v_per_sec, axis=0)
+    n_diff_saturated = np.r_[n_diff_saturated, 0]
+    # if either of those reaches more than the proportion of channels labels the sample as saturated
+    saturation = np.logical_or(saturation > proportion, n_diff_saturated > proportion)
+    # apply a cosine taper to the saturation to create a mute function
+    win = scipy.signal.windows.cosine(mute_window_samples)
+    mute = np.maximum(0, 1 - scipy.signal.convolve(saturation, win, mode='same'))
+    return saturation, mute
+
+
+def interpolate_bad_channels(
+    data, channel_labels=None, x=None, y=None, p=1.3, kriging_distance_um=20, gpu=False
+):
     """
     Interpolate the channel labeled as bad channels using linear interpolation.
     The weights applied to neighbouring channels come from an exponential decay function
     :param data: (nc, ns) np.ndarray
     :param channel_labels; (nc) np.ndarray: 0: channel is good, 1: dead, 2:noisy, 3: out of the brain
     :param x: channel x-coordinates, np.ndarray
     :param y: channel y-coordinates, np.ndarray
@@ -233,15 +297,15 @@
     # ephys_bad_channels(x, 30000, channel_labels[0], channel_labels[1])
 
     # we interpolate only noisy channels or dead channels (0: good), out of the brain channels are left
     bad_channels = gp.where(np.logical_or(channel_labels == 1, channel_labels == 2))[0]
     for i in bad_channels:
         # compute the weights to apply to neighbouring traces
         offset = gp.abs(x - x[i] + 1j * (y - y[i]))
-        weights = gp.exp(-(offset / kriging_distance_um) ** p)
+        weights = gp.exp(-((offset / kriging_distance_um) ** p))
         weights[bad_channels] = 0
         weights[weights < 0.005] = 0
         weights = weights / gp.sum(weights)
         imult = gp.where(weights > 0.005)[0]
         if imult.size == 0:
             data[i, :] = 0
             continue
@@ -251,27 +315,40 @@
     return data
 
 
 def _get_destripe_parameters(fs, butter_kwargs, k_kwargs, k_filter):
     """gets the default params for destripe. This is used for both the destripe fcn on a
     numpy array and the function that actuates on a cbin file"""
     if butter_kwargs is None:
-        butter_kwargs = {'N': 3, 'Wn': 300 / fs * 2, 'btype': 'highpass'}
+        butter_kwargs = {"N": 3, "Wn": 300 / fs * 2, "btype": "highpass"}
     if k_kwargs is None:
         lagc = None if fs < 3000 else int(fs / 10)
-        k_kwargs = {'ntr_pad': 60, 'ntr_tap': 0, 'lagc': lagc,
-                    'butter_kwargs': {'N': 3, 'Wn': 0.01, 'btype': 'highpass'}}
+        k_kwargs = {
+            "ntr_pad": 60,
+            "ntr_tap": 0,
+            "lagc": lagc,
+            "butter_kwargs": {"N": 3, "Wn": 0.01, "btype": "highpass"},
+        }
     if k_filter:
         spatial_fcn = lambda dat: kfilt(dat, **k_kwargs)  # noqa
     else:
         spatial_fcn = lambda dat: car(dat, **k_kwargs)  # noqa
     return butter_kwargs, k_kwargs, spatial_fcn
 
 
-def destripe(x, fs, h=None, neuropixel_version=1, butter_kwargs=None, k_kwargs=None, channel_labels=None, k_filter=True):
+def destripe(
+    x,
+    fs,
+    h=None,
+    neuropixel_version=1,
+    butter_kwargs=None,
+    k_kwargs=None,
+    channel_labels=None,
+    k_filter=True,
+):
     """Super Car (super slow also...) - far from being set in stone but a good workflow example
     :param x: demultiplexed array (nc, ns)
     :param fs: sampling frequency
     :param neuropixel_version (optional): 1 or 2. Useful for the ADC shift correction. If None,
      no correction is applied
     :param channel_labels:
       None: (default) keep all channels
@@ -284,29 +361,31 @@
        True: deduces the bad channels from the data provided
     :param butter_kwargs: (optional, None) butterworth params, see the code for the defaults dict
     :param k_kwargs: (optional, None) K-filter params, see the code for the defaults dict
         can also be set to 'car', in which case the median accross channels will be subtracted
     :param k_filter (True): applies k-filter by default, otherwise, apply CAR.
     :return: x, filtered array
     """
-    butter_kwargs, k_kwargs, spatial_fcn = _get_destripe_parameters(fs, butter_kwargs, k_kwargs, k_filter)
+    butter_kwargs, k_kwargs, spatial_fcn = _get_destripe_parameters(
+        fs, butter_kwargs, k_kwargs, k_filter
+    )
     if h is None:
         h = neuropixel.trace_header(version=neuropixel_version)
     if channel_labels is True:
         channel_labels, _ = detect_bad_channels(x, fs)
     # butterworth
-    sos = scipy.signal.butter(**butter_kwargs, output='sos')
+    sos = scipy.signal.butter(**butter_kwargs, output="sos")
     x = scipy.signal.sosfiltfilt(sos, x)
     # channel interpolation
     # apply ADC shift
     if neuropixel_version is not None:
-        x = fourier.fshift(x, h['sample_shift'], axis=1)
+        x = fourier.fshift(x, h["sample_shift"], axis=1)
     # apply spatial filter only on channels that are inside of the brain
     if channel_labels is not None:
-        x = interpolate_bad_channels(x, channel_labels, h['x'], h['y'])
+        x = interpolate_bad_channels(x, channel_labels, h["x"], h["y"])
         inside_brain = np.where(channel_labels != 3)[0]
         x[inside_brain, :] = spatial_fcn(x[inside_brain, :])  # apply the k-filter
     else:
         x = spatial_fcn(x)
     return x
 
 
@@ -314,24 +393,42 @@
     """
     Wrapper around the destipe function with some default parameters to destripe the LFP band
     See help destripe function for documentation
     :param x:
     :param fs:
     :return:
     """
-    kwargs['butter_kwargs'] = {'N': 3, 'Wn': 2 / fs * 2, 'btype': 'highpass'}
-    kwargs['k_filter'] = False
+    kwargs["butter_kwargs"] = {"N": 3, "Wn": 2 / fs * 2, "btype": "highpass"}
+    kwargs["k_filter"] = False
     if channel_labels is True:
-        kwargs['channel_labels'], _ = detect_bad_channels(x, fs=fs, psd_hf_threshold=1.4)
+        kwargs["channel_labels"], _ = detect_bad_channels(
+            x, fs=fs, psd_hf_threshold=1.4
+        )
     return destripe(x, fs, **kwargs)
 
 
-def decompress_destripe_cbin(sr_file, output_file=None, h=None, wrot=None, append=False, nc_out=None, butter_kwargs=None,
-                             dtype=np.int16, ns2add=0, nbatch=None, nprocesses=None, compute_rms=True, reject_channels=True,
-                             k_kwargs=None, k_filter=True, reader_kwargs=None, output_qc_path=None):
+def decompress_destripe_cbin(
+    sr_file,
+    output_file=None,
+    h=None,
+    wrot=None,
+    append=False,
+    nc_out=None,
+    butter_kwargs=None,
+    dtype=np.int16,
+    ns2add=0,
+    nbatch=None,
+    nprocesses=None,
+    compute_rms=True,
+    reject_channels=True,
+    k_kwargs=None,
+    k_filter=True,
+    reader_kwargs=None,
+    output_qc_path=None,
+):
     """
     From a spikeglx Reader object, decompresses and apply ADC.
     Saves output as a flat binary file in int16
     Production version with optimized FFTs - requires pyfftw
     :param sr: seismic reader object (spikeglx.Reader)
     :param output_file: (optional, defaults to .bin extension of the compressed bin file)
     :param h: (optional) neuropixel trace header. Dictionary with key 'sample_shift'
@@ -359,124 +456,141 @@
     NBATCH = nbatch or 65536
     # handles input parameters
     reader_kwargs = {} if reader_kwargs is None else reader_kwargs
     sr = spikeglx.Reader(sr_file, open=True, **reader_kwargs)
     if reject_channels:  # get bad channels if option is on
         channel_labels = detect_bad_channels_cbin(sr)
     assert isinstance(sr_file, str) or isinstance(sr_file, Path)
-    butter_kwargs, k_kwargs, spatial_fcn = _get_destripe_parameters(sr.fs, butter_kwargs, k_kwargs, k_filter)
+    butter_kwargs, k_kwargs, spatial_fcn = _get_destripe_parameters(
+        sr.fs, butter_kwargs, k_kwargs, k_filter
+    )
     h = sr.geometry if h is None else h
-    ncv = h['sample_shift'].size  # number of channels
-    output_file = sr.file_bin.with_suffix('.bin') if output_file is None else Path(output_file)
+    ncv = h["sample_shift"].size  # number of channels
+    output_file = (
+        sr.file_bin.with_suffix(".bin") if output_file is None else Path(output_file)
+    )
     assert output_file != sr.file_bin
     taper = np.r_[0, scipy.signal.windows.cosine((SAMPLES_TAPER - 1) * 2), 0]
     # create the FFT stencils
     nc_out = nc_out or sr.nc
     # compute LP filter coefficients
-    sos = scipy.signal.butter(**butter_kwargs, output='sos')
+    sos = scipy.signal.butter(**butter_kwargs, output="sos")
     nbytes = dtype(1).nbytes
     nprocesses = nprocesses or int(cpu_count() - cpu_count() / 4)
-    win = pyfftw.empty_aligned((ncv, NBATCH), dtype='float32')
-    WIN = pyfftw.empty_aligned((ncv, int(NBATCH / 2 + 1)), dtype='complex64')
-    fft_object = pyfftw.FFTW(win, WIN, axes=(1,), direction='FFTW_FORWARD', threads=4)
+    win = pyfftw.empty_aligned((ncv, NBATCH), dtype="float32")
+    WIN = pyfftw.empty_aligned((ncv, int(NBATCH / 2 + 1)), dtype="complex64")
+    fft_object = pyfftw.FFTW(win, WIN, axes=(1,), direction="FFTW_FORWARD", threads=4)
     dephas = np.zeros((ncv, NBATCH), dtype=np.float32)
-    dephas[:, 1] = 1.
-    DEPHAS = np.exp(1j * np.angle(fft_object(dephas)) * h['sample_shift'][:, np.newaxis])
+    dephas[:, 1] = 1.0
+    DEPHAS = np.exp(
+        1j * np.angle(fft_object(dephas)) * h["sample_shift"][:, np.newaxis]
+    )
 
-    # if we want to compute the rms ap across the session
+    # if we want to compute the rms ap across the session as well as the saturation
     if compute_rms:
-        ap_rms_file = output_file.parent.joinpath('ap_rms.bin')
-        ap_time_file = output_file.parent.joinpath('ap_time.bin')
+        # creates a saturation memmap, this is a nsamples vector of booleans
+        file_saturation = output_file.parent.joinpath("_iblqc_ephysSaturation.samples.npy")
+        np.save(file_saturation, np.zeros(sr.ns, dtype=bool))
+        # creates the place holders for the rms
+        ap_rms_file = output_file.parent.joinpath("ap_rms.bin")
+        ap_time_file = output_file.parent.joinpath("ap_time.bin")
         rms_nbytes = np.float32(1).nbytes
-
         if append:
             rms_offset = Path(ap_rms_file).stat().st_size
             time_offset = Path(ap_time_file).stat().st_size
-            with open(ap_time_file, 'rb') as tid:
+            with open(ap_time_file, "rb") as tid:
                 t = tid.read()
             time_data = np.frombuffer(t, dtype=np.float32)
             t0 = time_data[-1]
         else:
             rms_offset = 0
             time_offset = 0
             t0 = 0
-            open(ap_rms_file, 'wb').close()
-            open(ap_time_file, 'wb').close()
-
+            open(ap_rms_file, "wb").close()
+            open(ap_time_file, "wb").close()
     if append:
         # need to find the end of the file and the offset
         offset = Path(output_file).stat().st_size
     else:
         offset = 0
-        open(output_file, 'wb').close()
+        open(output_file, "wb").close()
 
     # chunks to split the file into, dependent on number of parallel processes
     CHUNK_SIZE = int(sr.ns / nprocesses)
 
     def my_function(i_chunk, n_chunk):
         _sr = spikeglx.Reader(sr_file, **reader_kwargs)
-
+        _saturation = np.load(file_saturation, mmap_mode="r+")
         n_batch = int(np.ceil(i_chunk * CHUNK_SIZE / NBATCH))
         first_s = (NBATCH - SAMPLES_TAPER * 2) * n_batch
 
         # Find the maximum sample for each chunk
         max_s = _sr.ns if i_chunk == n_chunk - 1 else (i_chunk + 1) * CHUNK_SIZE
         # need to redefine this here to avoid 4 byte boundary error
-        win = pyfftw.empty_aligned((ncv, NBATCH), dtype='float32')
-        WIN = pyfftw.empty_aligned((ncv, int(NBATCH / 2 + 1)), dtype='complex64')
-        fft_object = pyfftw.FFTW(win, WIN, axes=(1,), direction='FFTW_FORWARD', threads=4)
-        ifft_object = pyfftw.FFTW(WIN, win, axes=(1,), direction='FFTW_BACKWARD', threads=4)
+        win = pyfftw.empty_aligned((ncv, NBATCH), dtype="float32")
+        WIN = pyfftw.empty_aligned((ncv, int(NBATCH / 2 + 1)), dtype="complex64")
+        fft_object = pyfftw.FFTW(
+            win, WIN, axes=(1,), direction="FFTW_FORWARD", threads=4
+        )
+        ifft_object = pyfftw.FFTW(
+            WIN, win, axes=(1,), direction="FFTW_BACKWARD", threads=4
+        )
 
-        fid = open(output_file, 'r+b')
+        fid = open(output_file, "r+b")
         if i_chunk == 0:
             fid.seek(offset)
         else:
             fid.seek(offset + ((first_s + SAMPLES_TAPER) * nc_out * nbytes))
 
         if compute_rms:
-            aid = open(ap_rms_file, 'r+b')
-            tid = open(ap_time_file, 'r+b')
+            aid = open(ap_rms_file, "r+b")
+            tid = open(ap_time_file, "r+b")
             if i_chunk == 0:
                 aid.seek(rms_offset)
                 tid.seek(time_offset)
             else:
                 aid.seek(rms_offset + (n_batch * ncv * rms_nbytes))
                 tid.seek(time_offset + (n_batch * rms_nbytes))
 
         while True:
             last_s = np.minimum(NBATCH + first_s, _sr.ns)
             # Apply tapers
             chunk = _sr[first_s:last_s, :ncv].T
+            saturated_samples, mute_saturation = saturation(
+                data=chunk, max_voltage=_sr.range_volts[:ncv], fs=_sr.fs)
+            _saturation[first_s:last_s] = saturated_samples
             chunk[:, :SAMPLES_TAPER] *= taper[:SAMPLES_TAPER]
             chunk[:, -SAMPLES_TAPER:] *= taper[SAMPLES_TAPER:]
             # Apply filters
             chunk = scipy.signal.sosfiltfilt(sos, chunk)
             # Find the indices to save
             ind2save = [SAMPLES_TAPER, NBATCH - SAMPLES_TAPER]
             if last_s == _sr.ns:
                 # for the last batch just use the normal fft as the stencil doesn't fit
-                chunk = fourier.fshift(chunk, s=h['sample_shift'])
+                chunk = fourier.fshift(chunk, s=h["sample_shift"])
                 ind2save[1] = NBATCH
             else:
                 # apply precomputed fshift of the proper length
                 chunk = ifft_object(fft_object(chunk) * DEPHAS)
             if first_s == 0:
                 # for the first batch save the start with taper applied
                 ind2save[0] = 0
             # interpolate missing traces after the low-cut filter it's important to leave the
             # channels outside of the brain outside of the computation
             if reject_channels:
-                chunk = interpolate_bad_channels(chunk, channel_labels, h['x'], h['y'])
+                chunk = interpolate_bad_channels(chunk, channel_labels, h["x"], h["y"])
                 inside_brain = np.where(channel_labels != 3)[0]
-                chunk[inside_brain, :] = spatial_fcn(chunk[inside_brain, :])  # apply the k-filter / CAR
+                # this applies either the k-filter or CAR
+                chunk[inside_brain, :] = spatial_fcn(chunk[inside_brain, :])
             else:
                 chunk = spatial_fcn(chunk)  # apply the k-filter / CAR
 
             # add back sync trace and save
             chunk = np.r_[chunk, _sr[first_s:last_s, ncv:].T].T
+            chunk = chunk * mute_saturation[:, np.newaxis]
 
             # Compute rms - we get it before applying the whitening
             if compute_rms:
                 ap_rms = utils.rms(chunk[:, :ncv], axis=0)
                 ap_t = t0 + (first_s + (last_s - first_s - 1) / 2) / _sr.fs
                 ap_rms.astype(np.float32).tofile(aid)
                 ap_t.astype(np.float32).tofile(tid)
@@ -489,36 +603,42 @@
                 chunk[:, :ncv] = np.dot(chunk[:, :ncv], wrot)
             chunk[:, :nc_out].astype(dtype).tofile(fid)
             first_s += NBATCH - SAMPLES_TAPER * 2
 
             if last_s >= max_s:
                 if last_s == _sr.ns:
                     if ns2add > 0:
-                        np.tile(chunk[-1, :nc_out].astype(dtype), (ns2add, 1)).tofile(fid)
+                        np.tile(chunk[-1, :nc_out].astype(dtype), (ns2add, 1)).tofile(
+                            fid
+                        )
                 fid.close()
                 if compute_rms:
                     aid.close()
                     tid.close()
                 break
 
-    _ = Parallel(n_jobs=nprocesses)(delayed(my_function)(i, nprocesses) for i in range(nprocesses))
+    _ = Parallel(n_jobs=nprocesses)(
+        delayed(my_function)(i, nprocesses) for i in range(nprocesses)
+    )
     sr.close()
 
     # Here convert the ap_rms bin files to the ibl format and save
     if compute_rms:
-        with open(ap_rms_file, 'rb') as aid, open(ap_time_file, 'rb') as tid:
+        with open(ap_rms_file, "rb") as aid, open(ap_time_file, "rb") as tid:
             rms_data = aid.read()
             time_data = tid.read()
         time_data = np.frombuffer(time_data, dtype=np.float32)
         rms_data = np.frombuffer(rms_data, dtype=np.float32)
-        assert (rms_data.shape[0] == time_data.shape[0] * ncv)
+        assert rms_data.shape[0] == time_data.shape[0] * ncv
         rms_data = rms_data.reshape(time_data.shape[0], ncv)
         output_qc_path = output_qc_path or output_file.parent
-        np.save(output_qc_path.joinpath('_iblqc_ephysTimeRmsAP.rms.npy'), rms_data)
-        np.save(output_qc_path.joinpath('_iblqc_ephysTimeRmsAP.timestamps.npy'), time_data)
+        np.save(output_qc_path.joinpath("_iblqc_ephysTimeRmsAP.rms.npy"), rms_data)
+        np.save(
+            output_qc_path.joinpath("_iblqc_ephysTimeRmsAP.timestamps.npy"), time_data
+        )
 
 
 def detect_bad_channels(raw, fs, similarity_threshold=(-0.5, 1), psd_hf_threshold=None):
     """
     Bad channels detection for Neuropixel probes
     Labels channels
      0: all clear
@@ -537,15 +657,15 @@
         Computes Pearson correlation with the sum of neighbouring traces
         :param raw: nc, ns
         :param n:
         :return:
         """
         nc = raw.shape[0]
         mixer = np.triu(np.ones((nc, nc)), 1) - np.triu(np.ones((nc, nc)), 1 + n)
-        mixer += np.tril(np.ones((nc, nc)), -1) - np.tril(np.ones((nc, nc)), - n - 1)
+        mixer += np.tril(np.ones((nc, nc)), -1) - np.tril(np.ones((nc, nc)), -n - 1)
         r = rcoeff(raw, np.matmul(raw.T, mixer).T)
         r[np.isnan(r)] = 0
         return r
 
     def detrend(x, nmed):
         """
         Subtract the trend from a vector
@@ -564,16 +684,19 @@
         """
         Computes the similarity based on zero-lag crosscorrelation of each channel with the median
         trace referencing
         :param raw: [nc, ns]
         :param nmed:
         :return:
         """
+
         def fxcor(x, y):
-            return scipy.fft.irfft(scipy.fft.rfft(x) * np.conj(scipy.fft.rfft(y)), n=raw.shape[-1])
+            return scipy.fft.irfft(
+                scipy.fft.rfft(x) * np.conj(scipy.fft.rfft(y)), n=raw.shape[-1]
+            )
 
         def nxcor(x, ref):
             ref = ref - np.mean(ref)
             apeak = fxcor(ref, ref)[0]
             x = x - np.mean(x, axis=-1)[:, np.newaxis]  # remove DC component
             return fxcor(x, ref)[:, 0] / apeak
 
@@ -587,32 +710,39 @@
     nc, _ = raw.shape
     raw = raw - np.mean(raw, axis=-1)[:, np.newaxis]  # removes DC offset
     xcor = channels_similarity(raw)
     fscale, psd = scipy.signal.welch(raw * 1e6, fs=fs)  # units; uV ** 2 / Hz
     if psd_hf_threshold is None:
         # the LFP band data is obviously much stronger so auto-adjust the default threshold
         psd_hf_threshold = 1.4 if fs < 5000 else 0.02
-    sos_hp = scipy.signal.butter(**{'N': 3, 'Wn': 300 / fs * 2, 'btype': 'highpass'}, output='sos')
+    sos_hp = scipy.signal.butter(
+        **{"N": 3, "Wn": 300 / fs * 2, "btype": "highpass"}, output="sos"
+    )
     hf = scipy.signal.sosfiltfilt(sos_hp, raw)
     xcorf = channels_similarity(hf)
 
-    xfeats = ({
-        'ind': np.arange(nc),
-        'rms_raw': utils.rms(raw),  # very similar to the rms avfter butterworth filter
-        'xcor_hf': detrend(xcor, 11),
-        'xcor_lf': xcorf - detrend(xcorf, 11) - 1,
-        'psd_hf': np.mean(psd[:, fscale > (fs / 2 * 0.8)], axis=-1),  # 80% nyquists
-    })
+    xfeats = {
+        "ind": np.arange(nc),
+        "rms_raw": utils.rms(raw),  # very similar to the rms avfter butterworth filter
+        "xcor_hf": detrend(xcor, 11),
+        "xcor_lf": xcorf - detrend(xcorf, 11) - 1,
+        "psd_hf": np.mean(psd[:, fscale > (fs / 2 * 0.8)], axis=-1),  # 80% nyquists
+    }
 
     # make recommendation
     ichannels = np.zeros(nc)
-    idead = np.where(similarity_threshold[0] > xfeats['xcor_hf'])[0]
-    inoisy = np.where(np.logical_or(xfeats['psd_hf'] > psd_hf_threshold, xfeats['xcor_hf'] > similarity_threshold[1]))[0]
+    idead = np.where(similarity_threshold[0] > xfeats["xcor_hf"])[0]
+    inoisy = np.where(
+        np.logical_or(
+            xfeats["psd_hf"] > psd_hf_threshold,
+            xfeats["xcor_hf"] > similarity_threshold[1],
+        )
+    )[0]
     # the channels outside of the brains are the contiguous channels below the threshold on the trend coherency
-    ioutside = np.where(xfeats['xcor_lf'] < -0.75)[0]
+    ioutside = np.where(xfeats["xcor_lf"] < -0.75)[0]
     if ioutside.size > 0 and ioutside[-1] == (nc - 1):
         a = np.cumsum(np.r_[0, np.diff(ioutside) - 1])
         ioutside = ioutside[a == np.max(a)]
         ichannels[ioutside] = 3
 
     # indices
     ichannels[idead] = 1
@@ -627,15 +757,17 @@
     Runs a ap-binary file scan to automatically detect faulty channels
     :param bin_file: full file path to the binary or compressed binary file from spikeglx
     :param n_batches: number of batches throughout the file (defaults to 10)
     :param batch_duration: batch length in seconds, defaults to 0.3
     :param display: if True will return a figure with features and an excerpt of the raw data
     :return: channel_labels: nc int array with 0:ok, 1:dead, 2:high noise, 3:outside of the brain
     """
-    sr = bin_file if isinstance(bin_file, spikeglx.Reader) else spikeglx.Reader(bin_file)
+    sr = (
+        bin_file if isinstance(bin_file, spikeglx.Reader) else spikeglx.Reader(bin_file)
+    )
     nc = sr.nc - sr.nsync
     channel_labels = np.zeros((nc, n_batches))
     # loop over the file and take the mode of detections
     for i, t0 in enumerate(np.linspace(0, sr.rl - batch_duration, n_batches)):
         sl = slice(int(t0 * sr.fs), int((t0 + batch_duration) * sr.fs))
         channel_labels[:, i], _xfeats = detect_bad_channels(sr[sl, :nc].T, fs=sr.fs)
         if i == 0:  # init the features dictionary if necessary
@@ -645,14 +777,15 @@
     # the features are averaged  so there may be a discrepancy between the mode and applying
     # the thresholds to the average of the features - the goal of those features is for display only
     xfeats_med = {k: np.median(xfeats[k], axis=-1) for k in xfeats}
     channel_flags, _ = scipy.stats.mode(channel_labels, axis=1)
     if display:
         raw = sr[sl, :nc].TO
         from ibllib.plots.figures import ephys_bad_channels
+
         ephys_bad_channels(raw, sr.fs, channel_flags, xfeats_med)
     return channel_flags
 
 
 def resample_denoise_lfp_cbin(lf_file, RESAMPLE_FACTOR=10, output=None):
     """
     Downsamples an LFP file and apply dstriping
@@ -663,33 +796,43 @@
     ```
     :param lf_file:
     :param RESAMPLE_FACTOR:
     :param output: Path
     :return: None
     """
 
-    output = output or Path(lf_file).parent.joinpath('lf_resampled.bin')
+    output = output or Path(lf_file).parent.joinpath("lf_resampled.bin")
     sr = spikeglx.Reader(lf_file)
     wg = utils.WindowGenerator(ns=sr.ns, nswin=65536, overlap=1024)
     cflags = detect_bad_channels_cbin(lf_file)
 
     c = 0
-    with open(output, 'wb') as f:
+    with open(output, "wb") as f:
         for first, last in wg.firstlast:
-            butter_kwargs = {'N': 3, 'Wn': np.array([2, 200]) / sr.fs * 2, 'btype': 'bandpass'}
-            sos = scipy.signal.butter(**butter_kwargs, output='sos')
-            raw = sr[first:last, :-sr.nsync]
+            butter_kwargs = {
+                "N": 3,
+                "Wn": np.array([2, 200]) / sr.fs * 2,
+                "btype": "bandpass",
+            }
+            sos = scipy.signal.butter(**butter_kwargs, output="sos")
+            raw = sr[first:last, : -sr.nsync]
             raw = scipy.signal.sosfiltfilt(sos, raw, axis=0)
             destripe = destripe_lfp(raw.T, fs=sr.fs, channel_labels=cflags)
             # viewephys(raw.T, fs=sr.fs, title='raw')
             # viewephys(destripe, fs=sr.fs, title='destripe')
-            rsamp = scipy.signal.decimate(destripe, RESAMPLE_FACTOR, axis=1, ftype='fir').T
+            rsamp = scipy.signal.decimate(
+                destripe, RESAMPLE_FACTOR, axis=1, ftype="fir"
+            ).T
             # viewephys(rsamp, fs=sr.fs / RESAMPLE_FACTOR, title='rsamp')
             first_valid = 0 if first == 0 else int(wg.overlap / 2 / RESAMPLE_FACTOR)
-            last_valid = rsamp.shape[0] if last == sr.ns else int(rsamp.shape[0] - wg.overlap / 2 / RESAMPLE_FACTOR)
+            last_valid = (
+                rsamp.shape[0]
+                if last == sr.ns
+                else int(rsamp.shape[0] - wg.overlap / 2 / RESAMPLE_FACTOR)
+            )
             rsamp = rsamp[first_valid:last_valid, :]
             c += rsamp.shape[0]
             print(first, last, last - first, first_valid, last_valid, c)
             rsamp.astype(np.float32).tofile(f)
     # first, last = (500, 550)
     # viewephys(sr[int(first * sr.fs) : int(last * sr.fs), :-sr.nsync].T, sr.fs, title='orig')
     # viewephys(sr_[int(first * sr_.fs):int(last * sr_.fs), :].T, sr_.fs, title='rsamp')
@@ -714,58 +857,64 @@
         i2stack = sind == uinds
         stack[sind, :] = fcn_agg(data[i2stack, :], axis=0)
 
     # aggregate the header using pandas
     if header is None:
         hstack = fold
     else:
-        header['stack_word'] = word
-        dfh = pd.DataFrame(header).groupby('stack_word')
-        hstack = dfh.aggregate('mean').to_dict(orient='series')
+        header["stack_word"] = word
+        dfh = pd.DataFrame(header).groupby("stack_word")
+        hstack = dfh.aggregate("mean").to_dict(orient="series")
         hstack = {k: hstack[k].values for k in hstack.keys()}
-        hstack['fold'] = fold
+        hstack["fold"] = fold
 
     return stack, hstack
 
 
-def current_source_density(lfp, h, method='diff', sigma=1 / 3):
+def current_source_density(lfp, h, method="diff", sigma=1 / 3):
     """
     Compute the current source density (CSD) of a given LFP signal recorded on neuropixel 1 or 2
     :param data: LFP signal (n_channels, n_samples)
     :param h: trace header dictionary
     :param method: diff (straight double difference) or kernel CSD (needs the KCSD python package)
     :param sigma: conductivity, defaults to 1/3 S.m-1
     :return:
     """
     csd = np.zeros(lfp.shape, dtype=np.float64) * np.NAN
-    xy = h['x'] + 1j * h['y']
-    for col in np.unique(h['col']):
-        ind = np.where(h['col'] == col)[0]
-        isort = np.argsort(h['row'][ind])
+    xy = h["x"] + 1j * h["y"]
+    for col in np.unique(h["col"]):
+        ind = np.where(h["col"] == col)[0]
+        isort = np.argsort(h["row"][ind])
         itr = ind[isort]
         dx = np.median(np.diff(np.abs(xy[itr])))
-        if method == 'diff':
-            csd[itr[1:-1], :] = np.diff(lfp[itr, :].astype(np.float64), n=2, axis=0) / dx ** 2 * sigma
+        if method == "diff":
+            csd[itr[1:-1], :] = (
+                np.diff(lfp[itr, :].astype(np.float64), n=2, axis=0) / dx**2 * sigma
+            )
             csd[itr[0], :] = csd[itr[1], :]
             csd[itr[-1], :] = csd[itr[-2], :]
-        elif method == 'kcsd':
+        elif method == "kcsd":
             from kcsd import KCSD1D
+
             # here we could eventually expose the KCSD kwargs
             csd[itr, :] = KCSD1D(
-                h['y'][itr, np.newaxis],
+                h["y"][itr, np.newaxis],
                 lfp[itr, :],
-                h=np.median(np.diff(h['y'][ind])),  # this seems to work well with the current intertrace
+                h=np.median(
+                    np.diff(h["y"][ind])
+                ),  # this seems to work well with the current intertrace
                 sigma=sigma,
-                xmin=np.min(h['y'][itr]),
-                xmax=np.max(h['y'][itr]),
-                gdx=np.ceil((np.max(h['y'][itr]) - np.min(h['y'][itr])) / itr.size),
-                lambd=0.,
-                R_init=5.,
+                xmin=np.min(h["y"][itr]),
+                xmax=np.max(h["y"][itr]),
+                gdx=np.ceil((np.max(h["y"][itr]) - np.min(h["y"][itr])) / itr.size),
+                lambd=0.0,
+                R_init=5.0,
                 n_src_init=10000,
-                src_type='gauss').values('CSD')
+                src_type="gauss",
+            ).values("CSD")
     return csd
 
 
 def _svd_denoise(datr, rank):
     """
     SVD Encoder: does the decomposition, derank the mtrix and reproject in the feature's space
     :param datr: input matrix
```

### Comparing `ibl-neuropixel-0.9.2/src/ibldsp/waveforms.py` & `ibl_neuropixel-1.0.0/src/ibldsp/waveforms.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,75 +2,84 @@
 This module is to compute features on spike waveforms.
 Throughout the code, the convention is to have 2D waveforms in the (time, traces)
 For efficiency, several wavforms are fed in a memory contiguous manner: (iwaveform, time, traces)
 """
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
+import scipy
+from ibldsp.utils import parabolic_max
+from ibldsp.fourier import fshift
 
 
 def _validate_arr_in(arr_in):
     # expand array if 2d
     if arr_in.ndim == 2:
         arr_in = arr_in[np.newaxis, :, :]
 
     # Init remove nan vals in entry array
     arr_in[np.isnan(arr_in)] = 0
     return arr_in
 
 
 def get_array_peak(arr_in, df):
-    '''
+    """
     Create matrix of just NxT (spikes x time) of the peak waveforms channel (=1 channel)
 
     :param arr_in: NxTxC waveform matrix (spikes x time x channel) ; expands to 1xTxC if TxC as input
     :param df: dataframe of waveform features
     :return: NxT waveform matrix : spikes x time, only the peak channel
-    '''
+    """
     arr_in = _validate_arr_in(arr_in)
-    arr_peak = arr_in[np.arange(arr_in.shape[0]), :, df['peak_trace_idx'].to_numpy()]
+    arr_peak = arr_in[np.arange(arr_in.shape[0]), :, df["peak_trace_idx"].to_numpy()]
     return arr_peak
 
 
 def invert_peak_waveform(arr_peak, df):
     # Get the sign of the peak
-    indx_pos = np.where(df['peak_val'].to_numpy() > 0)[0]
+    indx_pos = np.where(df["peak_val"].to_numpy() > 0)[0]
     # Flip positive wavs so all are negative
     if len(indx_pos) > 0:
         arr_peak[indx_pos, :] = -1 * arr_peak[indx_pos, :]
 
-    df['invert_sign_peak'] = np.sign(df['peak_val']) * -1  # Inverted signe peak to multiply point values by
+    df["invert_sign_peak"] = (
+        np.sign(df["peak_val"]) * -1
+    )  # Inverted signe peak to multiply point values by
     return arr_peak, df
 
 
 def arr_pre_post(arr_peak, indx_peak):
-    '''
+    """
     :param arr_peak: NxT waveform matrix : spikes x time, only the peak channel
     :param indx_peak: Nx1 matrix : indices of the peak for each channel
     :return:
-    '''
+    """
     # Create zero mask with 1 at peak, cumsum
     arr_mask = np.zeros(arr_peak.shape)
     arr_mask[np.arange(0, arr_mask.shape[0], 1), indx_peak] = 1
     arr_mask = np.cumsum(arr_mask, axis=1)
     # arr_mask[np.arange(0, arr_mask.shape[0], 1), indx_peak] = 2  # to keep peak in both cases
     # Commented code above not needed: We want to keep peak = nan when keeping pre-values
 
     # Pad with Nans (as cannot slice since each waveform will have different length from peak)
     indx_prepeak = np.where(arr_mask == 0)
     indx_postpeak = np.where(arr_mask == 1)
     del arr_mask
 
     arr_pre = arr_peak.copy()
-    arr_pre = arr_pre.astype('float')
-    arr_pre[indx_postpeak] = np.nan  # Array with values pre-, nans post- peak (from peak to end)
+    arr_pre = arr_pre.astype("float")
+    arr_pre[
+        indx_postpeak
+    ] = np.nan  # Array with values pre-, nans post- peak (from peak to end)
 
     arr_post = arr_peak.copy()
-    arr_post = arr_post.astype('float')
-    arr_post[indx_prepeak] = np.nan  # Array with values post-, nans pre- peak (from start to peak-1)
+    arr_post = arr_post.astype("float")
+    arr_post[
+        indx_prepeak
+    ] = np.nan  # Array with values post-, nans pre- peak (from start to peak-1)
     return arr_pre, arr_post
 
 
 def pick_maxima(arr_in):
     """
     From one or several single or multi-trace waveforms, extract the absolute maxima for all traces
     :param: arr_in: array of waveforms; 3D dimension have to be (wav, time, trace)
@@ -110,98 +119,104 @@
     arr_in = _validate_arr_in(arr_in)
 
     # 1. Find max peak (absolute deviation in STD units)
     indx_trace, indx_peak, val_peak = pick_maximum(arr_in)
 
     # Create dict / pd df
     df = pd.DataFrame()
-    df['peak_trace_idx'] = indx_trace
-    df['peak_time_idx'] = indx_peak
-    df['peak_val'] = val_peak
+    df["peak_trace_idx"] = indx_trace
+    df["peak_time_idx"] = indx_peak
+    df["peak_val"] = val_peak
     return df
 
 
 def find_trough(arr_peak, df):
     # Find tip (at peak waveform)
 
     # Create masks pre/post
-    arr_pre, arr_post = arr_pre_post(arr_peak, df['peak_time_idx'].to_numpy())
+    arr_pre, arr_post = arr_pre_post(arr_peak, df["peak_time_idx"].to_numpy())
 
     # Find trough
     # indx_trough = np.nanargmin(arr_post * np.sign(val_peak)[:, np.newaxis], axis=1)
     indx_trough = np.nanargmax(arr_post, axis=1)
-    val_trough = arr_peak[np.arange(0, arr_peak.shape[0], 1), indx_trough] * df['invert_sign_peak'].to_numpy()
+    val_trough = (
+        arr_peak[np.arange(0, arr_peak.shape[0], 1), indx_trough]
+        * df["invert_sign_peak"].to_numpy()
+    )
 
     # Put values into df
-    df['trough_time_idx'] = indx_trough
-    df['trough_val'] = val_trough
+    df["trough_time_idx"] = indx_trough
+    df["trough_val"] = val_trough
 
     return df
 
 
 def find_tip(arr_peak, df):
     # Find tip (at peak waveform)
 
     # Create masks pre/post
-    arr_pre, arr_post = arr_pre_post(arr_peak, df['peak_time_idx'].to_numpy())
+    arr_pre, arr_post = arr_pre_post(arr_peak, df["peak_time_idx"].to_numpy())
 
     # Find tip
-    '''
+    """
     # 02-06-2023 ; Decided not to use the inflection point but rather maximum
     # Leaving code for now commented as legacy example
 
     # Inflection point
     y_dif1 = np.diff(arr_pre, axis=1)
     indx_posit = np.where(y_dif1 > 0)
     del arr_pre
     arr_cs = np.zeros(y_dif1.shape)
     arr_cs[indx_posit] = 1
     indx_tip = np.argmax(np.cumsum(arr_cs, axis=1), axis=1) + 1
     val_tip = arr_peak[np.arange(0, arr_peak.shape[0], 1), indx_tip] * df['invert_sign_peak'].to_numpy()
     del arr_cs
-    '''
+    """
     # Maximum
     indx_tip = np.nanargmax(arr_pre, axis=1)
-    val_tip = arr_peak[np.arange(0, arr_peak.shape[0], 1), indx_tip] * df['invert_sign_peak'].to_numpy()
+    val_tip = (
+        arr_peak[np.arange(0, arr_peak.shape[0], 1), indx_tip]
+        * df["invert_sign_peak"].to_numpy()
+    )
 
     # Put values into df
-    df['tip_time_idx'] = indx_tip
-    df['tip_val'] = val_tip
+    df["tip_time_idx"] = indx_tip
+    df["tip_val"] = val_tip
 
     return df
 
 
 def find_tip_trough(arr_peak, arr_peak_real, df):
-    '''
+    """
     :param arr_in: inverted
     :param df:
     :return:
-    '''
+    """
     # 2. Find trough and tip (at peak waveform)
 
     # Find trough
     df = find_trough(arr_peak, df)
     df = peak_to_trough_ratio(df)
     # If ratio of peak/trough is near 1, and peak is positive :
     # Assign trough as peak on same waveform channel
     # Call the function again to compute trough etc. with new peak assigned
 
     # Find df rows to be changed
-    df_index = df.index[(df['peak_val'] > 0) & (df['peak_to_trough_ratio'] <= 1.5)]
+    df_index = df.index[(df["peak_val"] > 0) & (df["peak_to_trough_ratio"] <= 1.5)]
     df_rows = df.iloc[df_index]
     if len(df_index) > 0:
         # New peak - Swap peak for trough values
-        df_rows = df_rows.drop(['peak_val', 'peak_time_idx'], axis=1)
-        df_rows['peak_val'] = df_rows['trough_val']
-        df_rows['peak_time_idx'] = df_rows['trough_time_idx']
+        df_rows = df_rows.drop(["peak_val", "peak_time_idx"], axis=1)
+        df_rows["peak_val"] = df_rows["trough_val"]
+        df_rows["peak_time_idx"] = df_rows["trough_time_idx"]
 
         # df_trials.loc[iss, f] = predicted[f].values
 
         # Drop trough columns
-        df_rows = df_rows.drop(['trough_time_idx', 'trough_val'], axis=1)
+        df_rows = df_rows.drop(["trough_time_idx", "trough_val"], axis=1)
         # Create mini arr_peak for those rows uniquely (take the real waveforms value in, not inverted ones)
         arr_peak_rows = arr_peak_real[df_index, :]
         # Place into "inverted" array peak for return
         arr_peak[df_index, :] = arr_peak_rows
         # Get new sign for the peak
         arr_peak_rows, df_rows = invert_peak_waveform(arr_peak_rows, df_rows)
         # New trough
@@ -212,28 +227,29 @@
         df.loc[df_index] = df_rows
     # Find tip
     df = find_tip(arr_peak, df)
 
     return df, arr_peak
 
 
-def plot_wiggle(wav, ax=None, scalar=0.3, clip=1.5, **axkwargs):
+def plot_wiggle(wav, fs=1, ax=None, scalar=0.3, clip=1.5, **axkwargs):
     """
     Displays a multi-trace waveform in a wiggle traces with negative
     amplitudes filled
     :param wav: (nchannels, nsamples)
     :param axkwargs: keyword arguments to feed to ax.set()
     :return:
     """
     if ax is None:
         fig, ax = plt.subplots()
     nc, ns = wav.shape
     vals = np.c_[wav, wav[:, :1] * np.nan].ravel()  # flat view of the 2d array.
     vect = np.arange(vals.size).astype(
-        np.float32)  # flat index array, for correctly locating zero crossings in the flat view
+        np.float32
+    )  # flat index array, for correctly locating zero crossings in the flat view
     crossing = np.where(np.diff(np.signbit(vals)))[0]  # index before zero crossing
     # use linear interpolation to find the zero crossing, i.e. y = mx + c.
     x1 = vals[crossing]
     x2 = vals[crossing + 1]
     y1 = vect[crossing]
     y2 = vect[crossing + 1]
     m = (y2 - y1) / (x2 - x1)
@@ -242,278 +258,320 @@
     x = np.hstack([vals, np.zeros_like(c)]) * scalar
     x = np.maximum(np.minimum(x, clip), -clip)
     y = np.hstack([vect, c])
     # resort the data
     order = np.argsort(y)
     # shift from amplitudes to plotting coordinates
     x_shift, y = y[order].__divmod__(ns + 1)
-    ax.plot(y, x[order] + x_shift + 1, 'k', linewidth=.5)
+    ax.plot(y / fs, x[order] + x_shift + 1, 'k', linewidth=.5)
     x[x > 0] = np.nan
     x = x[order] + x_shift + 1
-    ax.fill(y, x, 'k', aa=True)
-    ax.set(xlim=[0, ns], ylim=[0, nc], xlabel='sample', ylabel='trace')
+    ax.fill(y / fs, x, 'k', aa=True)
+    ax.set(xlim=[0, ns / fs], ylim=[0, nc], xlabel='sample', ylabel='trace')
     plt.tight_layout()
     return ax
 
 
 def plot_peaktiptrough(df, arr, ax, nth_wav=0, plot_grey=True, fs=30000):
     # Time axix
     nech, ntr = arr[nth_wav].shape
     tscale = np.array([0, nech - 1]) / fs * 1e3
 
     if ax is None:
         fig, ax = plt.subplots()
     if plot_grey:
-        ax.plot(tscale, arr[nth_wav], c='gray', alpha=0.5)
+        ax.plot(tscale, arr[nth_wav], c="gray", alpha=0.5)
     # Peak channel
-    ax.plot(tscale, arr[nth_wav][:, int(df.iloc[nth_wav].peak_trace_idx)], marker=".", c='blue')
+    ax.plot(
+        tscale,
+        arr[nth_wav][:, int(df.iloc[nth_wav].peak_trace_idx)],
+        marker=".",
+        c="blue",
+    )
     # Peak point
-    ax.plot(tscale[df.iloc[nth_wav].peak_time_idx], df.iloc[nth_wav].peak_val, 'r*')
+    ax.plot(tscale[df.iloc[nth_wav].peak_time_idx], df.iloc[nth_wav].peak_val, "r*")
     # Trough point
-    ax.plot(tscale[df.iloc[nth_wav].trough_time_idx], df.iloc[nth_wav].trough_val, 'g*')
+    ax.plot(tscale[df.iloc[nth_wav].trough_time_idx], df.iloc[nth_wav].trough_val, "g*")
     # Tip point
-    ax.plot(tscale[df.iloc[nth_wav].tip_time_idx], df.iloc[nth_wav].tip_val, 'k*')
+    ax.plot(tscale[df.iloc[nth_wav].tip_time_idx], df.iloc[nth_wav].tip_val, "k*")
     # Half peak points
-    ax.plot(tscale[df.iloc[nth_wav].half_peak_post_time_idx], df.iloc[nth_wav].half_peak_post_val, 'c*')
-    ax.plot(tscale[df.iloc[nth_wav].half_peak_pre_time_idx], df.iloc[nth_wav].half_peak_pre_val, 'c*')
+    ax.plot(
+        tscale[df.iloc[nth_wav].half_peak_post_time_idx],
+        df.iloc[nth_wav].half_peak_post_val,
+        "c*",
+    )
+    ax.plot(
+        tscale[df.iloc[nth_wav].half_peak_pre_time_idx],
+        df.iloc[nth_wav].half_peak_pre_val,
+        "c*",
+    )
     # Line for half peak boundary
     # ax.plot((0, arr.shape[1]), np.array((1, 1)) * df.iloc[nth_wav].peak_val / 2, '-k')
-    ax.plot((tscale[0], tscale[-1]), np.array((1, 1)) * df.iloc[nth_wav].peak_val / 2, '-k')
+    ax.plot(
+        (tscale[0], tscale[-1]), np.array((1, 1)) * df.iloc[nth_wav].peak_val / 2, "-k"
+    )
     # Recovery point
-    ax.plot(tscale[df.iloc[nth_wav].recovery_time_idx], df.iloc[nth_wav].recovery_val, 'y*')
+    ax.plot(
+        tscale[df.iloc[nth_wav].recovery_time_idx], df.iloc[nth_wav].recovery_val, "y*"
+    )
     # Axis labels
-    ax.set_ylabel('(Volt)')
-    ax.set_xlabel('Time (ms)')
+    ax.set_ylabel("(Volt)")
+    ax.set_xlabel("Time (ms)")
 
 
 def half_peak_point(arr_peak, df):
-    '''
+    """
     Compute the two intersection points at halp-maximum peak
     :param: arr_peak: NxT waveform matrix : spikes x time, only the peak channel (inverted for positive wavs)
     :return: df with columns containing indices of intersection points and values, length of N wav
-    '''
+    """
     # TODO Review: is df.to_numpy() necessary ?
     # Compute half max value, repmat and substract it
-    half_max = (df['peak_val'].to_numpy() / 2) * df['invert_sign_peak'].to_numpy()
+    half_max = (df["peak_val"].to_numpy() / 2) * df["invert_sign_peak"].to_numpy()
     half_max_rep = np.tile(half_max, (arr_peak.shape[1], 1)).transpose()
     # Note on the above: using np.tile because np.repeat does not work with axis=1
     # todo rewrite with np.repeat and np.newaxis
     arr_sub = arr_peak - half_max_rep
     # Create masks pre/post
-    arr_pre, arr_post = arr_pre_post(arr_sub, df['peak_time_idx'].to_numpy())
+    arr_pre, arr_post = arr_pre_post(arr_sub, df["peak_time_idx"].to_numpy())
     # POST: Find first time it crosses 0 (from negative -> positive values)
     indx_post = np.argmax(arr_post > 0, axis=1)
-    val_post = arr_peak[np.arange(0, arr_peak.shape[0], 1), indx_post] * df['invert_sign_peak'].to_numpy()
+    val_post = (
+        arr_peak[np.arange(0, arr_peak.shape[0], 1), indx_post]
+        * df["invert_sign_peak"].to_numpy()
+    )
     # PRE:
     # Invert matrix (flip L-R) to find first point crossing threshold before peak
     arr_pre_flip = np.fliplr(arr_pre)
     # Find first time it crosses 0 (from negative -> positive values)
     indx_pre_flip = np.argmax(arr_pre_flip > 0, axis=1)
     # Fill a matrix of 0 with 1 at index, flip, then find index
     arr_zeros = np.zeros(arr_pre_flip.shape)
     arr_zeros[np.arange(0, arr_pre_flip.shape[0], 1), indx_pre_flip] = 1
     arr_pre_ones = np.fliplr(arr_zeros)
     # Find index where there are 1
     indx_pre = np.argmax(arr_pre_ones > 0, axis=1)
-    val_pre = arr_peak[np.arange(0, arr_peak.shape[0], 1), indx_pre] * df['invert_sign_peak'].to_numpy()
+    val_pre = (
+        arr_peak[np.arange(0, arr_peak.shape[0], 1), indx_pre]
+        * df["invert_sign_peak"].to_numpy()
+    )
 
     # Add columns to DF and return
-    df['half_peak_post_time_idx'] = indx_post
-    df['half_peak_pre_time_idx'] = indx_pre
-    df['half_peak_post_val'] = val_post
-    df['half_peak_pre_val'] = val_pre
+    df["half_peak_post_time_idx"] = indx_post
+    df["half_peak_pre_time_idx"] = indx_pre
+    df["half_peak_post_val"] = val_post
+    df["half_peak_pre_val"] = val_pre
 
     return df
 
 
 def half_peak_duration(df, fs=30000):
-    '''
+    """
     Compute the half peak duration (in second)
     :param df: dataframe of waveforms features, with the half peak intersection points computed
     :param fs:  sampling rate (Hz)
     :return: dataframe wirth added column
-    '''
-    df['half_peak_duration'] = (df['half_peak_post_time_idx'] - df['half_peak_pre_time_idx']) / fs
+    """
+    df["half_peak_duration"] = (
+        df["half_peak_post_time_idx"] - df["half_peak_pre_time_idx"]
+    ) / fs
     return df
 
 
 def peak_to_trough_duration(df, fs=30000):
-    '''
+    """
     Compute the duration (second) of the peak-to-trough
     :param df: dataframe of waveforms features
     :param fs: sampling rate (Hz)
     :return: df
-    '''
+    """
     # Duration
-    df['peak_to_trough_duration'] = (df['trough_time_idx'] - df['peak_time_idx']) / fs
+    df["peak_to_trough_duration"] = (df["trough_time_idx"] - df["peak_time_idx"]) / fs
     return df
 
 
 def peak_to_trough_ratio(df):
-    '''
+    """
     Compute the ratio of the peak-to-trough
     :param df: dataframe of waveforms features
     :param fs: sampling rate (Hz)
     :return:
-    '''
+    """
     # Ratio
-    df['peak_to_trough_ratio'] = np.abs(df['peak_val'] / df['trough_val'])  # Division by 0 returns NaN
+    df["peak_to_trough_ratio"] = np.abs(
+        df["peak_val"] / df["trough_val"]
+    )  # Division by 0 returns NaN
     # Ratio log-scale
-    df['peak_to_trough_ratio_log'] = np.log(df['peak_to_trough_ratio'])
+    df["peak_to_trough_ratio_log"] = np.log(df["peak_to_trough_ratio"])
     return df
 
 
 def polarisation_slopes(df, fs=30000):
-    '''
+    """
     Computes the depolarisation and repolarisation slopes as the difference between tip-peak
     and peak-trough respectively.
     :param df: dataframe of waveforms features
     :param fs: sampling frequency (Hz)
     :return: dataframe with added columns
-    '''
+    """
     # Depolarisation: slope before the peak (between tip and peak)
-    depolarise_duration = (df['peak_time_idx'] - df['tip_time_idx']) / fs
-    depolarise_volt = df['peak_val'] - df['tip_val']
-    df['depolarisation_slope'] = depolarise_volt / depolarise_duration
+    depolarise_duration = (df["peak_time_idx"] - df["tip_time_idx"]) / fs
+    depolarise_volt = df["peak_val"] - df["tip_val"]
+    df["depolarisation_slope"] = depolarise_volt / depolarise_duration
     # Repolarisation: slope after the peak (between peak and trough)
-    repolarise_duration = (df['trough_time_idx'] - df['peak_time_idx']) / fs
-    repolarise_volt = df['trough_val'] - df['peak_val']
-    df['repolarisation_slope'] = repolarise_volt / repolarise_duration
+    repolarise_duration = (df["trough_time_idx"] - df["peak_time_idx"]) / fs
+    repolarise_volt = df["trough_val"] - df["peak_val"]
+    df["repolarisation_slope"] = repolarise_volt / repolarise_duration
     return df
 
 
 def recovery_point(arr_peak, df, idx_from_trough=5):
-    '''
+    """
     Compute the single recovery secondary point (selected by a fixed increment
     from the trough). If the fixed increment from the trough is outside the matrix boundary, the
     last value of the waveform is used.
     :param arr_peak: NxT waveform matrix : spikes x time, only the peak channel
     :param df: dataframe of waveforms features
     :param idx_from_trough: sample index to be taken into account for the second point ; index from the trough
     :return: dataframe with added columns
-    '''
+    """
     # Check range is not outside of matrix boundary)
     if idx_from_trough >= (arr_peak.shape[1]):
-        raise ValueError('Index out of bound: Index larger than waveform array shape')
+        raise ValueError("Index out of bound: Index larger than waveform array shape")
 
     # Check df['peak_time_idx'] + pt_idx is not out of bound
-    idx_all = df['trough_time_idx'].to_numpy() + idx_from_trough
+    idx_all = df["trough_time_idx"].to_numpy() + idx_from_trough
     # Find waveform(s) for which the second point is outside matrix boundary range
     idx_over = np.where(idx_all > arr_peak.shape[1])[0]
     if len(idx_over) > 0:
         # Todo should this raise a warning ?
         idx_all[idx_over] = arr_peak.shape[1] - 1  # Take the last value of the waveform
 
-    df['recovery_time_idx'] = idx_all
-    df['recovery_val'] = arr_peak[np.arange(0, arr_peak.shape[0], 1), idx_all] * df['invert_sign_peak'].to_numpy()
+    df["recovery_time_idx"] = idx_all
+    df["recovery_val"] = (
+        arr_peak[np.arange(0, arr_peak.shape[0], 1), idx_all]
+        * df["invert_sign_peak"].to_numpy()
+    )
     return df
 
 
 def recovery_slope(df, fs=30000):
-    '''
+    """
     Compute the recovery slope, from the trough to the single secondary point.
     :param df: dataframe of waveforms features
     :param fs: sampling frequency (Hz)
     :return: dataframe with added columns
-    '''
+    """
     # Note: this could be lumped in with the polarisation_slopes
     # Time, volt and slope values
-    recovery_duration = (df['recovery_time_idx'] - df['trough_time_idx']) / fs  # Diff between second point and peak
-    recovery_volt = df['recovery_val'] - df['trough_val']
-    df['recovery_slope'] = recovery_volt / recovery_duration
+    recovery_duration = (
+        df["recovery_time_idx"] - df["trough_time_idx"]
+    ) / fs  # Diff between second point and peak
+    recovery_volt = df["recovery_val"] - df["trough_val"]
+    df["recovery_slope"] = recovery_volt / recovery_duration
     return df
 
 
 def dist_chanel_from_peak(channel_geometry, peak_trace_idx):
-    '''
+    """
     Compute distance for each channel from the peak channel, for each spike
     :param channel_geometry: Matrix N(spikes) * N(channels) * 3 (spatial coordinates x,y,z)
     # Note: computing this to provide it as input will be a pain
     :param peak_trace_idx: index of the highest amplitude channel in the multi-channel waveform
     :return: eu_dist : N(spikes) * N(channels): the euclidian distance between each channel and the peak channel,
     for each waveform
-    '''
+    """
     # Note: It deals with Nan in entry coordinate (fake padding channels); returns Nan as Eu dist
     # Get peak coordinates (x,y,z)
-    peak_coord = channel_geometry[np.arange(0, channel_geometry.shape[0], 1), peak_trace_idx, :]
+    peak_coord = channel_geometry[
+        np.arange(0, channel_geometry.shape[0], 1), peak_trace_idx, :
+    ]
 
     # repmat peak coordinates (x,y,z) [Nspikes x Ncoordinates] across channels
-    peak_coord_rep = np.repeat(peak_coord[:, :, np.newaxis], channel_geometry.shape[1], axis=2)  # Todo -1
-    peak_coord_rep = np.swapaxes(peak_coord_rep, 1, 2)  # N spikes x channel x coordinates
+    peak_coord_rep = np.repeat(
+        peak_coord[:, :, np.newaxis], channel_geometry.shape[1], axis=2
+    )  # Todo -1
+    peak_coord_rep = np.swapaxes(
+        peak_coord_rep, 1, 2
+    )  # N spikes x channel x coordinates
 
     # Difference
     diff_ch = peak_coord_rep - channel_geometry
     # Square
     square_ch = np.square(diff_ch)
     # Sum
     sum_ch = np.sum(square_ch, axis=2)
     # Sqrt
     eu_dist = np.sqrt(sum_ch)
     return eu_dist
 
 
 def spatial_spread_weighted(eu_dist, weights):
-    '''
+    """
     Returns the spatial spread defined by the sum(w_i * dist_i) / sum(w_i).
     The weight is a given value per channel (e.g. the absolute peak voltage value)
     :param eu_dist: N(spikes) * N(channels): the euclidian distance between each channel and the peak channel,
     for each waveform
     :param weights: N(spikes) * N(channels): the weights per channel per spikes
     :return: spatial_spread : N(spikes) * 1 vector
-    '''
+    """
     # Note: possible to have nan entries in eu_dist
-    spatial_spread = np.nansum(np.multiply(eu_dist, weights), axis=1) / np.sum(weights, axis=1)
+    spatial_spread = np.nansum(np.multiply(eu_dist, weights), axis=1) / np.sum(
+        weights, axis=1
+    )
     return spatial_spread
 
 
 def reshape_wav_one_channel(arr):
-    '''
+    """
     Reshape matrix so instead of being like waveforms: (wav, time, trace) i.e. (npsikes x nsamples x nchannels)
     it is of size (npsikes * nchannels) x nsamples
     :param waveforms: 3D np.array containing multi-channel waveforms, 3D dimension have to be (wav, time, trace)
     :return:
-    '''
+    """
     # Swap axis so the matrix is now: wav x channel x time
     arr_ax = np.swapaxes(arr, 1, 2)
     # reshape using the first 2 dimension (multiplied) x time
     arr_resh = arr_ax.reshape(-1, arr_ax.shape[-1])
     # add a new axis for computation
     arr_out = arr_resh[:, :, np.newaxis]
     return arr_out
 
 
-def weights_spk_ch(arr, weight_type='peak'):
-    '''
+def weights_spk_ch(arr, weight_type="peak"):
+    """
     Compute a value on all channels of a waveform matrix, and return as weights (to be used in spatial spread).
     :param arr: 3D np.array containing multi-channel waveforms, 3D dimension have to be (wav, time, trace)
     :param weight_type: value to be returned as weight (implemented: peak)
     :return: weights: N(spikes) * N(channels): the weights per channel per spikes
-    '''
+    """
     # Reshape
     arr_resh = reshape_wav_one_channel(arr)
     # Peak
     df = find_peak(arr_resh)
-    if weight_type == 'peak':
-        weights_flat = df['peak_val'].to_numpy()
+    if weight_type == "peak":
+        weights_flat = df["peak_val"].to_numpy()
     else:
-        raise ValueError('weight_type: unknown value attributed')
+        raise ValueError("weight_type: unknown value attributed")
     # Reshape
     # Order in DF: #1-2-3 channel of spike #1, then #1-2-3 channel spike #2 etc
     weights = np.reshape(weights_flat, (arr.shape[0], arr.shape[2]))
     return weights
 
 
-def compute_spatial_spread(arr, df, channel_geometry, weight_type='peak'):
+def compute_spatial_spread(arr, df, channel_geometry, weight_type="peak"):
     eu_dist = dist_chanel_from_peak(channel_geometry, df)
     weights = weights_spk_ch(arr, weight_type)
-    df['spatial_spread'] = spatial_spread_weighted(eu_dist, weights)
+    df["spatial_spread"] = spatial_spread_weighted(eu_dist, weights)
     return df
 
 
-def compute_spike_features(arr_in, fs=30000, recovery_duration_ms=0.16, return_peak_channel=False):
+def compute_spike_features(
+    arr_in, fs=30000, recovery_duration_ms=0.16, return_peak_channel=False
+):
     """
     This is the main function to compute spike features from a set of waveforms
     Current features:
     Index(['peak_trace_idx', 'peak_time_idx', 'peak_val', 'trough_time_idx',
        'trough_val', 'tip_time_idx', 'tip_val', 'half_peak_post_time_idx',
        'half_peak_pre_time_idx', 'half_peak_post_val', 'half_peak_pre_val',
        'half_peak_duration', 'recovery_time_idx', 'recovery_val',
@@ -525,26 +583,178 @@
     :return: dataframe of spikes with all features,
     Returns:
     """
     df = find_peak(arr_in)
     # Per waveform, keep only trace that contains the peak
     arr_peak_real = get_array_peak(arr_in, df)
     # Invert positive spikes
-    arr_peak, df = invert_peak_waveform(arr_peak_real.copy(), df)  # Copy otherwise overwrite the variable in memory
+    arr_peak, df = invert_peak_waveform(
+        arr_peak_real.copy(), df
+    )  # Copy otherwise overwrite the variable in memory
     # Tip-trough (this also computes the peak_to_trough_ratio)
     df, arr_peak = find_tip_trough(arr_peak, arr_peak_real, df)
     # Peak to trough duration
     df = peak_to_trough_duration(df, fs=30000)
     # Half peak points
     df = half_peak_point(arr_peak, df)
     # Half peak duration
     df = half_peak_duration(df, fs=fs)
     # Recovery point
-    df = recovery_point(arr_peak, df, idx_from_trough=int(round(recovery_duration_ms * fs / 1000)))
+    df = recovery_point(
+        arr_peak, df, idx_from_trough=int(round(recovery_duration_ms * fs / 1000))
+    )
     # Slopes
     df = polarisation_slopes(df, fs=fs)
     df = recovery_slope(df, fs=fs)
 
     if return_peak_channel:
         return df, arr_peak_real
     else:
         return df
+
+
+def wave_shift_corrmax(spike, spike2):
+    '''
+    Shift in time (sub-sample) the spike2 onto the spike
+    (For residual subtraction, typically, the spike2 would be the template)
+    :param spike: 1D array of float (e.g. on peak channel); same size as spike2
+    :param spike2: 1D array of float
+    :return: spike_resync: 1D array of float, shift_computed: in time sample (e.g. -4.03)
+    '''
+    # Numpy implementation of correlation centers it in the middle at np.floor(len_sample/2)
+    assert spike.shape[0] == spike2.shape[0]
+    sig_len = spike.shape[0]
+    c = scipy.signal.correlate(spike, spike2, mode='same')
+    ipeak, maxi = parabolic_max(c)
+    shift_computed = (ipeak - np.floor(sig_len / 2)) * -1
+    spike_resync = fshift(spike2, -shift_computed)
+    return spike_resync, shift_computed
+
+# -------------------------------------------------------------
+# Functions to fit the phase slope, and find the relationship between phase slope and sample shift
+
+
+def line_fit(x, a, b):  # function to fit a line and get the slope out
+    return a * x + b
+
+
+def get_apf_from2spikes(spike, spike2, fs):
+    fscale = np.fft.rfftfreq(spike.size, 1 / fs)
+    C = np.fft.rfft(spike) * np.conj(np.fft.rfft(spike2))
+
+    # Take the phase for freq at high amplitude, and compute slope
+    amp = np.abs(C)
+    phase = np.unwrap(np.angle(C))
+    return amp, phase, fscale
+
+
+def get_phase_slope(amp, phase, fscale, q=90):
+    # Take 90 percentile of distribution to find high amplitude freq
+    thresh_amp = np.percentile(amp, q)
+    indx_highamp = np.where(amp >= thresh_amp)[0]
+    # Perform linear fit to get the slope
+    popt, _ = scipy.optimize.curve_fit(line_fit, xdata=fscale[indx_highamp], ydata=phase[indx_highamp])
+    a, b = popt
+    return a, b
+
+
+def fit_phaseshift(phase_slopes, sample_shifts):
+    # Get parameters for the phase slope / sample shift curve
+    popt, _ = scipy.optimize.curve_fit(line_fit, xdata=sample_shifts, ydata=phase_slopes)
+    a, b = popt
+    return a, b
+
+
+def get_phase_from_fit(sample_shifts, a, b):
+    # phases = line_fit(np.abs(sample_shifts), a, b) * np.sign(sample_shifts)
+    phases = line_fit(sample_shifts, a, b)
+    return phases
+
+
+def get_shift_from_fit(phases, a, b):
+    # Invert the line function: x = (y-b)/a
+    sample_shifts = (phases - b) / a
+    return sample_shifts
+
+
+def get_spike_slopeparams(spike, fs, num_estim=50):
+    sample_shifts = np.linspace(-1, 1, num=num_estim)
+    phase_slopes = np.empty(shape=sample_shifts.shape)
+
+    for i_shift, sample_shift in enumerate(sample_shifts):
+        spike2 = fshift(spike, sample_shift)
+        # Get amplitude, phase, fscale
+        amp, phase, fscale = get_apf_from2spikes(spike, spike2, fs)
+        # Perform linear fit to get the slope
+        a, b = get_phase_slope(amp, phase, fscale)
+        phase_slopes[i_shift] = a
+
+    a_pslope, b_pslope = fit_phaseshift(phase_slopes, sample_shifts)
+    return a_pslope, b_pslope, sample_shifts, phase_slopes
+
+
+def wave_shift_phase(spike, spike2, fs, a_pos=None, b_pos=None):
+    '''
+    Resynch spike2 onto spike using the phase spectrum's slope
+    (this work perfectly in theory, but does not work well with raw daw sampled at 30kHz!)
+    '''
+    # Get template parameters if not passed in
+    if a_pos is None or b_pos is None:
+        a_pos, b_pos, _, _ = get_spike_slopeparams(spike, fs)
+    # Get amplitude, phase, fscale
+    amp, phase, fscale = get_apf_from2spikes(spike, spike2, fs)
+    # Perform linear fit to get the slope
+    a, b = get_phase_slope(amp, phase, fscale)
+    phase_slope = a
+    # Get sample shift
+    sample_shift = get_shift_from_fit(phase_slope, a_pos, b_pos)
+
+    # Resynch in time given phase slope
+    spike_resync = fshift(spike2, -sample_shift)  # Use negative to re-synch
+    return spike_resync, sample_shift
+
+# End of functions
+# -------------------------------------------------------------
+
+
+def shift_waveform(wf_cluster):
+    '''
+    :param wf_cluster: # A matrix of spike waveforms per cluster (N spike, trace, time)
+    :return: wf_out (same shape as waveform cluster): A matrix with the waveforms shifted in time
+    '''
+    # Take first the average as template to compute shift on
+    wfs_avg = np.nanmedian(wf_cluster, axis=0)
+    # Find the peak channel from template
+    template = np.transpose(wfs_avg.copy())  # wfs_avg is 2D (trace, time) -> transpose: (time, trace)
+    arr_temp = np.expand_dims(template, axis=0)  # 3D dimension have to be (wav, time, trace) -> add 1 dimension (ax=0)
+    df_temp = find_peak(arr_temp)
+    spike_template = arr_temp[:, :, df_temp['peak_trace_idx'][0]]  # Take template at peak trace
+    spike_template = np.squeeze(spike_template)
+
+    # Take the raw spikes at that channel
+    # Create df for all spikes
+    '''
+    Note: took the party here to NOT recompute the peak channel of each waveform, but to reuse the one from the
+    template — this is because the function to find the peak assumes the waveform has been denoised
+    and uses the maximum amplitude value --> which here would lead to failures in the case of collision
+    '''
+    df = pd.DataFrame()
+    df['peak_trace_idx'] = [df_temp['peak_trace_idx'][0]] * wf_cluster.shape[0]
+
+    # Per waveform, keep only trace that contains the peak
+    arr_in = np.swapaxes(wf_cluster, axis1=1, axis2=2)  # wfs size (wav, trace, time) -> swap (wav, time, trace)
+    arr_peak_real = get_array_peak(arr_in, df)
+
+    # Resynch 1 spike with 1 template (using only peak channel) ; Apply shift to all wav traces
+    wf_out = np.zeros(wf_cluster.shape)
+    shift_applied = np.zeros(wf_cluster.shape[0])
+    for i_spike in range(0, wf_cluster.shape[0]):
+        # Raw spike at peak channel
+        spike_raw = arr_peak_real[i_spike, :]
+        # Resynch
+        spike_template_resynch, shift_computed = wave_shift_corrmax(spike_raw, spike_template)
+        # Apply shift to all traces at once
+        wfs_avg_resync = fshift(wf_cluster[i_spike, :, :], shift_computed)
+        wf_out[i_spike, :, :] = wfs_avg_resync
+        shift_applied[i_spike] = shift_computed
+
+    return wf_out, shift_applied
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ibl-neuropixel-0.9.2/src/neuropixel.py` & `ibl_neuropixel-1.0.0/src/neuropixel.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,74 +7,81 @@
 
 import scipy.signal
 import numpy as np
 
 import spikeglx
 from ibldsp.utils import WindowGenerator
 
-_logger = logging.getLogger('ibllib')
+_logger = logging.getLogger("ibllib")
 
 # hardware pin to channel mapping
-SYNC_PIN_OUT = {'3A': {"pin01": 0,
-                       "pin02": 1,
-                       "pin03": 2,
-                       "pin04": 3,
-                       "pin05": None,
-                       "pin06": 4,
-                       "pin07": 5,
-                       "pin08": 6,
-                       "pin09": 7,
-                       "pin10": None,
-                       "pin11": 8,
-                       "pin12": 9,
-                       "pin13": 10,
-                       "pin14": 11,
-                       "pin15": None,
-                       "pin16": 12,
-                       "pin17": 13,
-                       "pin18": 14,
-                       "pin19": 15,
-                       "pin20": None,
-                       "pin21": None,
-                       "pin22": None,
-                       "pin23": None,
-                       "pin24": None
-                       },
-                '3B': {"P0.0": 0,
-                       "P0.1": 1,
-                       "P0.2": 2,
-                       "P0.3": 3,
-                       "P0.4": 4,
-                       "P0.5": 5,
-                       "P0.6": 6,
-                       "P0.7": 7,
-                       }
-                }
+SYNC_PIN_OUT = {
+    "3A": {
+        "pin01": 0,
+        "pin02": 1,
+        "pin03": 2,
+        "pin04": 3,
+        "pin05": None,
+        "pin06": 4,
+        "pin07": 5,
+        "pin08": 6,
+        "pin09": 7,
+        "pin10": None,
+        "pin11": 8,
+        "pin12": 9,
+        "pin13": 10,
+        "pin14": 11,
+        "pin15": None,
+        "pin16": 12,
+        "pin17": 13,
+        "pin18": 14,
+        "pin19": 15,
+        "pin20": None,
+        "pin21": None,
+        "pin22": None,
+        "pin23": None,
+        "pin24": None,
+    },
+    "3B": {
+        "P0.0": 0,
+        "P0.1": 1,
+        "P0.2": 2,
+        "P0.3": 3,
+        "P0.4": 4,
+        "P0.5": 5,
+        "P0.6": 6,
+        "P0.7": 7,
+    },
+}
 
 # sample to volt conversion factors
 S2V_AP = 2.34375e-06
 S2V_LFP = 4.6875e-06
 TIP_SIZE_UM = 200
 NC = 384
 SITES_COORDINATES: np.array
+# channel layouts for neuropixel probes as a function of the major version (1 or 2)
+CHANNEL_GRID = {1: dict(DX=16, X0=11, DY=20, Y0=20), 2: dict(DX=32, X0=27, DY=15, Y0=20)}
 
 
 def _deprecated_sites_coordinates() -> np.array:
     # this is used in legacy code
-    warnings.warn("the SITES_COORDINATES module attribute reflects only 374 channels and is only applicable to old"
-                  "deprecated 3A probes \n Use `neuropixel.trace_header() to get the canonical probe geometries "
-                  "according to the probe versions: see help(neuropixel.trace_header)."
-                  "\n If possible the reommended approach is to directly read the probe geometry"
-                  "from the metadata using spigeglx.Reader")
+    warnings.warn(
+        "the SITES_COORDINATES module attribute reflects only 374 channels and is only applicable to old"
+        "deprecated 3A probes \n Use `neuropixel.trace_header() to get the canonical probe geometries "
+        "according to the probe versions: see help(neuropixel.trace_header)."
+        "\n If possible the reommended approach is to directly read the probe geometry"
+        "from the metadata using spigeglx.Reader"
+    )
     for line in traceback.format_stack():
-        if 'ibllib' in line:
+        if "ibllib" in line:
             print(line.strip())
     refch_3a = np.array([36, 75, 112, 151, 188, 227, 264, 303, 340, 379])
     th = trace_header(version=1)
-    SITES_COORDINATES = np.delete(np.c_[th['x'], th['y']], refch_3a, axis=0)
+    SITES_COORDINATES = np.delete(np.c_[th["x"], th["y"]], refch_3a, axis=0)
     return SITES_COORDINATES
 
 
 def __getattr__(name: str) -> Any:
     # super hacky, once the SITES_COORDINATES values are deprecated, need to remove this function
     if name == "SITES_COORDINATES":
         return _deprecated_sites_coordinates()
@@ -86,64 +93,74 @@
     """
     converts the um indices to row/col coordinates.
     :param y: row coordinate on the probe
     :param x: col coordinate on the probe
     :param version: neuropixel major version 1 or 2
     :return: dictionary with keys x and y
     """
-    if version == 1:
-        col = (x - 11) / 16
-        row = (y - 20) / 20
-    elif np.floor(version) == 2:
-        col = x / 32
-        row = y / 15
-    return {'col': col, 'row': row}
+    grid = CHANNEL_GRID[np.floor(version)]
+    col = (x - grid['X0']) / grid['DX']
+    row = (y - grid['Y0']) / grid['DY']
+    return {"col": col, "row": row}
 
 
 def rc2xy(row, col, version=1):
     """
     converts the row/col indices to um coordinates.
     :param row: row index on the probe
     :param col: col index on the probe
     :param version: neuropixel major version 1 or 2
     :return: dictionary with keys x and y
     """
-    if version == 1:
-        x = col * 16 + 11
-        y = (row * 20) + 20
-    elif np.floor(version) == 2:
-        x = col * 32
-        y = row * 15
-    return {'x': x, 'y': y}
+    grid = CHANNEL_GRID[np.floor(version)]
+    x = col * grid['DX'] + grid['X0']
+    y = row * grid['DY'] + grid['Y0']
+    return {"x": x, "y": y}
 
 
 def dense_layout(version=1, nshank=1):
     """
     Returns a dense layout indices map for neuropixel, as used at IBL
     :param version: major version number: 1 or 2 or 2.4
     :return: dictionary with keys 'ind', 'col', 'row', 'x', 'y'
     """
-    ch = {'ind': np.arange(NC),
-          'row': np.floor(np.arange(NC) / 2),
-          'shank': np.zeros(NC)}
+    ch = {
+        "ind": np.arange(NC),
+        "row": np.floor(np.arange(NC) / 2),
+        "shank": np.zeros(NC),
+    }
 
     if version == 1:  # version 1 has a dense layout, checkerboard pattern
-        ch.update({'col': np.tile(np.array([2, 0, 3, 1]), int(NC / 4))})
-    elif np.floor(version) == 2 and nshank == 1:  # single shank NP1 has 2 columns in a dense patter
-        ch.update({'col': np.tile(np.array([0, 1]), int(NC / 2))})
-    elif np.floor(version) == 2 and nshank == 4:  # the 4 shank version default is rather complicated
+        ch.update({"col": np.tile(np.array([2, 0, 3, 1]), int(NC / 4))})
+    elif (
+        np.floor(version) == 2 and nshank == 1
+    ):  # single shank NP1 has 2 columns in a dense patter
+        ch.update({"col": np.tile(np.array([0, 1]), int(NC / 2))})
+    elif (
+        np.floor(version) == 2 and nshank == 4
+    ):  # the 4 shank version default is rather complicated
         shank_row = np.tile(np.arange(NC / 16), (2, 1)).T[:, np.newaxis].flatten()
         shank_row = np.tile(shank_row, 8)
-        shank_row += np.tile(np.array([0, 0, 1, 1, 0, 0, 1, 1])[:, np.newaxis], (1, int(NC / 8))).flatten() * 24
-        ch.update({
-            'col': np.tile(np.array([0, 1]), int(NC / 2)),
-            'shank': np.tile(np.array([0, 1, 0, 1, 2, 3, 2, 3])[:, np.newaxis], (1, int(NC / 8))).flatten(),
-            'row': shank_row})
+        shank_row += (
+            np.tile(
+                np.array([0, 0, 1, 1, 0, 0, 1, 1])[:, np.newaxis], (1, int(NC / 8))
+            ).flatten()
+            * 24
+        )
+        ch.update(
+            {
+                "col": np.tile(np.array([0, 1]), int(NC / 2)),
+                "shank": np.tile(
+                    np.array([0, 1, 0, 1, 2, 3, 2, 3])[:, np.newaxis], (1, int(NC / 8))
+                ).flatten(),
+                "row": shank_row,
+            }
+        )
     # for all, get coordinates
-    ch.update(rc2xy(ch['row'], ch['col'], version=version))
+    ch.update(rc2xy(ch["row"], ch["col"], version=version))
     return ch
 
 
 def adc_shifts(version=1, nc=NC):
     """
     Neuropixel NP1
     The sampling is serial within the same ADC, but it happens at the same time in all ADCs.
@@ -196,26 +213,26 @@
      ensure the channel maps corresponds the actually read data.`
     :param version: major version number: 1 or 2
     :param nshank: (defaults 1) number of shanks for NP2
     :return: , returns a dictionary with keys
     x, y, row, col, ind, adc and sampleshift vectors corresponding to each site
     """
     h = dense_layout(version=version, nshank=nshank)
-    h['sample_shift'], h['adc'] = adc_shifts(version=version)
+    h["sample_shift"], h["adc"] = adc_shifts(version=version)
     return h
 
 
 def split_trace_header(h, shank=0):
     """
     Split the trace header into values for a specific shank. Applicable for NP2.4 probes
     :param h:
     :param shank:
     :return:
     """
-    shank_idx = np.where(h['shank'] == shank)[0]
+    shank_idx = np.where(h["shank"] == shank)[0]
     h_shank = {key: h[key][shank_idx] for key in h.keys()}
     return h_shank
 
 
 class NP2Converter:
     """
     Class used to 1. Extract LFP data from NP2 data and 2. If NP2.4 split the data into
@@ -252,102 +269,116 @@
         :return:
         """
         self.fs_ap = 30000
         self.fs_lf = 2500
         self.ratio = int(self.fs_ap / self.fs_lf)
         self.nsamples = nsamples or self.sr.ns
         self.samples_window = nwindow or 2 * self.fs_ap
-        assert np.mod(self.samples_window, self.ratio) == 0, \
-            f'nwindow must be a factor or {self.ratio}'
+        assert (
+            np.mod(self.samples_window, self.ratio) == 0
+        ), f"nwindow must be a factor or {self.ratio}"
         self.samples_overlap = 576
-        assert np.mod(self.samples_overlap, self.ratio) == 0, \
-            f'samples_overlap must be a factor or {self.ratio}'
+        assert (
+            np.mod(self.samples_overlap, self.ratio) == 0
+        ), f"samples_overlap must be a factor or {self.ratio}"
         self.samples_taper = int(self.samples_overlap / 4)
-        assert np.mod(self.samples_taper, self.ratio) == 0, \
-            f'samples_taper must be a factor or {self.ratio}'
-        self.taper = np.r_[0, scipy.signal.windows.cosine((self.samples_taper - 1) * 2), 0]
+        assert (
+            np.mod(self.samples_taper, self.ratio) == 0
+        ), f"samples_taper must be a factor or {self.ratio}"
+        self.taper = np.r_[
+            0, scipy.signal.windows.cosine((self.samples_taper - 1) * 2), 0
+        ]
 
         # Low pass filter (acts as both anti-aliasing and LP filter)
-        butter_lp_kwargs = {'N': 2, 'Wn': 1000 / 2500 / 2, 'btype': 'lowpass'}
-        self.sos_lp = scipy.signal.butter(**butter_lp_kwargs, output='sos')
+        butter_lp_kwargs = {"N": 2, "Wn": 1000 / 2500 / 2, "btype": "lowpass"}
+        self.sos_lp = scipy.signal.butter(**butter_lp_kwargs, output="sos")
 
         # Number of ap channels
-        self.napch = int(self.sr.meta['snsApLfSy'][0])
+        self.napch = int(self.sr.meta["snsApLfSy"][0])
         # Position of start of sync channels in the raw data
-        self.idxsyncch = int(self.sr.meta['snsApLfSy'][0])
+        self.idxsyncch = int(self.sr.meta["snsApLfSy"][0])
 
-        self.extra = extra or ''
+        self.extra = extra or ""
         self.nshank = nshank or None
         self.check_completed = False
 
     def check_metadata(self):
         """
         Checks the keys in meta data to see if we are trying to process an ap file that has already
         been split into shanks. If we are sets flag and prevents further processing occurring
         :return:
         """
-        if self.sr.meta.get(f'{self.np_version}_shank', None) is not None:
+        if self.sr.meta.get(f"{self.np_version}_shank", None) is not None:
             self.already_processed = True
         else:
             self.already_processed = False
 
     def process(self, overwrite=False):
         """
         Function to call to process NP2 data
 
         :param overwrite:
         :return:
         """
-        if self.np_version == 'NP2.4':
+        if self.np_version == "NP2.4":
             status = self._process_NP24(overwrite=overwrite)
-        elif self.np_version == 'NP2.1':
+        elif self.np_version == "NP2.1":
             status = self._process_NP21(overwrite=overwrite)
         else:
-            _logger.warning('Meta file is not of type NP2.1 or NP2.4, cannot process')
+            _logger.warning("Meta file is not of type NP2.1 or NP2.4, cannot process")
             status = -1
         return status
 
     def _process_NP24(self, overwrite=False):
         """
         Splits AP signal into individual shanks and also extracts the LFP signal. Writes ap and
         lf data to ap.bin and lf.bin files in individual shank folders. Don't call this function
         directly but access through process() method
 
         :param overwrite:
         :return:
         """
         if self.already_processed:
-            _logger.warning('This ap file is an NP2.4 that has already been split into shanks, '
-                            'nothing to do here')
+            _logger.warning(
+                "This ap file is an NP2.4 that has already been split into shanks, "
+                "nothing to do here"
+            )
             return 0
 
         self.shank_info = self._prepare_files_NP24(overwrite=overwrite)
         if self.already_exists:
-            _logger.warning('One or more of the sub shank folders already exists, '
-                            'to force reprocessing set overwrite to True')
+            _logger.warning(
+                "One or more of the sub shank folders already exists, "
+                "to force reprocessing set overwrite to True"
+            )
             return 0
 
         # Initial checks out the way. Let's goooo!
         wg = WindowGenerator(self.nsamples, self.samples_window, self.samples_overlap)
 
         for first, last in wg.firstlast:
-            chunk_ap = self.sr[first:last, :self.napch].T
+            chunk_ap = self.sr[first:last, : self.napch].T
             chunk_ap_sync = self.sr[first:last, self.idxsyncch:].T
-            chunk_lf = self.extract_lfp(self.sr[first:last, :self.napch].T)
-            chunk_lf_sync = self.extract_lfp_sync(self.sr[first:last, self.idxsyncch:].T)
-
-            chunk_ap2save = self._ind2save(chunk_ap, chunk_ap_sync, wg, ratio=1, etype='ap')
-            chunk_lf2save = self._ind2save(chunk_lf, chunk_lf_sync, wg, ratio=self.ratio,
-                                           etype='lf')
+            chunk_lf = self.extract_lfp(self.sr[first:last, : self.napch].T)
+            chunk_lf_sync = self.extract_lfp_sync(
+                self.sr[first:last, self.idxsyncch:].T
+            )
+
+            chunk_ap2save = self._ind2save(
+                chunk_ap, chunk_ap_sync, wg, ratio=1, etype="ap"
+            )
+            chunk_lf2save = self._ind2save(
+                chunk_lf, chunk_lf_sync, wg, ratio=self.ratio, etype="lf"
+            )
 
-            self._split2shanks(chunk_ap2save, etype='ap')
-            self._split2shanks(chunk_lf2save, etype='lf')
+            self._split2shanks(chunk_ap2save, etype="ap")
+            self._split2shanks(chunk_lf2save, etype="lf")
 
-        self._closefiles(etype='ap')
-        self._closefiles(etype='lf')
+        self._closefiles(etype="ap")
+        self._closefiles(etype="lf")
 
         self._writemetadata_ap()
         self._writemetadata_lf()
 
         if self.post_check:
             self.check_NP24()
         if self.compress:
@@ -365,45 +396,51 @@
         process() method
 
         :param overwrite: set to True to force rerunning even if lf.bin file already exists
         :return:
         """
 
         chn_info = spikeglx._map_channels_from_meta(self.sr.meta)
-        n_shanks = self.nshank or np.unique(chn_info['shank']).astype(np.int16)
+        n_shanks = self.nshank or np.unique(chn_info["shank"]).astype(np.int16)
         label = self.ap_file.parent.parts[-1]
         shank_info = {}
         self.already_exists = False
 
         for sh in n_shanks:
             _shank_info = {}
             # channels for individual shank + sync channel
-            _shank_info['chns'] = np.r_[np.where(chn_info['shank'] == sh)[0],
-                                        np.array(spikeglx._get_sync_trace_indices_from_meta(
-                                            self.sr.meta))]
-
-            probe_path = self.ap_file.parent.parent.joinpath(label + chr(97 + int(sh)) + self.extra)
+            _shank_info["chns"] = np.r_[
+                np.where(chn_info["shank"] == sh)[0],
+                np.array(spikeglx._get_sync_trace_indices_from_meta(self.sr.meta)),
+            ]
+
+            probe_path = self.ap_file.parent.parent.joinpath(
+                label + chr(97 + int(sh)) + self.extra
+            )
 
             if not probe_path.exists() or overwrite:
                 if self.sr.is_mtscomp:
-                    ap_file_bin = self.ap_file.with_suffix('.bin').name
+                    ap_file_bin = self.ap_file.with_suffix(".bin").name
                 else:
                     ap_file_bin = self.ap_file.name
                 probe_path.mkdir(parents=True, exist_ok=True)
-                _shank_info['ap_file'] = probe_path.joinpath(ap_file_bin)
-                _shank_info['ap_open_file'] = open(_shank_info['ap_file'], 'wb')
-                _shank_info['lf_file'] = probe_path.joinpath(
-                    ap_file_bin.replace('ap', 'lf'))
-                _shank_info['lf_open_file'] = open(_shank_info['lf_file'], 'wb')
+                _shank_info["ap_file"] = probe_path.joinpath(ap_file_bin)
+                _shank_info["ap_open_file"] = open(_shank_info["ap_file"], "wb")
+                _shank_info["lf_file"] = probe_path.joinpath(
+                    ap_file_bin.replace("ap", "lf")
+                )
+                _shank_info["lf_open_file"] = open(_shank_info["lf_file"], "wb")
 
-                shank_info[f'shank{sh}'] = _shank_info
+                shank_info[f"shank{sh}"] = _shank_info
             else:
                 self.already_exists = True
-                _logger.warning('One or more of the sub shank folders already exists, '
-                                'to force reprocessing set overwrite to True')
+                _logger.warning(
+                    "One or more of the sub shank folders already exists, "
+                    "to force reprocessing set overwrite to True"
+                )
 
         return shank_info
 
     def _process_NP21(self, overwrite=False, offset=0, **kwargs):
         """
         Extracts LFP signal from original data and writes to lf.bin file. Also created lf.meta
         file. Don't call this function directly but access through process() method
@@ -411,34 +448,38 @@
         :param overwrite: set to True to force rerunning even if lf.bin file already exists
         :param offset: offset to add to the window generator in cases where the whole file doens't want to be processed
         :return:
         """
 
         self.shank_info = self._prepare_files_NP21(overwrite=overwrite, **kwargs)
         if self.already_exists:
-            _logger.warning('This ap file is an NP2.1 that already has lfp extracted, '
-                            'nothing to do here')
+            _logger.warning(
+                "This ap file is an NP2.1 that already has lfp extracted, "
+                "nothing to do here"
+            )
             return 0
 
         wg = WindowGenerator(self.nsamples, self.samples_window, self.samples_overlap)
 
         for first, last in wg.firstlast:
-
             first = first + offset
             last = last + offset
 
-            chunk_lf = self.extract_lfp(self.sr[first:last, :self.napch].T)
-            chunk_lf_sync = self.extract_lfp_sync(self.sr[first:last, self.idxsyncch:].T)
+            chunk_lf = self.extract_lfp(self.sr[first:last, : self.napch].T)
+            chunk_lf_sync = self.extract_lfp_sync(
+                self.sr[first:last, self.idxsyncch:].T
+            )
+
+            chunk_lf2save = self._ind2save(
+                chunk_lf, chunk_lf_sync, wg, ratio=self.ratio, etype="lf"
+            )
 
-            chunk_lf2save = self._ind2save(chunk_lf, chunk_lf_sync, wg, ratio=self.ratio,
-                                           etype='lf')
+            self._split2shanks(chunk_lf2save, etype="lf")
 
-            self._split2shanks(chunk_lf2save, etype='lf')
-
-        self._closefiles(etype='lf')
+        self._closefiles(etype="lf")
 
         self._writemetadata_lf()
 
         if self.compress:
             self.compress_NP21(overwrite=overwrite)
 
         return 1
@@ -451,307 +492,324 @@
 
         :param overwrite: set to True to force rerunning even if lf.bin file already exists
         :return:
         """
 
         chn_info = spikeglx._map_channels_from_meta(self.sr.meta)
         if assert_shanks:
-            n_shanks = np.unique(chn_info['shank']).astype(np.int16)
-            assert (len(n_shanks) == 1)
+            n_shanks = np.unique(chn_info["shank"]).astype(np.int16)
+            assert len(n_shanks) == 1
         else:
             n_shanks = np.array([0])
         shank_info = {}
         self.already_exists = False
 
-        lf_file = self.ap_file.parent.joinpath(self.ap_file.name.replace('ap', 'lf')).with_suffix('.bin')
-        lf_cbin_file = lf_file.with_suffix('.cbin')
+        lf_file = self.ap_file.parent.joinpath(
+            self.ap_file.name.replace("ap", "lf")
+        ).with_suffix(".bin")
+        lf_cbin_file = lf_file.with_suffix(".cbin")
         if not (lf_file.exists() or lf_cbin_file.exists()) or overwrite:
             for sh in n_shanks:
                 _shank_info = {}
                 # channels for individual shank + sync channel
                 if assert_shanks:
-                    _shank_info['chns'] = np.r_[np.where(chn_info['shank'] == sh)[0],
-                                                np.array(spikeglx._get_sync_trace_indices_from_meta(
-                                                    self.sr.meta))]
+                    _shank_info["chns"] = np.r_[
+                        np.where(chn_info["shank"] == sh)[0],
+                        np.array(
+                            spikeglx._get_sync_trace_indices_from_meta(self.sr.meta)
+                        ),
+                    ]
                 else:
-                    _shank_info['chns'] = np.arange(self.sr.nc)
+                    _shank_info["chns"] = np.arange(self.sr.nc)
 
-                _shank_info['lf_file'] = lf_file
-                _shank_info['lf_open_file'] = open(_shank_info['lf_file'], 'wb')
+                _shank_info["lf_file"] = lf_file
+                _shank_info["lf_open_file"] = open(_shank_info["lf_file"], "wb")
 
-                shank_info[f'shank{sh}'] = _shank_info
+                shank_info[f"shank{sh}"] = _shank_info
         else:
             self.already_exists = True
-            _logger.warning('LF file for this probe already exists, '
-                            'to force reprocessing set overwrite to True')
+            _logger.warning(
+                "LF file for this probe already exists, "
+                "to force reprocessing set overwrite to True"
+            )
 
         return shank_info
 
     def check_NP24(self):
         """
         Check that the splitting into shanks process has completed correctly. Compares the original
         file to the reconstructed file from the individual shanks
 
         :return:
         """
         for sh in self.shank_info.keys():
-            self.shank_info[sh]['sr'] = spikeglx.Reader(self.shank_info[sh]['ap_file'])
+            self.shank_info[sh]["sr"] = spikeglx.Reader(self.shank_info[sh]["ap_file"])
 
         wg = WindowGenerator(self.nsamples, self.samples_window, 0)
         for first, last in wg.firstlast:
             expected = self.sr[first:last, :]
             chunk = np.zeros_like(expected)
             for ish, sh in enumerate(self.shank_info.keys()):
                 if ish == 0:
-                    chunk[:, self.shank_info[sh]['chns']] = self.shank_info[sh]['sr'][first:last, :]
+                    chunk[:, self.shank_info[sh]["chns"]] = self.shank_info[sh]["sr"][
+                        first:last, :
+                    ]
                 else:
-                    chunk[:, self.shank_info[sh]['chns'][:-1]] = \
-                        self.shank_info[sh]['sr'][first:last, :-1]
-            assert np.array_equal(expected, chunk), \
-                'data in original file and split files do no match'
+                    chunk[:, self.shank_info[sh]["chns"][:-1]] = self.shank_info[sh][
+                        "sr"
+                    ][first:last, :-1]
+            assert np.array_equal(
+                expected, chunk
+            ), "data in original file and split files do no match"
 
         # close the sglx instances once we are done checking
         for sh in self.shank_info.keys():
-            sr = self.shank_info[sh].pop('sr')
+            sr = self.shank_info[sh].pop("sr")
             sr.close()
 
         self.check_completed = True
 
     def compress_NP24(self, overwrite=False, **kwargs):
         """
         Compress spikeglx files
         :return:
         """
         for sh in self.shank_info.keys():
-            bin_file = self.shank_info[sh]['ap_file']
+            bin_file = self.shank_info[sh]["ap_file"]
             if overwrite:
-                cbin_file = bin_file.with_suffix('.cbin')
+                cbin_file = bin_file.with_suffix(".cbin")
                 cbin_file.unlink()
 
             sr_ap = spikeglx.Reader(bin_file)
             cbin_file = sr_ap.compress_file(**kwargs)
             sr_ap.close()
             bin_file.unlink()
-            self.shank_info[sh]['ap_file'] = cbin_file
+            self.shank_info[sh]["ap_file"] = cbin_file
 
-            bin_file = self.shank_info[sh]['lf_file']
+            bin_file = self.shank_info[sh]["lf_file"]
             if overwrite:
-                cbin_file = bin_file.with_suffix('.cbin')
+                cbin_file = bin_file.with_suffix(".cbin")
                 cbin_file.unlink()
             sr_lf = spikeglx.Reader(bin_file)
             cbin_file = sr_lf.compress_file(**kwargs)
             sr_lf.close()
             bin_file.unlink()
-            self.shank_info[sh]['lf_file'] = cbin_file
+            self.shank_info[sh]["lf_file"] = cbin_file
 
     def compress_NP21(self, overwrite=False):
         """
         Compress spikeglx files
         :return:
         """
         for sh in self.shank_info.keys():
             if not self.sr.is_mtscomp:
                 cbin_file = self.sr.compress_file()
                 self.sr.close()
                 self.ap_file.unlink()
                 self.ap_file = cbin_file
                 self.sr = spikeglx.Reader(self.ap_file)
 
-            bin_file = self.shank_info[sh]['lf_file']
+            bin_file = self.shank_info[sh]["lf_file"]
             if overwrite:
-                cbin_file = bin_file.with_suffix('.cbin')
+                cbin_file = bin_file.with_suffix(".cbin")
                 cbin_file.unlink()
             sr_lf = spikeglx.Reader(bin_file)
             cbin_file = sr_lf.compress_file()
             sr_lf.close()
             bin_file.unlink()
-            self.shank_info[sh]['lf_file'] = cbin_file
+            self.shank_info[sh]["lf_file"] = cbin_file
 
     def delete_NP24(self):
         """
         Delete the original ap file that doesn't has all shanks in one file
 
         :return:
         """
         if self.check_completed and self.delete_original:
-            _logger.info(f'Removing original file in folder {self.ap_file}')
+            _logger.info(f"Removing original file in folder {self.ap_file}")
             self.sr.close()
             self.ap_file.unlink()
             # shutil.rmtree(self.ap_file.parent) #  should we remove the whole folder?
 
-    def _split2shanks(self, chunk, etype='ap'):
+    def _split2shanks(self, chunk, etype="ap"):
         """
         Splits the signal on the 384 channels into the individual shanks and saves to file
 
         :param chunk: portion of signal with all 384 channels
         :param type: ephys type, either 'ap' or 'lf'
         :return:
         """
 
         for sh in self.shank_info.keys():
-            open = self.shank_info[sh][f'{etype}_open_file']
-            (chunk[:, self.shank_info[sh]['chns']]).tofile(open)
+            open = self.shank_info[sh][f"{etype}_open_file"]
+            (chunk[:, self.shank_info[sh]["chns"]]).tofile(open)
 
-    def _ind2save(self, chunk, chunk_sync, wg, ratio=1, etype='ap'):
+    def _ind2save(self, chunk, chunk_sync, wg, ratio=1, etype="ap"):
         """
         Determines the portion of the full chunk to save based on the window and taper used. Cuts
         off beginning and end to get rid of filtering/ decimating artefacts
 
         :param chunk: chunk of ephys signal
         :param chunk_sync: chunk of sync signal
         :param wg: Window generator object
         :param ratio: downsample ratio
         :param etype: ephys type, either 'ap' or 'lf'
         :return:
         """
 
-        ind2save = [int(self.samples_taper * 2 / ratio),
-                    int((self.samples_window - self.samples_taper * 2) / ratio)]
+        ind2save = [
+            int(self.samples_taper * 2 / ratio),
+            int((self.samples_window - self.samples_taper * 2) / ratio),
+        ]
         if wg.iw == 0:
             ind2save[0] = 0
         if wg.iw == wg.nwin - 1:
             ind2save[1] = int(self.samples_window / ratio)
 
-        chunk2save = (np.c_[chunk[:, slice(*ind2save)].T /
-                            self.sr.channel_conversion_sample2v[etype][:self.napch],
-                            chunk_sync[:, slice(*ind2save)].T /
-                            self.sr.channel_conversion_sample2v[etype][self.idxsyncch:]]).\
-            astype(np.int16)
+        chunk2save = (
+            np.c_[
+                chunk[:, slice(*ind2save)].T
+                / self.sr.channel_conversion_sample2v[etype][: self.napch],
+                chunk_sync[:, slice(*ind2save)].T
+                / self.sr.channel_conversion_sample2v[etype][self.idxsyncch:],
+            ]
+        ).astype(np.int16)
 
         return chunk2save
 
     def extract_lfp(self, chunk):
         """
         Extracts LFP signal from full band signal, first applies low pass to anti-alias and LP,
         then downsamples
 
         :param chunk: portion of signal to extract LFP from
         :return: LFP signal
         """
 
-        chunk[:, :self.samples_taper] *= self.taper[:self.samples_taper]
+        chunk[:, : self.samples_taper] *= self.taper[: self.samples_taper]
         chunk[:, -self.samples_taper:] *= self.taper[self.samples_taper:]
         chunk = scipy.signal.sosfiltfilt(self.sos_lp, chunk)
-        chunk = chunk[:, ::self.ratio]
+        chunk = chunk[:, :: self.ratio]
         return chunk
 
     def extract_lfp_sync(self, chunk_sync):
         """
         Extracts downsampled signal of imec sync trace
 
         :param chunk_sync: portion of sync signal to downsample
         :return: downsampled sync signal
         """
 
-        chunk_sync = chunk_sync[:, ::self.ratio]
+        chunk_sync = chunk_sync[:, :: self.ratio]
         return chunk_sync
 
-    def _closefiles(self, etype='ap'):
+    def _closefiles(self, etype="ap"):
         """
         Close .bin files that were being written to
 
         :param etype: ephys type, either 'ap' or 'lf'
         :return:
         """
 
         for sh in self.shank_info.keys():
-            open = self.shank_info[sh].pop(f'{etype}_open_file')
+            open = self.shank_info[sh].pop(f"{etype}_open_file")
             open.close()
 
     def _writemetadata_ap(self):
         """
         Function to create ap meta data file. Adapts the relevant keys in the spikeglx meta file
         to contain the correct number of channels. Also adds key to indicate that this is not an
         original meta data file, but one that has been adapted
 
         :return:
         """
 
         for sh in self.shank_info.keys():
-            n_chns = len(self.shank_info[sh]['chns'])
+            n_chns = len(self.shank_info[sh]["chns"])
             # First for the ap file
             meta_shank = copy.deepcopy(self.sr.meta)
-            meta_shank['acqApLfSy'][0] = n_chns - 1
-            meta_shank['snsApLfSy'][0] = n_chns - 1
-            meta_shank['nSavedChans'] = n_chns
-            meta_shank['fileSizeBytes'] = self.shank_info[sh]['ap_file'].stat().st_size
-            meta_shank['snsSaveChanSubset_orig'] = \
-                spikeglx._get_savedChans_subset(self.shank_info[sh]['chns'])
-            meta_shank['snsSaveChanSubset'] = f'0:{n_chns-1}'
-            meta_shank['original_meta'] = False
-            meta_shank[f'{self.np_version}_shank'] = int(sh[-1])
-            meta_file = self.shank_info[sh]['ap_file'].with_suffix('.meta')
+            meta_shank["acqApLfSy"][0] = n_chns - 1
+            meta_shank["snsApLfSy"][0] = n_chns - 1
+            meta_shank["nSavedChans"] = n_chns
+            meta_shank["fileSizeBytes"] = self.shank_info[sh]["ap_file"].stat().st_size
+            meta_shank["snsSaveChanSubset_orig"] = spikeglx._get_savedChans_subset(
+                self.shank_info[sh]["chns"]
+            )
+            meta_shank["snsSaveChanSubset"] = f"0:{n_chns-1}"
+            meta_shank["original_meta"] = False
+            meta_shank[f"{self.np_version}_shank"] = int(sh[-1])
+            meta_file = self.shank_info[sh]["ap_file"].with_suffix(".meta")
             spikeglx.write_meta_data(meta_shank, meta_file)
 
     def _writemetadata_lf(self):
         """
         Function to create lf meta data file. Adapts the relevant keys in the spikeglx meta file
         to contain the correct number of channels. Also adds key to indicate that this is not an
         original meta data file, but one that has been adapted
 
         :return:
         """
 
         for sh in self.shank_info.keys():
-            n_chns = len(self.shank_info[sh]['chns'])
+            n_chns = len(self.shank_info[sh]["chns"])
             meta_shank = copy.deepcopy(self.sr.meta)
-            meta_shank['acqApLfSy'][0] = 0
-            meta_shank['acqApLfSy'][1] = n_chns - 1
-            meta_shank['snsApLfSy'][0] = 0
-            meta_shank['snsApLfSy'][1] = n_chns - 1
-            meta_shank['fileSizeBytes'] = self.shank_info[sh]['lf_file'].stat().st_size
-            meta_shank['imSampRate'] = self.fs_lf
-            if self.np_version == 'NP2.4':
-                meta_shank['snsSaveChanSubset_orig'] = \
-                    spikeglx._get_savedChans_subset(self.shank_info[sh]['chns'])
-                meta_shank['snsSaveChanSubset'] = f'0:{n_chns-1}'
-                meta_shank['nSavedChans'] = n_chns
-            meta_shank['original_meta'] = False
-            meta_shank[f'{self.np_version}_shank'] = int(sh[-1])
-            meta_file = self.shank_info[sh]['lf_file'].with_suffix('.meta')
+            meta_shank["acqApLfSy"][0] = 0
+            meta_shank["acqApLfSy"][1] = n_chns - 1
+            meta_shank["snsApLfSy"][0] = 0
+            meta_shank["snsApLfSy"][1] = n_chns - 1
+            meta_shank["fileSizeBytes"] = self.shank_info[sh]["lf_file"].stat().st_size
+            meta_shank["imSampRate"] = self.fs_lf
+            if self.np_version == "NP2.4":
+                meta_shank["snsSaveChanSubset_orig"] = spikeglx._get_savedChans_subset(
+                    self.shank_info[sh]["chns"]
+                )
+                meta_shank["snsSaveChanSubset"] = f"0:{n_chns-1}"
+                meta_shank["nSavedChans"] = n_chns
+            meta_shank["original_meta"] = False
+            meta_shank[f"{self.np_version}_shank"] = int(sh[-1])
+            meta_file = self.shank_info[sh]["lf_file"].with_suffix(".meta")
             spikeglx.write_meta_data(meta_shank, meta_file)
 
     def get_processed_files_NP24(self):
         """
         Function to return full list of files output from the NP conversion
         :return:
         """
         out_files = []
         for sh in self.shank_info.keys():
-            ap_file = self.shank_info[sh]['ap_file']
+            ap_file = self.shank_info[sh]["ap_file"]
             out_files.append(ap_file)
-            out_files.append(ap_file.with_suffix('.meta'))
+            out_files.append(ap_file.with_suffix(".meta"))
 
-            if ap_file.suffix == '.cbin':
-                out_files.append(ap_file.with_suffix('.ch'))
+            if ap_file.suffix == ".cbin":
+                out_files.append(ap_file.with_suffix(".ch"))
 
-            lf_file = self.shank_info[sh]['lf_file']
+            lf_file = self.shank_info[sh]["lf_file"]
             out_files.append(lf_file)
-            out_files.append(lf_file.with_suffix('.meta'))
+            out_files.append(lf_file.with_suffix(".meta"))
 
-            if lf_file.suffix == '.cbin':
-                out_files.append(lf_file.with_suffix('.ch'))
+            if lf_file.suffix == ".cbin":
+                out_files.append(lf_file.with_suffix(".ch"))
 
         return out_files
 
     def get_processed_files_NP21(self):
-
         out_files = []
         for sh in self.shank_info.keys():
-            lf_file = self.shank_info[sh]['lf_file']
+            lf_file = self.shank_info[sh]["lf_file"]
             out_files.append(lf_file)
-            out_files.append(lf_file.with_suffix('.meta'))
+            out_files.append(lf_file.with_suffix(".meta"))
 
-            if lf_file.suffix == '.cbin':
-                out_files.append(lf_file.with_suffix('.ch'))
+            if lf_file.suffix == ".cbin":
+                out_files.append(lf_file.with_suffix(".ch"))
 
         out_files.append(self.ap_file)
-        out_files.append(self.ap_file.with_suffix('.meta'))
-        if self.ap_file.suffix == '.cbin':
-            out_files.append(self.ap_file.with_suffix('.ch'))
+        out_files.append(self.ap_file.with_suffix(".meta"))
+        if self.ap_file.suffix == ".cbin":
+            out_files.append(self.ap_file.with_suffix(".ch"))
 
         return out_files
 
 
 class NP2Reconstructor:
     def __init__(self, raw_ephys_path, pname, compress=True):
         """
@@ -790,68 +848,76 @@
     def _prepare_files(self):
         """
         Searches for the relevant subshank files in the raw_ephys_data directory and opens the files with spikeglx ready to be
         accessed. Don't call this function directly but access through process() method
         :return:
         """
 
-        folders = list(self.data_path.glob(f'{self.pname}*'))
+        folders = list(self.data_path.glob(f"{self.pname}*"))
         # remove any probe00 folder if present
-        folders = sorted([fold for fold in folders if fold != self.data_path.joinpath(f'{self.pname}')])
+        folders = sorted(
+            [
+                fold
+                for fold in folders
+                if fold != self.data_path.joinpath(f"{self.pname}")
+            ]
+        )
 
         # TODO check the meta data
-        meta_file = next(folders[0].glob('*ap.meta'))
+        meta_file = next(folders[0].glob("*ap.meta"))
         meta_info = spikeglx.read_meta_data(meta_file)
         self.np_version = spikeglx._get_neuropixel_version_from_meta(meta_info)
-        if self.np_version != 'NP2.4':
-            _logger.warning('Not Neuropixel 2.4 nothing to do')
+        if self.np_version != "NP2.4":
+            _logger.warning("Not Neuropixel 2.4 nothing to do")
             return
 
-        ap_file = next(folders[0].glob('*ap.*bin'))
-        self.save_file = self.probe_path.joinpath(ap_file.name).with_suffix('.bin')
+        ap_file = next(folders[0].glob("*ap.*bin"))
+        self.save_file = self.probe_path.joinpath(ap_file.name).with_suffix(".bin")
 
         # note we use the private method here to make sure we get all of the original channels,
         # as the .geometry() method returns only channels pertaining to the shank
         chn_info = spikeglx._map_channels_from_meta(meta_info)
-        expected_shanks = np.unique(chn_info['shank'])
+        expected_shanks = np.unique(chn_info["shank"])
 
         if len(folders) != len(expected_shanks):
-            _logger.warning('Number of expected subfolders and number of shanks do not match')
+            _logger.warning(
+                "Number of expected subfolders and number of shanks do not match"
+            )
             return
 
         shank_info = {}
         for iF, fold in enumerate(folders):
-            ap_file = next(fold.glob('*ap.*bin'))
+            ap_file = next(fold.glob("*ap.*bin"))
             _shank_info = {}
 
-            _shank_info['ap_file'] = ap_file
+            _shank_info["ap_file"] = ap_file
             sr = spikeglx.Reader(ap_file)
-            sh = sr.meta.get(f'{self.np_version}_shank')
-            _shank_info['sr'] = sr
-            _shank_info['chns'] = self._get_chans(sr.meta)
-            assert all(_shank_info['chns'][:-1] == np.where(chn_info['shank'] == sh)[0])
-            shank_info[f'shank{iF}'] = _shank_info
+            sh = sr.meta.get(f"{self.np_version}_shank")
+            _shank_info["sr"] = sr
+            _shank_info["chns"] = self._get_chans(sr.meta)
+            assert all(_shank_info["chns"][:-1] == np.where(chn_info["shank"] == sh)[0])
+            shank_info[f"shank{iF}"] = _shank_info
 
         return shank_info
 
     def get_params(self):
         """
         Get some useful parameters for reconstructing file and metadata. This should only be called after _prepare_files
         :return:
         """
         self.fs_ap = 30000
-        self.nch = np.max(self.shank_info['shank0']['chns']) + 1
-        self.nsamples = self.shank_info['shank0']['sr'].ns
+        self.nch = np.max(self.shank_info["shank0"]["chns"]) + 1
+        self.nsamples = self.shank_info["shank0"]["sr"].ns
         self.samples_window = 2 * self.fs_ap
 
     def _get_chans(self, meta):
-        chn_subset = meta.get('snsSaveChanSubset_orig')
-        chn_subset = chn_subset.split(',')
+        chn_subset = meta.get("snsSaveChanSubset_orig")
+        chn_subset = chn_subset.split(",")
         for ich, ch_sub in enumerate(chn_subset):
-            sub = ch_sub.split(':')
+            sub = ch_sub.split(":")
             if len(sub) > 1:
                 chns = np.arange(int(sub[0]), int(sub[1]) + 1)
             else:
                 chns = np.array(int(sub[0]))
 
             if ich == 0:
                 chns_all = chns
@@ -862,62 +928,67 @@
 
     def _reconstruct(self):
         """
         Reconstructs the original file from the subshank files
         :return:
         """
 
-        file_out = open(self.save_file, 'wb')
+        file_out = open(self.save_file, "wb")
 
         wg = WindowGenerator(self.nsamples, self.samples_window, 0)
         for first, last in wg.firstlast:
             ns = int(last - first)
             chunk = np.zeros((ns, self.nch), dtype=np.int16)
             for ish, sh in enumerate(self.shank_info.keys()):
                 if ish == 0:
-                    chunk[:, self.shank_info[sh]['chns']] = self.shank_info[sh]['sr']._raw[first:last, :]
+                    chunk[:, self.shank_info[sh]["chns"]] = self.shank_info[sh][
+                        "sr"
+                    ]._raw[first:last, :]
                 else:
-                    chunk[:, self.shank_info[sh]['chns'][:-1]] = \
-                        self.shank_info[sh]['sr']._raw[first:last, :-1]
+                    chunk[:, self.shank_info[sh]["chns"][:-1]] = self.shank_info[sh][
+                        "sr"
+                    ]._raw[first:last, :-1]
 
             chunk.tofile(file_out)
 
         # close the sglx instances once we are done converting
         for sh in self.shank_info.keys():
-            sr = self.shank_info[sh].pop('sr')
+            sr = self.shank_info[sh].pop("sr")
             sr.close()
 
         file_out.close()
 
         return 1
 
     def write_metadata(self):
         """
         Write metadata for the original ap file. If it already exists and the file size matches, does not replace the original
         file
         :return:
         """
         # see if the meta file already exists
 
-        meta_file = self.save_file.with_suffix('.meta')
+        meta_file = self.save_file.with_suffix(".meta")
         if meta_file.exists():
             meta_info = spikeglx.read_meta_data(meta_file)
-            if meta_info['fileSizeBytes'] == self.save_file.stat().st_size:
+            if meta_info["fileSizeBytes"] == self.save_file.stat().st_size:
                 _logger.info('Meta file already present won"t overwrite')
                 return
 
         # First for the ap file
-        meta_shank = spikeglx.read_meta_data(self.shank_info['shank0']['ap_file'].with_suffix('.meta'))
-        meta_shank['acqApLfSy'][0] = self.nch - 1
-        meta_shank['snsApLfSy'][0] = self.nch - 1
-        meta_shank['nSavedChans'] = self.nch
-        meta_shank['fileSizeBytes'] = self.save_file.stat().st_size
-        meta_shank['snsSaveChanSubset'] = f'0:{self.nch - 1}'
-        _ = meta_shank.pop(f'{self.np_version}_shank')
-        _ = meta_shank.pop('snsSaveChanSubset_orig')
+        meta_shank = spikeglx.read_meta_data(
+            self.shank_info["shank0"]["ap_file"].with_suffix(".meta")
+        )
+        meta_shank["acqApLfSy"][0] = self.nch - 1
+        meta_shank["snsApLfSy"][0] = self.nch - 1
+        meta_shank["nSavedChans"] = self.nch
+        meta_shank["fileSizeBytes"] = self.save_file.stat().st_size
+        meta_shank["snsSaveChanSubset"] = f"0:{self.nch - 1}"
+        _ = meta_shank.pop(f"{self.np_version}_shank")
+        _ = meta_shank.pop("snsSaveChanSubset_orig")
 
         spikeglx.write_meta_data(meta_shank, meta_file)
 
     def compress_file(self, **kwargs):
         """
         Compress the reconstructed ap file
         :param kwargs:
```

### Comparing `ibl-neuropixel-0.9.2/src/spikeglx.py` & `ibl_neuropixel-1.0.0/src/spikeglx.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from iblutil.io import hashfile
 from iblutil.util import Bunch
 
 import neuropixel
 
 SAMPLE_SIZE = 2  # int16
 DEFAULT_BATCH_SIZE = 1e6
-_logger = logging.getLogger('ibllib')
+_logger = logging.getLogger("ibllib")
 
 
 class Reader:
     """
     Class for SpikeGLX reading purposes
     Some format description was found looking at the Matlab SDK here
     https://github.com/billkarsh/SpikeGLX/blob/master/MATLAB-SDK/DemoReadSGLXData.m
@@ -34,31 +34,51 @@
     usual sample 2 mv conversion factors (cf. neuropixel module):
         s2mv = 2.34375e-06 (NP1 ap banc) : default value used
         s2mv = 4.6875e-06 (NP1 lfp band)
 
     Note: To release system resources the close method must be called
     """
 
-    def __init__(self, sglx_file, open=True, nc=None, ns=None, fs=None, dtype='int16', s2v=None,
-                 nsync=None, ignore_warnings=False, meta_file=None, ch_file=None):
+    def __init__(
+        self,
+        sglx_file,
+        open=True,
+        nc=None,
+        ns=None,
+        fs=None,
+        dtype="int16",
+        s2v=None,
+        nsync=None,
+        ignore_warnings=False,
+        meta_file=None,
+        ch_file=None,
+    ):
         """
         An interface for reading data from a SpikeGLX file
         :param sglx_file: Path to a SpikeGLX file (compressed or otherwise), or to a meta-data file
         :param open: when True the file is opened
         """
         self.ignore_warnings = ignore_warnings
         sglx_file = Path(sglx_file)
-        meta_file = meta_file or sglx_file.with_suffix('.meta')
+        meta_file = meta_file or sglx_file.with_suffix(".meta")
         # only used if MTSCOMP compressed
         self.ch_file = ch_file
 
         if meta_file == sglx_file:
             # if a meta-data file is provided, try to get the binary file
-            self.file_bin = sglx_file.with_suffix('.cbin') if sglx_file.with_suffix('.cbin').exists() else None
-            self.file_bin = sglx_file.with_suffix('.bin') if sglx_file.with_suffix('.bin').exists() else None
+            self.file_bin = (
+                sglx_file.with_suffix(".cbin")
+                if sglx_file.with_suffix(".cbin").exists()
+                else None
+            )
+            self.file_bin = (
+                sglx_file.with_suffix(".bin")
+                if sglx_file.with_suffix(".bin").exists()
+                else None
+            )
         else:
             self.file_bin = sglx_file
         self.nbytes = self.file_bin.stat().st_size if self.file_bin else None
         self.dtype = np.dtype(dtype)
 
         if not meta_file.exists():
             # if no meta-data file is provided, try to get critical info from the binary file
@@ -70,67 +90,78 @@
             elif self.file_bin.stat().st_size / 385 % 2 == 0:
                 nc = nc or 385
                 ns = ns or self.file_bin.stat().st_size / 2 / 385
                 fs = fs or 30000
                 nsync = nsync or 1
 
             err_str = "Instantiating an Reader without meta data requires providing nc, fs and nc parameters"
-            assert (nc is not None and fs is not None and nc is not None), err_str
+            assert nc is not None and fs is not None and nc is not None, err_str
             self.file_meta_data = None
             self.meta = None
             self._nc, self._fs, self._ns = (int(nc), int(fs), int(ns))
             # handles default parameters: if int16 we assume it's a raw recording, we've checked the
             # multiple of the file size above to determine if there is a sync or not
             self._nsync = nsync or 0
             if s2v is None:
-                s2v = neuropixel.S2V_AP if self.dtype == np.dtype('int16') else 1.0
-            self.channel_conversion_sample2v = {'samples': np.ones(nc) * s2v}
+                s2v = neuropixel.S2V_AP if self.dtype == np.dtype("int16") else 1.0
+            self.channel_conversion_sample2v = {"samples": np.ones(nc) * s2v}
             if self._nsync > 0:
-                self.channel_conversion_sample2v['samples'][-nsync:] = 1
+                self.channel_conversion_sample2v["samples"][-nsync:] = 1
         else:
             # normal case we continue reading and interpreting the metadata file
             self.file_meta_data = meta_file
             self.meta = read_meta_data(meta_file)
             self.channel_conversion_sample2v = _conversion_sample2v_from_meta(self.meta)
             self._raw = None
         if open and self.file_bin:
             self.open()
 
     def open(self):
         # if we are not looking at a compressed file, use a memmap, otherwise instantiate mtscomp
         sglx_file = str(self.file_bin)
         if self.is_mtscomp:
             self._raw = mtscomp.Reader()
-            ch_file = self.ch_file or self.file_bin.with_suffix('.ch')
+            ch_file = self.ch_file or self.file_bin.with_suffix(".ch")
             self._raw.open(self.file_bin, ch_file)
             if self._raw.shape != (self.ns, self.nc):
                 ftsec = self._raw.shape[0] / self.fs
                 if not self.ignore_warnings:  # avoid the checks for streaming data
-                    _logger.warning(f"{sglx_file} : meta data and compressed chunks dont checkout\n"
-                                    f"File duration: expected {self.meta['fileTimeSecs']},"
-                                    f" actual {ftsec}\n"
-                                    f"Will attempt to fudge the meta-data information.")
-                self.meta['fileTimeSecs'] = ftsec
+                    _logger.warning(
+                        f"{sglx_file} : meta data and compressed chunks dont checkout\n"
+                        f"File duration: expected {self.meta['fileTimeSecs']},"
+                        f" actual {ftsec}\n"
+                        f"Will attempt to fudge the meta-data information."
+                    )
+                self.meta["fileTimeSecs"] = ftsec
         else:
             if self.nc * self.ns * self.dtype.itemsize != self.nbytes:
-                ftsec = self.file_bin.stat().st_size / self.dtype.itemsize / self.nc / self.fs
+                ftsec = (
+                    self.file_bin.stat().st_size
+                    / self.dtype.itemsize
+                    / self.nc
+                    / self.fs
+                )
                 if self.meta is not None:
                     if not self.ignore_warnings:
-                        _logger.warning(f"{sglx_file} : meta data and filesize do not checkout\n"
-                                        f"File size: expected {self.meta['fileSizeBytes']},"
-                                        f" actual {self.file_bin.stat().st_size}\n"
-                                        f"File duration: expected {self.meta['fileTimeSecs']},"
-                                        f" actual {ftsec}\n"
-                                        f"Will attempt to fudge the meta-data information.")
-                    self.meta['fileTimeSecs'] = ftsec
-            self._raw = np.memmap(sglx_file, dtype=self.dtype, mode='r', shape=(self.ns, self.nc))
+                        _logger.warning(
+                            f"{sglx_file} : meta data and filesize do not checkout\n"
+                            f"File size: expected {self.meta['fileSizeBytes']},"
+                            f" actual {self.file_bin.stat().st_size}\n"
+                            f"File duration: expected {self.meta['fileTimeSecs']},"
+                            f" actual {ftsec}\n"
+                            f"Will attempt to fudge the meta-data information."
+                        )
+                    self.meta["fileTimeSecs"] = ftsec
+            self._raw = np.memmap(
+                sglx_file, dtype=self.dtype, mode="r", shape=(self.ns, self.nc)
+            )
 
     def close(self):
         if self.is_open:
-            getattr(self._raw, '_mmap', self._raw).close()
+            getattr(self._raw, "_mmap", self._raw).close()
 
     def __enter__(self):
         if not self.is_open:
             self.open()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
@@ -160,68 +191,89 @@
 
     @property
     def is_open(self):
         return self._raw is not None
 
     @property
     def is_mtscomp(self):
-        return 'cbin' in self.file_bin.suffix
+        return "cbin" in self.file_bin.suffix
 
     @property
     def version(self):
         """Gets the version string: '3A', '3B2', '3B1', 'NP2.1', 'NP2.4'"""
-        return None if self.meta is None else _get_neuropixel_version_from_meta(self.meta)
+        return (
+            None if self.meta is None else _get_neuropixel_version_from_meta(self.meta)
+        )
 
     @property
     def major_version(self):
         """Gets the the major version int: 1 or 2"""
-        return None if self.meta is None else _get_neuropixel_major_version_from_meta(self.meta)
+        return (
+            None
+            if self.meta is None
+            else _get_neuropixel_major_version_from_meta(self.meta)
+        )
 
     @property
     def rl(self):
         return self.ns / self.fs
 
     @property
     def type(self):
-        """:return: ap, lf or nidq. Useful to index dictionaries """
+        """:return: ap, lf or nidq. Useful to index dictionaries"""
         if not self.meta:
-            return 'samples'
+            return "samples"
         return _get_type_from_meta(self.meta)
 
     @property
     def fs(self):
-        """ :return: sampling frequency (Hz) """
+        """:return: sampling frequency (Hz)"""
         return self._fs if self.meta is None else _get_fs_from_meta(self.meta)
 
     @property
     def nc(self):
-        """ :return: number of channels """
+        """:return: number of channels"""
         return self._nc if self.meta is None else _get_nchannels_from_meta(self.meta)
 
     @property
     def nsync(self):
         """:return: number of sync channels"""
-        return self._nsync if self.meta is None else len(_get_sync_trace_indices_from_meta(self.meta))
+        return (
+            self._nsync
+            if self.meta is None
+            else len(_get_sync_trace_indices_from_meta(self.meta))
+        )
 
     @property
     def ns(self):
-        """ :return: number of samples """
+        """:return: number of samples"""
         if self.meta is None:
             return self._ns
-        return int(np.round(self.meta.get('fileTimeSecs') * self.fs))
+        return int(np.round(self.meta.get("fileTimeSecs") * self.fs))
+
+    @property
+    def range_volts(self):
+        """
+        Returns the maximum voltage that can be recorded before saturation
+        :return: [nc, ] array of float32 (V)
+        """
+        if not self.meta:
+            return self.sample2volts * np.NaN
+        maxint = _get_max_int_from_meta(self.meta)
+        return self.sample2volts * maxint
 
     def read(self, nsel=slice(0, 10000), csel=slice(None), sync=True):
         """
         Read from slices or indexes
         :param slice_n: slice or sample indices
         :param slice_c: slice or channel indices
         :return: float32 array
         """
         if not self.is_open:
-            raise IOError('Reader not open; call `open` before `read`')
+            raise IOError("Reader not open; call `open` before `read`")
         darray = self._raw[nsel, csel].astype(np.float32, copy=True)
         darray *= self.channel_conversion_sample2v[self.type][csel]
         if sync:
             return darray, self.read_sync(nsel)
         else:
             return darray
 
@@ -242,18 +294,20 @@
 
     def read_sync_digital(self, _slice=slice(0, 10000)):
         """
         Reads only the digital sync trace at specified samples using slicing syntax
         >>> sync_samples = sr.read_sync_digital(slice(0,10000))
         """
         if not self.is_open:
-            raise IOError('Reader not open; call `open` before `read`')
+            raise IOError("Reader not open; call `open` before `read`")
         if not self.meta:
-            _logger.warning('Sync trace not labeled in metadata. Assuming last trace')
-        return split_sync(self._raw[_slice, _get_sync_trace_indices_from_meta(self.meta)])
+            _logger.warning("Sync trace not labeled in metadata. Assuming last trace")
+        return split_sync(
+            self._raw[_slice, _get_sync_trace_indices_from_meta(self.meta)]
+        )
 
     def read_sync_analog(self, _slice=slice(0, 10000)):
         """
         Reads only the analog sync traces at specified samples using slicing syntax
         >>> sync_samples = sr.read_sync_analog(slice(0,10000))
         """
         if not self.meta:
@@ -287,76 +341,88 @@
         """
         Compresses
         :param keep_original: defaults True. If False, the original uncompressed file is deleted
          and the current spikeglx.Reader object is modified in place
         :param kwargs:
         :return: pathlib.Path of the compressed *.cbin file
         """
-        file_tmp = self.file_bin.with_suffix('.cbin_tmp')
+        file_tmp = self.file_bin.with_suffix(".cbin_tmp")
         assert not self.is_mtscomp
-        mtscomp.compress(self.file_bin,
-                         out=file_tmp,
-                         outmeta=self.file_bin.with_suffix('.ch'),
-                         sample_rate=self.fs,
-                         n_channels=self.nc,
-                         dtype=self.dtype,
-                         **kwargs)
-        file_out = file_tmp.with_suffix('.cbin')
+        mtscomp.compress(
+            self.file_bin,
+            out=file_tmp,
+            outmeta=self.file_bin.with_suffix(".ch"),
+            sample_rate=self.fs,
+            n_channels=self.nc,
+            dtype=self.dtype,
+            **kwargs,
+        )
+        file_out = file_tmp.with_suffix(".cbin")
         file_tmp.rename(file_out)
         if not keep_original:
             self.file_bin.unlink()
             self.file_bin = file_out
         return file_out
 
     def decompress_file(self, keep_original=True, **kwargs):
         """
         Decompresses a mtscomp file
         :param keep_original: defaults True. If False, the original compressed file (input)
         is deleted and the current spikeglx.Reader object is modified in place
         NB: This is not equivalent to overwrite (which replaces the output file)
         :return: pathlib.Path of the decompressed *.bin file
         """
-        if 'out' not in kwargs:
-            kwargs['out'] = self.file_bin.with_suffix('.bin')
+        if "out" not in kwargs:
+            kwargs["out"] = self.file_bin.with_suffix(".bin")
         assert self.is_mtscomp
-        r = mtscomp.decompress(self.file_bin, self.file_bin.with_suffix('.ch'), **kwargs)
+        r = mtscomp.decompress(
+            self.file_bin, self.file_bin.with_suffix(".ch"), **kwargs
+        )
         r.close()
         if not keep_original:
             self.close()
             self.file_bin.unlink()
-            self.file_bin.with_suffix('.ch').unlink()
-            self.file_bin = kwargs['out']
-        return kwargs['out']
+            self.file_bin.with_suffix(".ch").unlink()
+            self.file_bin = kwargs["out"]
+        return kwargs["out"]
 
     def verify_hash(self):
         """
         Computes SHA-1 hash and returns True if it matches metadata, False otherwise
         :return: boolean
         """
         if self.is_mtscomp:
-            with open(self.file_bin.with_suffix('.ch')) as fid:
+            with open(self.file_bin.with_suffix(".ch")) as fid:
                 mtscomp_params = json.load(fid)
-            sm = mtscomp_params.get('sha1_compressed', None)
+            sm = mtscomp_params.get("sha1_compressed", None)
             if sm is None:
-                _logger.warning("SHA1 hash is not implemented for compressed ephys. To check "
-                                "the spikeglx acquisition hash, uncompress the file first !")
+                _logger.warning(
+                    "SHA1 hash is not implemented for compressed ephys. To check "
+                    "the spikeglx acquisition hash, uncompress the file first !"
+                )
                 return True
             sm = sm.upper()
         else:
             sm = self.meta.fileSHA1
         sc = hashfile.sha1(self.file_bin).upper()
         if sm == sc:
             log_func = _logger.info
         else:
             log_func = _logger.error
         log_func(f"SHA1 metadata: {sm}")
         log_func(f"SHA1 computed: {sc}")
         return sm == sc
 
 
+class OnlineReader(Reader):
+    @property
+    def ns(self):
+        return int(self.file_bin.stat().st_size / self.dtype.itemsize / self.nc)
+
+
 def read(sglx_file, first_sample=0, last_sample=10000):
     """
     Function to read from a spikeglx binary file without instantiating the class.
     Gets the meta-data as well.
 
     >>> ibllib.io.spikeglx.read('/path/to/file.bin', first_sample=0, last_sample=1000)
 
@@ -378,160 +444,181 @@
     :param md_file: last sample to be read, python slice-wise
     :return: Data array, sync trace, meta-data
     """
     with open(md_file) as fid:
         md = fid.read()
     d = {}
     for a in md.splitlines():
-        k, v = a.split('=', maxsplit=1)
+        k, v = a.split("=", maxsplit=1)
         # if all numbers, try to interpret the string
-        if v and re.fullmatch('[0-9,.]*', v) and v.count('.') < 2:
-            v = [float(val) for val in v.split(',')]
+        if v and re.fullmatch("[0-9,.]*", v) and v.count(".") < 2:
+            v = [float(val) for val in v.split(",")]
             # scalars should not be nested
             if len(v) == 1:
                 v = v[0]
         # tildes in keynames removed
-        d[k.replace('~', '')] = v
-    d['neuropixelVersion'] = _get_neuropixel_version_from_meta(d)
-    d['serial'] = _get_serial_number_from_meta(d)
+        d[k.replace("~", "")] = v
+    d["neuropixelVersion"] = _get_neuropixel_version_from_meta(d)
+    d["serial"] = _get_serial_number_from_meta(d)
     return Bunch(d)
 
 
 def write_meta_data(md, md_file):
     """
     Parses a dict into a spikeglx meta data file
     :param meta: meta data dict
     :param md_file: file to save meta data to
     :return:
     """
-    with open(md_file, 'w') as fid:
+    with open(md_file, "w") as fid:
         for key, val in md.items():
             if isinstance(val, list):
-                val = ','.join([str(int(v)) for v in val])
+                val = ",".join([str(int(v)) for v in val])
             if isinstance(val, float):
                 if val.is_integer():
                     val = int(val)
-            fid.write(f'{key}={val}\n')
+            fid.write(f"{key}={val}\n")
 
 
 def _get_savedChans_subset(chns):
     """
     Get the subset of the original channels that are saved per shank
     :param chns:
     :return:
     """
     chn_grps = np.r_[0, np.where(np.diff(chns) != 1)[0] + 1, len(chns)]
-    chn_subset = [f'{chns[chn_grps[i]]}:{chns[chn_grps[i + 1] - 1]}'
-                  if chn_grps[i] < len(chns) - 1 else f'{chns[chn_grps[i]]}'
-                  for i in range(len(chn_grps) - 1)]
+    chn_subset = [
+        f"{chns[chn_grps[i]]}:{chns[chn_grps[i + 1] - 1]}"
+        if chn_grps[i] < len(chns) - 1
+        else f"{chns[chn_grps[i]]}"
+        for i in range(len(chn_grps) - 1)
+    ]
 
-    return ','.join([sub for sub in chn_subset])
+    return ",".join([sub for sub in chn_subset])
 
 
 def _get_serial_number_from_meta(md):
     """
     Get neuropixel serial number from the metadata dictionary
     """
     # imProbeSN for 3A, imDatPrb_sn for 3B2, None for nidq 3B2
-    serial = md.get('imProbeSN') or md.get('imDatPrb_sn')
+    serial = md.get("imProbeSN") or md.get("imDatPrb_sn")
     if serial:
         return int(serial)
 
 
 def _get_neuropixel_major_version_from_meta(md):
-    MAJOR_VERSION = {'3A': 1, '3B2': 1, '3B1': 1, 'NP2.1': 2, 'NP2.4': 2.4}
+    MAJOR_VERSION = {"3A": 1, "3B2": 1, "3B1": 1, "NP2.1": 2, "NP2.4": 2.4}
     version = _get_neuropixel_version_from_meta(md)
     if version is not None:
         return MAJOR_VERSION[version]
 
 
+def _get_max_int_from_meta(md, neuropixel_version=None):
+    """
+    Gets the int value corresponding to the maximum voltage (range max)
+    :param md:
+    :param neuropixel_version:
+    :return:
+    """
+    # if this is an imec probe, this is electrophysiology and we assert the imMaxInt presence in NP2
+    if md.get("typeThis", None) == "imec":
+        neuropixel_version = neuropixel_version or _get_neuropixel_version_from_meta(md)
+        if "NP2" in neuropixel_version:
+            return int(md["imMaxInt"])  # usually 8192 but could be different
+        else:  # in case of NP1 it may not be in the header, but it has always been 512
+            return int(md.get("imMaxInt", 512))
+    else:  # this is a nidq device
+        return int(md.get("imMaxInt", 32768))
+
+
 def _get_neuropixel_version_from_meta(md):
     """
     Get neuropixel version tag (3A, 3B1, 3B2) from the metadata dictionary
     """
-    if 'typeEnabled' in md.keys():
-        return '3A'
-    prb_type = md.get('imDatPrb_type')
+    if "typeEnabled" in md.keys():
+        return "3A"
+    prb_type = md.get("imDatPrb_type")
     # Neuropixel 1.0 either 3B1 or 3B2 (ask Olivier about 3B1)
     if prb_type == 0:
-        if 'imDatPrb_port' in md.keys() and 'imDatPrb_slot' in md.keys():
-            return '3B2'
+        if "imDatPrb_port" in md.keys() and "imDatPrb_slot" in md.keys():
+            return "3B2"
         else:
-            return '3B1'
+            return "3B1"
     # Neuropixel 2.0 single shank
-    if prb_type == 21:
-        return 'NP2.1'
+    elif prb_type == 21:
+        return "NP2.1"
     # Neuropixel 2.0 four shank
-    if prb_type == 24:
-        return 'NP2.4'
+    elif prb_type == 24 or prb_type == 2013:
+        return "NP2.4"
 
 
 def _get_sync_trace_indices_from_meta(md):
     """
     Returns a list containing indices of the sync traces in the original array
     """
     typ = _get_type_from_meta(md)
     ntr = int(_get_nchannels_from_meta(md))
-    if typ == 'nidq':
-        nsync = int(md.get('snsMnMaXaDw')[-1])
-    elif typ in ['lf', 'ap']:
-        nsync = int(md.get('snsApLfSy')[2])
+    if typ == "nidq":
+        nsync = int(md.get("snsMnMaXaDw")[-1])
+    elif typ in ["lf", "ap"]:
+        nsync = int(md.get("snsApLfSy")[2])
     return list(range(ntr - nsync, ntr))
 
 
 def _get_analog_sync_trace_indices_from_meta(md):
     """
     Returns a list containing indices of the sync traces in the original array
     """
     typ = _get_type_from_meta(md)
-    if typ != 'nidq':
+    if typ != "nidq":
         return []
-    tr = md.get('snsMnMaXaDw')
+    tr = md.get("snsMnMaXaDw")
     nsa = int(tr[-2])
     return list(range(int(sum(tr[0:2])), int(sum(tr[0:2])) + nsa))
 
 
 def _get_nchannels_from_meta(md):
-    return int(md.get('nSavedChans'))
+    return int(md.get("nSavedChans"))
 
 
 def _get_nshanks_from_meta(md):
     th = _geometry_from_meta(md)
-    return len(np.unique(th['shank']))
+    return len(np.unique(th["shank"]))
 
 
 def _get_fs_from_meta(md):
-    if md.get('typeThis') == 'imec':
-        return md.get('imSampRate')
+    if md.get("typeThis") == "imec":
+        return md.get("imSampRate")
     else:
-        return md.get('niSampRate')
+        return md.get("niSampRate")
 
 
 def _get_type_from_meta(md):
     """
     Get neuropixel data type (ap, lf or nidq) from metadata
     """
-    snsApLfSy = md.get('snsApLfSy', [-1, -1, -1])
+    snsApLfSy = md.get("snsApLfSy", [-1, -1, -1])
     if snsApLfSy[0] == 0 and snsApLfSy[1] != 0:
-        return 'lf'
+        return "lf"
     elif snsApLfSy[0] != 0 and snsApLfSy[1] == 0:
-        return 'ap'
-    elif snsApLfSy == [-1, -1, -1] and md.get('typeThis', None) == 'nidq':
-        return 'nidq'
+        return "ap"
+    elif snsApLfSy == [-1, -1, -1] and md.get("typeThis", None) == "nidq":
+        return "nidq"
 
 
 def _split_geometry_into_shanks(th, meta_data):
     """
     Reduces the geometry information to that pertaining to specific shank
     :param th:
     :param meta_data:
     :return:
     """
-    if 'NP2.4_shank' in meta_data.keys():
-        shank_idx = np.where(th['shank'] == int(meta_data['NP2.4_shank']))[0]
+    if "NP2.4_shank" in meta_data.keys():
+        shank_idx = np.where(th["shank"] == int(meta_data["NP2.4_shank"]))[0]
         th = {key: th[key][shank_idx] for key in th.keys()}
 
     return th
 
 
 def _geometry_from_meta(meta_data):
     """
@@ -540,31 +627,37 @@
     :return: dictionary with keys 'row', 'col', 'ind', 'shank', 'adc', 'x', 'y', 'sample_shift'
     """
     cm = _map_channels_from_meta(meta_data)
     major_version = _get_neuropixel_major_version_from_meta(meta_data)
     if cm is None:
         _logger.warning("Meta data doesn't have geometry (snsShankMap/snsGeomMap field), returning defaults")
         th = neuropixel.trace_header(version=major_version)
-        th['flag'] = th['x'] * 0 + 1.
+        th["flag"] = th["x"] * 0 + 1.0
         return th
     th = cm.copy()
     # as of 2023-04 spikeglx stores only x, y coordinates of sites in UM and no col / row. Here
     # we convert to col / row for consistency with previous versions
-    if 'x' in cm.keys():
-        if major_version == 1:  # the spike sorting channel maps have a flipped version of the channel map
-            th['x'] = 70 - (th['x'])
-        th['y'] += 20  # there is a 20um offset between the probe tip and the first site in the coordinate conversion
-        th.update(neuropixel.xy2rc(th['x'], th['y'], version=major_version))
+    if "x" in cm.keys():
+        # the spike sorting channel maps have a flipped version of the channel map
+        # there is a 20um offset between the probe tip and the first site in the coordinate conversion
+        if major_version == 1:
+            th["x"] = 70 - (th["x"])
+
+        th["y"] += 20
+        th.update(neuropixel.xy2rc(th["x"], th["y"], version=major_version))
     else:
-        if major_version == 1:  # the spike sorting channel maps have a flipped version of the channel map
-            th['col'] = - cm['col'] * 2 + 2 + np.mod(cm['row'], 2)
-        th.update(neuropixel.rc2xy(th['row'], th['col'], version=major_version))
-    th['sample_shift'], th['adc'] = neuropixel.adc_shifts(version=major_version, nc=th['col'].size)
+        # the spike sorting channel maps have a flipped version of the channel map
+        if major_version == 1:
+            th["col"] = -cm["col"] * 2 + 2 + np.mod(cm["row"], 2)
+        th.update(neuropixel.rc2xy(th["row"], th["col"], version=major_version))
+    th["sample_shift"], th["adc"] = neuropixel.adc_shifts(
+        version=major_version, nc=th["col"].size
+    )
     th = _split_geometry_into_shanks(th, meta_data)
-    th['ind'] = np.arange(th['col'].size)
+    th["ind"] = np.arange(th["col"].size)
 
     return th
 
 
 def read_geometry(meta_file):
     """
     Reads the geometry
@@ -577,28 +670,28 @@
 def _map_channels_from_meta(meta_data):
     """
     Interpret the meta data string to extract an array of channel positions along the shank
 
     :param meta_data: dictionary output from  spikeglx.read_meta_data
     :return: dictionary of arrays 'shank', 'col', 'row', 'flag', one value per active site
     """
-    if 'snsShankMap' in meta_data.keys():
-        chmap = re.findall(r'([0-9]*:[0-9]*:[0-9]*:[0-9]*)', meta_data['snsShankMap'])
-        key_names = {'shank': 0, 'col': 1, 'row': 2, 'flag': 3}
-    elif 'snsGeomMap' in meta_data.keys():
-        chmap = re.findall(r'([0-9]*:[0-9]*:[0-9]*:[0-9]*)', meta_data['snsGeomMap'])
-        key_names = {'shank': 0, 'x': 1, 'y': 2, 'flag': 3}
+    if "snsShankMap" in meta_data.keys():
+        chmap = re.findall(r"([0-9]*:[0-9]*:[0-9]*:[0-9]*)", meta_data["snsShankMap"])
+        key_names = {"shank": 0, "col": 1, "row": 2, "flag": 3}
+    elif "snsGeomMap" in meta_data.keys():
+        chmap = re.findall(r"([0-9]*:[0-9]*:[0-9]*:[0-9]*)", meta_data["snsGeomMap"])
+        key_names = {"shank": 0, "x": 1, "y": 2, "flag": 3}
     else:
         return None
     # for digital nidq types, the key exists but does not contain any information
     if not chmap:
-        return {'shank': None, 'col': None, 'row': None, 'flag': None}
+        return {"shank": None, "col": None, "row": None, "flag": None}
     # shank#, col#, row#, drawflag
     # (nb: drawflag is one should be drawn and considered spatial average)
-    chmap = np.array([np.float32(cm.split(':')) for cm in chmap])
+    chmap = np.array([np.float32(cm.split(":")) for cm in chmap])
     return {k: chmap[:, v] for (k, v) in key_names.items()}
 
 
 def _conversion_sample2v_from_meta(meta_data):
     """
     Interpret the meta data to extract an array of conversion factors for each channel
     so the output data is in Volts
@@ -607,54 +700,93 @@
     For Nidq, repmat the gains from the trace counts in `snsMnMaXaDw`
 
     :param meta_data: dictionary output from  spikeglx.read_meta_data
     :return: numpy array with one gain value per channel
     """
 
     def int2volts(md):
-        """ :return: Conversion scalar to Volts. Needs to be combined with channel gains """
-        if md.get('typeThis', None) == 'imec':
-            if 'imMaxInt' in md:
-                return md.get('imAiRangeMax') / int(md['imMaxInt'])
-            else:
-                return md.get('imAiRangeMax') / 512
+        """:return: Conversion scalar to Volts. Needs to be combined with channel gains"""
+        maxint = _get_max_int_from_meta(md)
+        if md.get("typeThis", None) == "imec":
+            return md.get("imAiRangeMax") / maxint
         else:
-            return md.get('niAiRangeMax') / 32768
+            return md.get("niAiRangeMax") / maxint
 
     int2volt = int2volts(meta_data)
     version = _get_neuropixel_version_from_meta(meta_data)
     # interprets the gain value from the metadata header:
-    if 'imroTbl' in meta_data.keys():  # binary from the probes: ap or lf
-        sy_gain = np.ones(int(meta_data['snsApLfSy'][-1]), dtype=np.float32)
+    if "imroTbl" in meta_data.keys():  # binary from the probes: ap or lf
+        sy_gain = np.ones(int(meta_data["snsApLfSy"][-1]), dtype=np.float32)
         # imroTbl has 384 entries regardless of no of channels saved, so need to index by n_ch
-        # TODO need to look at snsSaveChanMap and index channels to get correct gain
-        n_chn = _get_nchannels_from_meta(meta_data) - len(_get_sync_trace_indices_from_meta(meta_data))
-        if 'NP2' in version:
+        n_chn = _get_nchannels_from_meta(meta_data) - len(
+            _get_sync_trace_indices_from_meta(meta_data)
+        )
+        if "NP2" in version:
             # NP 2.0; APGain = 80 for all AP
             # return 0 for LFgain (no LF channels)
-            out = {'lf': np.hstack((int2volt / 80 * np.ones(n_chn).astype(np.float32), sy_gain)),
-                   'ap': np.hstack((int2volt / 80 * np.ones(n_chn).astype(np.float32), sy_gain))}
+            out = {
+                "lf": np.hstack(
+                    (int2volt / 80 * np.ones(n_chn).astype(np.float32), sy_gain)
+                ),
+                "ap": np.hstack(
+                    (int2volt / 80 * np.ones(n_chn).astype(np.float32), sy_gain)
+                ),
+            }
         else:
             # the sync traces are not included in the gain values, so are included for
             # broadcast ops
-            gain = re.findall(r'([0-9]* [0-9]* [0-9]* [0-9]* [0-9]*)',
-                              meta_data['imroTbl'])[:n_chn]
-            out = {'lf': np.hstack((np.array([1 / np.float32(g.split(' ')[-1]) for g in gain]) *
-                                    int2volt, sy_gain)),
-                   'ap': np.hstack((np.array([1 / np.float32(g.split(' ')[-2]) for g in gain]) *
-                                    int2volt, sy_gain))}
+            gain = re.findall(
+                r"([0-9]* [0-9]* [0-9]* [0-9]* [0-9]*)", meta_data["imroTbl"]
+            )[:n_chn]
+            out = {
+                "lf": np.hstack(
+                    (
+                        np.array([1 / np.float32(g.split(" ")[-1]) for g in gain])
+                        * int2volt,
+                        sy_gain,
+                    )
+                ),
+                "ap": np.hstack(
+                    (
+                        np.array([1 / np.float32(g.split(" ")[-2]) for g in gain])
+                        * int2volt,
+                        sy_gain,
+                    )
+                ),
+            }
 
     # nidaq gain can be read in the same way regardless of NP1.0 or NP2.0
-    elif 'niMNGain' in meta_data.keys():  # binary from nidq
+    elif "niMNGain" in meta_data.keys():  # binary from nidq
         gain = np.r_[
-            np.ones(int(meta_data['snsMnMaXaDw'][0], )) / meta_data['niMNGain'] * int2volt,
-            np.ones(int(meta_data['snsMnMaXaDw'][1], )) / meta_data['niMAGain'] * int2volt,
-            np.ones(int(meta_data['snsMnMaXaDw'][2], )) * int2volt,  # no gain for analog sync
-            np.ones(int(np.sum(meta_data['snsMnMaXaDw'][3]), ))]  # no unit for digital sync
-        out = {'nidq': gain}
+            np.ones(
+                int(
+                    meta_data["snsMnMaXaDw"][0],
+                )
+            )
+            / meta_data["niMNGain"]
+            * int2volt,
+            np.ones(
+                int(
+                    meta_data["snsMnMaXaDw"][1],
+                )
+            )
+            / meta_data["niMAGain"]
+            * int2volt,
+            np.ones(
+                int(
+                    meta_data["snsMnMaXaDw"][2],
+                )
+            )
+            * int2volt,  # no gain for analog sync
+            np.ones(
+                int(
+                    np.sum(meta_data["snsMnMaXaDw"][3]),
+                )),
+        ]  # no unit for digital sync
+        out = {"nidq": gain}
 
     return out
 
 
 def split_sync(sync_tr):
     """
     The synchronization channels are stored as single bits, this will split the int16 original
@@ -666,38 +798,40 @@
     sync_tr = np.int16(np.copy(sync_tr))
     out = np.unpackbits(sync_tr.view(np.uint8)).reshape(sync_tr.size, 16)
     out = np.flip(np.roll(out, 8, axis=1), axis=1)
     return np.int8(out)
 
 
 def get_neuropixel_version_from_folder(session_path):
-    ephys_files = glob_ephys_files(session_path, ext='meta')
+    ephys_files = glob_ephys_files(session_path, ext="meta")
     return get_neuropixel_version_from_files(ephys_files)
 
 
 def get_neuropixel_version_from_files(ephys_files):
-    if any([ef.get('nidq') for ef in ephys_files]):
-        return '3B'
+    if any([ef.get("nidq") for ef in ephys_files]):
+        return "3B"
     else:
-        return '3A'
+        return "3A"
 
 
 def get_probes_from_folder(session_path):
     # should glob the ephys files and get out the labels
     # This assumes the meta files exist on the server (this is the case for now but should it be?)
-    ephys_files = glob_ephys_files(session_path, ext='meta')
+    ephys_files = glob_ephys_files(session_path, ext="meta")
     probes = []
     for files in ephys_files:
-        if files['label']:
-            probes.append(files['label'])
+        if files["label"]:
+            probes.append(files["label"])
 
     return probes
 
 
-def glob_ephys_files(session_path, suffix='.meta', ext='bin', recursive=True, bin_exists=True):
+def glob_ephys_files(
+    session_path, suffix=".meta", ext="bin", recursive=True, bin_exists=True
+):
     """
     From an arbitrary folder (usually session folder) gets the ap and lf files and labels
     Associated to the subfolders where they are
     the expected folder tree is:
     ├── 3A
     │   ├── imec0
     │   ├── sync_testing_g0_t0.imec0.ap.bin
@@ -717,124 +851,156 @@
     :param bin_exists:
     :param suffix:
     :param ext: file extension to look for, default 'bin' but could also be 'meta' or 'ch'
     :param recursive:
     :param session_path: folder, string or pathlib.Path
     :returns: a list of dictionaries with keys 'ap': apfile, 'lf': lffile and 'label'
     """
+
     def get_label(raw_ephys_apfile):
-        if raw_ephys_apfile.parts[-2] != 'raw_ephys_data':
+        if raw_ephys_apfile.parts[-2] != "raw_ephys_data":
             return raw_ephys_apfile.parts[-2]
         else:
-            return ''
+            return ""
 
-    recurse = '**/' if recursive else ''
+    recurse = "**/" if recursive else ""
     ephys_files = []
-    for raw_ephys_file in Path(session_path).glob(f'{recurse}*.ap*{suffix}'):
-        raw_ephys_apfile = next(raw_ephys_file.parent.glob(raw_ephys_file.stem + f'.*{ext}'), None)
+    for raw_ephys_file in Path(session_path).glob(f"{recurse}*.ap*{suffix}"):
+        raw_ephys_apfile = next(
+            raw_ephys_file.parent.glob(raw_ephys_file.stem + f".*{ext}"), None
+        )
         if not raw_ephys_apfile and bin_exists:
             continue
-        elif not raw_ephys_apfile and ext != 'bin':
+        elif not raw_ephys_apfile and ext != "bin":
             continue
-        elif not bin_exists and ext == 'bin':
-            raw_ephys_apfile = raw_ephys_file.with_suffix('.bin')
+        elif not bin_exists and ext == "bin":
+            raw_ephys_apfile = raw_ephys_file.with_suffix(".bin")
         # first get the ap file
-        ephys_files.extend([Bunch({'label': None, 'ap': None, 'lf': None, 'path': None})])
+        ephys_files.extend(
+            [Bunch({"label": None, "ap": None, "lf": None, "path": None})]
+        )
         ephys_files[-1].ap = raw_ephys_apfile
         # then get the corresponding lf file if it exists
-        lf_file = raw_ephys_apfile.parent / raw_ephys_apfile.name.replace('.ap.', '.lf.')
-        ephys_files[-1].lf = next(lf_file.parent.glob(lf_file.stem + f'.*{ext}'), None)
+        lf_file = raw_ephys_apfile.parent / raw_ephys_apfile.name.replace(
+            ".ap.", ".lf."
+        )
+        ephys_files[-1].lf = next(lf_file.parent.glob(lf_file.stem + f".*{ext}"), None)
         # finally, the label is the current directory except if it is bare in raw_ephys_data
         ephys_files[-1].label = get_label(raw_ephys_apfile)
         ephys_files[-1].path = raw_ephys_apfile.parent
     # for 3b probes, need also to get the nidq dataset type
-    for raw_ephys_file in Path(session_path).rglob(f'{recurse}*.nidq*{suffix}'):
-        raw_ephys_nidqfile = next(raw_ephys_file.parent.glob(raw_ephys_file.stem + f'.*{ext}'),
-                                  None)
-        if not bin_exists and ext == 'bin':
-            raw_ephys_nidqfile = raw_ephys_file.with_suffix('.bin')
-        ephys_files.extend([Bunch({'label': get_label(raw_ephys_file),
-                                   'nidq': raw_ephys_nidqfile,
-                                   'path': raw_ephys_file.parent})])
+    for raw_ephys_file in Path(session_path).rglob(f"{recurse}*.nidq*{suffix}"):
+        raw_ephys_nidqfile = next(
+            raw_ephys_file.parent.glob(raw_ephys_file.stem + f".*{ext}"), None
+        )
+        if not bin_exists and ext == "bin":
+            raw_ephys_nidqfile = raw_ephys_file.with_suffix(".bin")
+        ephys_files.extend(
+            [
+                Bunch(
+                    {
+                        "label": get_label(raw_ephys_file),
+                        "nidq": raw_ephys_nidqfile,
+                        "path": raw_ephys_file.parent,
+                    }
+                )
+            ]
+        )
     return ephys_files
 
 
-def _mock_spikeglx_file(mock_bin_file, meta_file, ns, nc, sync_depth,
-                        random=False, int2volts=0.6 / 32768, corrupt=False):
+def _mock_spikeglx_file(
+    mock_bin_file,
+    meta_file,
+    ns,
+    nc,
+    sync_depth,
+    random=False,
+    int2volts=0.6 / 32768,
+    corrupt=False,
+):
     """
     For testing purposes, create a binary file with sync pulses to test reading and extraction
     """
     meta_file = Path(meta_file)
     mock_path_bin = Path(mock_bin_file)
-    mock_path_meta = mock_path_bin.with_suffix('.meta')
+    mock_path_meta = mock_path_bin.with_suffix(".meta")
     md = read_meta_data(meta_file)
     assert meta_file != mock_path_meta
     fs = _get_fs_from_meta(md)
     fid_source = open(meta_file)
-    fid_target = open(mock_path_meta, 'w+')
+    fid_target = open(mock_path_meta, "w+")
     line = fid_source.readline()
     while line:
         line = fid_source.readline()
-        if line.startswith('fileSizeBytes'):
-            line = f'fileSizeBytes={ns * nc * 2}\n'
-        if line.startswith('fileTimeSecs'):
+        if line.startswith("fileSizeBytes"):
+            line = f"fileSizeBytes={ns * nc * 2}\n"
+        if line.startswith("fileTimeSecs"):
             if corrupt:
-                line = f'fileTimeSecs={ns / fs + 1.8324}\n'
+                line = f"fileTimeSecs={ns / fs + 1.8324}\n"
             else:
-                line = f'fileTimeSecs={ns / fs}\n'
+                line = f"fileTimeSecs={ns / fs}\n"
         fid_target.write(line)
     fid_source.close()
     fid_target.close()
     if random:
         D = np.random.randint(-32767, 32767, size=(ns, nc), dtype=np.int16)
     else:  # each channel as an int of chn + 1
         D = np.tile(np.int16((np.arange(nc) + 1) / int2volts), (ns, 1))
         D[0:16, :] = 0
     # the last channel is the sync that we fill with
     sync = np.int16(2 ** np.float32(np.arange(-1, sync_depth)))
     D[:, -1] = 0
-    D[:sync.size, -1] = sync
-    with open(mock_path_bin, 'w+') as fid:
+    D[: sync.size, -1] = sync
+    with open(mock_path_bin, "w+") as fid:
         D.tofile(fid)
-    return {'bin_file': mock_path_bin, 'ns': ns, 'nc': nc, 'sync_depth': sync_depth, 'D': D}
+    return {
+        "bin_file": mock_path_bin,
+        "ns": ns,
+        "nc": nc,
+        "sync_depth": sync_depth,
+        "D": D,
+    }
 
 
 def get_hardware_config(config_file):
     """
     Reads the neuropixel_wirings.json file containing sync mapping and parameters
     :param config_file: folder or json file
     :return: dictionary or None
     """
     config_file = Path(config_file)
     if config_file.is_dir():
-        config_file = list(config_file.glob('*.wiring*.json'))
+        config_file = list(config_file.glob("*.wiring*.json"))
         if config_file:
             config_file = config_file[0]
     if not config_file or not config_file.exists():
         return
     with open(config_file) as fid:
         par = json.loads(fid.read())
     return par
 
 
 def _sync_map_from_hardware_config(hardware_config):
     """
     :param hardware_config: dictonary from json read of neuropixel_wirings.json
     :return: dictionary where key names refer to object and values to sync channel index
     """
-    if hardware_config['SYSTEM'] == '3A' or hardware_config['SYSTEM'] == '3B':
-        pin_out = neuropixel.SYNC_PIN_OUT[hardware_config['SYSTEM']]
-        sync_map = {hardware_config['SYNC_WIRING_DIGITAL'][pin]: pin_out[pin]
-                    for pin in hardware_config['SYNC_WIRING_DIGITAL']
-                    if pin_out[pin] is not None}
+    if hardware_config["SYSTEM"] == "3A" or hardware_config["SYSTEM"] == "3B":
+        pin_out = neuropixel.SYNC_PIN_OUT[hardware_config["SYSTEM"]]
+        sync_map = {
+            hardware_config["SYNC_WIRING_DIGITAL"][pin]: pin_out[pin]
+            for pin in hardware_config["SYNC_WIRING_DIGITAL"]
+            if pin_out[pin] is not None
+        }
     else:
-        digital = hardware_config.get('SYNC_WIRING_DIGITAL')
+        digital = hardware_config.get("SYNC_WIRING_DIGITAL")
         sync_map = {digital[pin]: int(pin[3:]) for pin in digital}
 
-    analog = hardware_config.get('SYNC_WIRING_ANALOG')
+    analog = hardware_config.get("SYNC_WIRING_ANALOG")
     if analog:
         sync_map.update({analog[pin]: int(pin[2:]) + 16 for pin in analog})
     return sync_map
 
 
 def get_sync_map(folder_ephys):
     hc = get_hardware_config(folder_ephys)
```

