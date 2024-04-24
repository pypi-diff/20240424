# Comparing `tmp/thunderfish-1.9.9.tar.gz` & `tmp/thunderfish-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunderfish-1.9.9.tar", last modified: Sun Jan 23 20:03:50 2022, max compression
+gzip compressed data, was "thunderfish-2.0.0.tar", last modified: Wed Apr 24 10:06:05 2024, max compression
```

## Comparing `thunderfish-1.9.9.tar` & `thunderfish-2.0.0.tar`

### file list

```diff
@@ -1,44 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-23 20:03:50.541985 thunderfish-1.9.9/
--rw-r--r--   0 root         (0) root         (0)    35141 2018-10-26 17:47:52.000000 thunderfish-1.9.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1483 2022-01-23 20:03:50.541985 thunderfish-1.9.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3635 2022-01-21 23:05:06.000000 thunderfish-1.9.9/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-01-23 20:03:50.541985 thunderfish-1.9.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2248 2022-01-16 15:31:13.000000 thunderfish-1.9.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-23 20:03:50.533984 thunderfish-1.9.9/thunderfish/
--rw-r--r--   0 root         (0) root         (0)      543 2022-01-21 23:05:28.000000 thunderfish-1.9.9/thunderfish/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34058 2022-01-22 18:02:07.000000 thunderfish-1.9.9/thunderfish/bestwindow.py
--rw-r--r--   0 root         (0) root         (0)     6874 2021-02-10 22:00:12.000000 thunderfish-1.9.9/thunderfish/checkpulse.py
--rw-r--r--   0 root         (0) root         (0)     8886 2021-02-10 22:01:06.000000 thunderfish-1.9.9/thunderfish/chirp.py
--rw-rw-r--   0 root         (0) root         (0)    26732 2022-01-22 22:11:17.000000 thunderfish-1.9.9/thunderfish/collectfish.py
--rw-r--r--   0 root         (0) root         (0)    13438 2020-07-17 07:30:39.000000 thunderfish-1.9.9/thunderfish/configfile.py
--rw-r--r--   0 root         (0) root         (0)     7555 2021-02-10 22:02:17.000000 thunderfish-1.9.9/thunderfish/consistentfishes.py
--rw-r--r--   0 root         (0) root         (0)     3334 2021-02-10 22:03:50.000000 thunderfish-1.9.9/thunderfish/consoleinput.py
--rw-r--r--   0 root         (0) root         (0)    41902 2022-01-21 23:23:46.000000 thunderfish-1.9.9/thunderfish/dataloader.py
--rw-rw-r--   0 root         (0) root         (0)    12342 2022-01-22 08:22:56.000000 thunderfish-1.9.9/thunderfish/datawriter.py
--rw-r--r--   0 root         (0) root         (0)    21585 2021-07-13 20:24:48.000000 thunderfish-1.9.9/thunderfish/efield.py
--rw-rw-r--   0 root         (0) root         (0)   102281 2022-01-22 23:04:00.000000 thunderfish-1.9.9/thunderfish/eodanalysis.py
--rw-rw-r--   0 root         (0) root         (0)    34055 2022-01-22 17:21:52.000000 thunderfish-1.9.9/thunderfish/eodexplorer.py
--rw-r--r--   0 root         (0) root         (0)    44408 2018-11-11 23:04:06.000000 thunderfish-1.9.9/thunderfish/eventdetection-fast.py
--rw-rw-r--   0 root         (0) root         (0)    51084 2021-12-07 20:23:28.000000 thunderfish-1.9.9/thunderfish/eventdetection.py
--rw-r--r--   0 root         (0) root         (0)    33905 2021-10-01 20:54:11.000000 thunderfish-1.9.9/thunderfish/fakefish.py
--rw-rw-r--   0 root         (0) root         (0)    36276 2022-01-22 16:38:55.000000 thunderfish-1.9.9/thunderfish/fishfinder.py
--rw-r--r--   0 root         (0) root         (0)    42376 2021-02-17 09:02:53.000000 thunderfish-1.9.9/thunderfish/fishshapes.py
--rw-rw-r--   0 root         (0) root         (0)    69964 2022-01-18 17:45:02.000000 thunderfish-1.9.9/thunderfish/harmonics.py
--rw-r--r--   0 root         (0) root         (0)    56951 2021-12-15 21:28:56.000000 thunderfish-1.9.9/thunderfish/multivariateexplorer.py
--rw-r--r--   0 root         (0) root         (0)    18828 2021-02-10 21:52:39.000000 thunderfish-1.9.9/thunderfish/powerspectrum.py
--rw-r--r--   0 root         (0) root         (0)    38088 2022-01-18 17:47:34.000000 thunderfish-1.9.9/thunderfish/pulseplots.py
--rw-rw-r--   0 root         (0) root         (0)    80899 2022-01-20 22:08:03.000000 thunderfish-1.9.9/thunderfish/pulses.py
--rw-r--r--   0 root         (0) root         (0)    41161 2021-02-10 22:58:50.000000 thunderfish-1.9.9/thunderfish/pulsetracker.py
--rw-rw-r--   0 root         (0) root         (0)   111330 2021-12-23 21:39:52.000000 thunderfish-1.9.9/thunderfish/tabledata.py
--rw-rw-r--   0 root         (0) root         (0)    12665 2022-01-22 11:27:35.000000 thunderfish-1.9.9/thunderfish/thunderbrowse.py
--rw-rw-r--   0 root         (0) root         (0)    61554 2022-01-22 22:56:43.000000 thunderfish-1.9.9/thunderfish/thunderfish.py
--rw-rw-r--   0 root         (0) root         (0)    35789 2022-01-22 16:40:01.000000 thunderfish-1.9.9/thunderfish/thunderlogger.py
--rw-rw-r--   0 root         (0) root         (0)      210 2022-01-18 17:46:02.000000 thunderfish-1.9.9/thunderfish/version.py
--rw-r--r--   0 root         (0) root         (0)    44954 2021-02-10 22:56:41.000000 thunderfish-1.9.9/thunderfish/voronoi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-23 20:03:50.537984 thunderfish-1.9.9/thunderfish.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1483 2022-01-23 20:03:50.000000 thunderfish-1.9.9/thunderfish.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1039 2022-01-23 20:03:50.000000 thunderfish-1.9.9/thunderfish.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-23 20:03:50.000000 thunderfish-1.9.9/thunderfish.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      283 2022-01-23 20:03:50.000000 thunderfish-1.9.9/thunderfish.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       39 2022-01-23 20:03:50.000000 thunderfish-1.9.9/thunderfish.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-01-23 20:03:50.000000 thunderfish-1.9.9/thunderfish.egg-info/top_level.txt
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-24 10:06:05.175521 thunderfish-2.0.0/
+-rw-rw-r--   0 benda     (1001) benda     (1001)    35141 2020-05-14 11:55:11.000000 thunderfish-2.0.0/LICENSE
+-rw-r--r--   0 benda     (1001) benda     (1001)    46515 2024-04-24 10:06:05.175521 thunderfish-2.0.0/PKG-INFO
+-rw-rw-r--   0 benda     (1001) benda     (1001)     4575 2024-04-24 10:05:07.000000 thunderfish-2.0.0/README.md
+-rw-rw-r--   0 benda     (1001) benda     (1001)     1922 2024-04-24 09:56:20.000000 thunderfish-2.0.0/pyproject.toml
+-rw-rw-r--   0 benda     (1001) benda     (1001)       38 2024-04-24 10:06:05.175521 thunderfish-2.0.0/setup.cfg
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-24 10:06:05.171521 thunderfish-2.0.0/src/
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-24 10:06:05.175521 thunderfish-2.0.0/src/thunderfish/
+-rw-rw-r--   0 benda     (1001) benda     (1001)      774 2024-04-22 08:52:35.000000 thunderfish-2.0.0/src/thunderfish/__init__.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    34262 2024-04-24 09:56:20.000000 thunderfish-2.0.0/src/thunderfish/bestwindow.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     6899 2024-04-24 09:56:20.000000 thunderfish-2.0.0/src/thunderfish/checkpulse.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     8922 2024-04-24 09:56:20.000000 thunderfish-2.0.0/src/thunderfish/chirp.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    28161 2024-04-24 09:56:20.000000 thunderfish-2.0.0/src/thunderfish/collectfish.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     7555 2024-04-22 08:52:35.000000 thunderfish-2.0.0/src/thunderfish/consistentfishes.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    21574 2024-04-22 08:52:35.000000 thunderfish-2.0.0/src/thunderfish/efield.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)   121901 2024-04-24 09:56:20.000000 thunderfish-2.0.0/src/thunderfish/eodanalysis.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    34220 2024-04-24 09:56:20.000000 thunderfish-2.0.0/src/thunderfish/eodexplorer.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    34921 2024-04-24 09:56:20.000000 thunderfish-2.0.0/src/thunderfish/fakefish.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    36313 2024-04-24 09:56:20.000000 thunderfish-2.0.0/src/thunderfish/fishfinder.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    47932 2024-04-22 08:52:35.000000 thunderfish-2.0.0/src/thunderfish/fishshapes.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    70677 2024-04-24 09:56:20.000000 thunderfish-2.0.0/src/thunderfish/harmonics.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     4585 2024-04-22 08:52:35.000000 thunderfish-2.0.0/src/thunderfish/hopkinsloader.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    38088 2024-04-22 08:52:35.000000 thunderfish-2.0.0/src/thunderfish/pulseplots.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    81476 2024-04-24 09:56:20.000000 thunderfish-2.0.0/src/thunderfish/pulses.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    41112 2024-04-24 09:56:20.000000 thunderfish-2.0.0/src/thunderfish/pulsetracker.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    38456 2024-04-24 09:56:20.000000 thunderfish-2.0.0/src/thunderfish/thunderbrowse.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    72308 2024-04-24 09:56:20.000000 thunderfish-2.0.0/src/thunderfish/thunderfish.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    35832 2024-04-24 09:56:20.000000 thunderfish-2.0.0/src/thunderfish/thunderlogger.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)      206 2024-04-22 08:52:35.000000 thunderfish-2.0.0/src/thunderfish/version.py
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-24 10:06:05.175521 thunderfish-2.0.0/src/thunderfish.egg-info/
+-rw-r--r--   0 benda     (1001) benda     (1001)    46515 2024-04-24 10:06:05.000000 thunderfish-2.0.0/src/thunderfish.egg-info/PKG-INFO
+-rw-rw-r--   0 benda     (1001) benda     (1001)     1021 2024-04-24 10:06:05.000000 thunderfish-2.0.0/src/thunderfish.egg-info/SOURCES.txt
+-rw-rw-r--   0 benda     (1001) benda     (1001)        1 2024-04-24 10:06:05.000000 thunderfish-2.0.0/src/thunderfish.egg-info/dependency_links.txt
+-rw-rw-r--   0 benda     (1001) benda     (1001)      282 2024-04-24 10:06:05.000000 thunderfish-2.0.0/src/thunderfish.egg-info/entry_points.txt
+-rw-rw-r--   0 benda     (1001) benda     (1001)       47 2024-04-24 10:06:05.000000 thunderfish-2.0.0/src/thunderfish.egg-info/requires.txt
+-rw-rw-r--   0 benda     (1001) benda     (1001)       12 2024-04-24 10:06:05.000000 thunderfish-2.0.0/src/thunderfish.egg-info/top_level.txt
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-24 10:06:05.175521 thunderfish-2.0.0/tests/
+-rw-rw-r--   0 benda     (1001) benda     (1001)     3585 2024-04-24 09:56:20.000000 thunderfish-2.0.0/tests/test_bestwindow.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     1301 2024-04-24 09:56:20.000000 thunderfish-2.0.0/tests/test_eodanalysis.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     4791 2024-04-16 15:47:02.000000 thunderfish-2.0.0/tests/test_fakefish.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     7414 2024-04-16 15:47:14.000000 thunderfish-2.0.0/tests/test_fishshapes.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     2161 2024-04-24 09:56:20.000000 thunderfish-2.0.0/tests/test_harmonics.py
```

### Comparing `thunderfish-1.9.9/LICENSE` & `thunderfish-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thunderfish-1.9.9/thunderfish/bestwindow.py` & `thunderfish-2.0.0/src/thunderfish/bestwindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 ## Visualization
 - `plot_clipping()`: visualization of the algorithm for detecting clipped amplitudes in `clip_amplitudes()`.
 - `plot_best_window()`: visualization of the algorithm used in `best_window_indices()`.
 - `plot_data_window()`: plot the data and the selected analysis window.
 """
 
 import numpy as np
-from .eventdetection import percentile_threshold, detect_peaks, trim_to_peak
-from audioio.audioloader import unwrap
+from thunderlab.eventdetection import percentile_threshold, detect_peaks, trim_to_peak
+from audioio import unwrap
 try:
     import matplotlib.pyplot as plt
     import matplotlib.ticker as ticker
 except ImportError:
     pass
 
 
@@ -114,24 +114,23 @@
 
 def plot_clipping(data, winx0, winx1, bins,
                   h, min_clip, max_clip, min_ampl, max_ampl):
     """Visualize the data histograms and the detected clipping amplitudes.
 
     Pass this function as the `plot_hist_func` argument to `clip_amplitudes()`.
     """
-    plt.subplot(2, 1, 1)
-    plt.plot(data[winx0:winx1], 'b')
-    plt.axhline(min_clip, color='r')
-    plt.axhline(max_clip, color='r')
-    plt.ylim(-1.0, 1.0)
-    plt.subplot(2, 1, 2)
-    plt.bar(bins[:-1], h, width=np.mean(np.diff(bins)))
-    plt.axvline(min_clip, color='r')
-    plt.axvline(max_clip, color='r')
-    plt.xlim(-1.0, 1.0)
+    fig, (ax1, ax2) = plt.subplots(2, 1)
+    ax1.plot(data[winx0:winx1], 'b')
+    ax1.axhline(min_clip, color='r')
+    ax1.axhline(max_clip, color='r')
+    ax1.set_ylim(-1.0, 1.0)
+    ax2.bar(bins[:-1], h, width=np.mean(np.diff(bins)))
+    ax2.axvline(min_clip, color='r')
+    ax2.axvline(max_clip, color='r')
+    ax2.set_xlim(-1.0, 1.0)
     plt.show()
 
 
 def add_clip_config(cfg, min_clip=0.0, max_clip=0.0,
                     window=1.0, min_fac=2.0, nbins=20,
                     min_ampl=-1.0, max_ampl=1.0):
     """Add parameter needed for `clip_amplitudes()` as a new section to a configuration.
@@ -142,17 +141,15 @@
         The configuration.
     min_clip: float
         Default minimum clip amplitude.
     max_clip: float
         Default maximum clip amplitude.
         
     See `clip_amplitudes()` for details on the remaining arguments.
-
     """
-
     cfg.add_section('Clipping amplitudes:')
     cfg.add('minClipAmplitude', min_clip, '', 'Minimum amplitude that is not clipped. If zero estimate from data.')
     cfg.add('maxClipAmplitude', max_clip, '', 'Maximum amplitude that is not clipped. If zero estimate from data.')
     cfg.add('clipWindow', window, 's', 'Window size for estimating clip amplitudes.')
     cfg.add('clipBins', nbins, '', 'Number of bins used for constructing histograms of signal amplitudes.')
     cfg.add('minClipFactor', min_fac, '',
             'Edge bins of the histogram of clipped signals have to be larger then their neighbors by this factor.')
@@ -174,15 +171,14 @@
         The sampling rate of the data.
 
     Returns
     -------
     a: dict
         Dictionary with names of arguments of the `clip_amplitudes()` function
         and their values as supplied by `cfg`.
-
     """
     a = cfg.map({'min_fac': 'minClipFactor',
                  'nbins': 'clipBins',
                  'min_ampl': 'minDataAmplitude',
                  'max_ampl': 'maxDataAmplitude'})
     a['win_indices'] = int(cfg.value('clipWindow') * rate)
     return a
@@ -195,15 +191,15 @@
     """Find the window within data most suitable for subsequent analysis.
     
     First, large peaks and troughs of the data are detected.  Peaks and
     troughs have to be separated in amplitude by at least the value of a
     dynamic threshold.  The threshold is computed in `win_shift` wide
     windows as `thresh_fac` times the interpercentile range at
     the `percentile`-th and 100.0-`percentile`-th percentile of the data
-    using the `eventdetection.percentile_threshold()` function.
+    using the `thunderlab.eventdetection.percentile_threshold()` function.
 
     Second, criteria for selecting the best window are computed for each
     window of width `win_size` shifted by `win_shift` trough the data. The
     three criteria are:
 
     - the mean peak-to-trough amplitude multiplied with the fraction of
       non clipped peak and trough amplitudes.
@@ -237,18 +233,18 @@
         plus tolerance.
     win_size: float
         Minimum size of the desired best window in seconds.
         Choose it large enough for the subsequent analysis.
     win_shift: float
         Time shift in seconds between windows. Should be smaller or equal to `win_size`.
     percentile: float
-        `percentile` parameter for the `eventdetection.percentile_threshold()` function
+        `percentile` parameter for the `thunderlab.eventdetection.percentile_threshold()` function
         used to estimate thresholds for detecting peaks in the data.
     thresh_fac: float
-        `thresh_fac` parameter for the `eventdetection.percentile_threshold()` function
+        `thresh_fac` parameter for the `thunderlab.eventdetection.percentile_threshold()` function
         used to estimate thresholds for detecting peaks in the data.
     min_clip: float
         Minimum amplitude below which data are clipped.
     max_clip: float
         Maximum amplitude above which data are clipped.
     w_cv_interv: float
         Weight for the coefficient of variation of the intervals between detected
@@ -312,19 +308,18 @@
         - No peaks detected.
         - No finite amplitudes detected.
         - No valid interval CV detected.
         - No valid amplitude CV detected.
     """
     # too little data:
     if len(data) / samplerate < win_size:
-        raise UserWarning('not enough data (data=%gs, win=%gs)' %
-                          (len(data) / samplerate, win_size))
+        raise UserWarning(f'not enough data (data={len(data) / samplerate:g}s, win={win_size:g}s)')
 
     # threshold for peak detection:
-    threshold = percentile_threshold(data, samplerate, win_shift,
+    threshold = percentile_threshold(data, int(win_shift*samplerate),
                                      thresh_fac=thresh_fac,
                                      percentile=percentile)
 
     # detect large peaks and troughs:
     peak_idx, trough_idx = detect_peaks(data, threshold)
     if len(peak_idx) == 0 or len(trough_idx) == 0:
         raise UserWarning('no peaks or troughs detected')
@@ -476,15 +471,14 @@
     """Visualize the cost function of used for finding the best window for analysis.
 
     Pass this function as the `plot_data_func` to the `best_window_*` functions.
 
     Parameters
     ----------
     See documentation of the `best_window_indices()` functions.
-
     """
     # raw data:
     time = np.arange(0.0, len(data)) / rate
     ax[0].plot(time, data, 'b', lw=3)
     if np.mean(clipped_frac[win_idx0:win_idx1]) > 0.01:
         ax[0].plot(time[idx0:idx1], data[idx0:idx1], color='magenta', lw=3)
     else:
@@ -559,22 +553,22 @@
     time = np.arange(len(data)) / samplerate
     ax.plot(time[:idx0], data[:idx0], color=data_color)
     ax.plot(time[idx1:], data[idx1:], color=data_color)
     if idx1 > idx0:
         ax.plot(time[idx0:idx1], data[idx0:idx1], color=window_color)
         label = 'analysis\nwindow'
         if clipped > 0.0:
-            label += '\n%.0f%% clipped' % (100.0*clipped)
+            label += f'\n{100.0*clipped:.0f}% clipped'
         ax.text(time[(idx0+idx1)//2], 0.0, label, ha='center', va='center')
     ax.set_xlim(time[0], time[-1])
     ax.set_xlabel('Time [sec]')
     if len(unit) == 0 or unit == 'a.u.':
         ax.set_ylabel('Amplitude')
     else:
-        ax.set_ylabel('Amplitude [%s]' % unit)
+        ax.set_ylabel(f'Amplitude [{unit}]')
     ax.yaxis.set_major_locator(ticker.MaxNLocator(3))
 
         
 def add_best_window_config(cfg, win_pos='best', win_size=1., win_shift=0.5,
                            thresh_fac=0.8, percentile=0.1,
                            min_clip=-np.inf, max_clip=np.inf,
                            w_cv_interv=1.0, w_ampl=1.0, w_cv_ampl=1.0,
@@ -584,15 +578,14 @@
     Parameters
     ----------
     cfg: ConfigFile
         The configuration.
         
     See `best_window_indices()` for details on the remaining arguments.
     """
-
     cfg.add_section('Analysis window:')
     cfg.add('windowPosition', win_pos, '', 'Position of the analysis window: "beginning", "center", "end", "best", or a time in seconds.')
     cfg.add('windowSize', win_size, 's', 'Size of the best window. This should be much larger than the expected period of the signal. If 0 select the whole time series.')
     cfg.add('bestWindowShift', win_shift, 's',
             'Increment for shifting the analysis windows trough the data. Should be larger than the expected period of the signal.')
     cfg.add('bestWindowThresholdPercentile', percentile, '%',
             'Percentile for estimating interpercentile range. Should be smaller than the duty cycle of the periodic signal.')
@@ -634,23 +627,26 @@
                     'w_cv_interv': 'weightCVInterval',
                     'w_ampl': 'weightAmplitude',
                     'w_cv_ampl': 'weightCVAmplitude',
                     'tolerance': 'bestWindowTolerance',
                     'expand': 'expandBestWindow'})
 
         
-def analysis_window(data, samplerate, win_pos, cfg, show_bestwindow=False):
+def analysis_window(data, samplerate, ampl_max, win_pos,
+                    cfg, show_bestwindow=False):
     """Set clipping amplitudes and find analysis window.
 
     Parameters
     ----------
     data: 1-D array
         The data to be analyzed.
     samplerate: float
         Sampling rate of the data in Hertz.
+    ampl_max: float
+        Maximum value of input range.
     win_pos: string or float
         Position of the analysis window: "beginning", "center", "end" or "best".
         Alternatively the beginning of the analysis window in seconds.
     cfg: ConfigFile
         Configuration for clipping and best window.
     show_bestwindow: boolean
         If true show a plot with the best window cost functions.
@@ -673,15 +669,15 @@
     found_bestwindow = True
     min_clip = cfg.value('minClipAmplitude')
     max_clip = cfg.value('maxClipAmplitude')
     clipped = 0
     if min_clip == 0.0 or max_clip == 0.0:
         min_clip, max_clip = clip_amplitudes(data, **clip_args(cfg, samplerate))
     if cfg.value('unwrapData'):
-        data = unwrap(data)
+        unwrap(data, 1.5, ampl_max)
         min_clip *= 2
         max_clip *= 2
     # window size parameter:
     bwa = best_window_args(cfg)
     if 'win_size' in bwa:
         del bwa['win_size']
     window_size = cfg.value('windowSize')
@@ -733,74 +729,77 @@
             if not found_bestwindow or idx1 > len(data):
                 return data, 0, 0, False, min_clip, max_clip
             data_seg = data[idx0:idx1]
             # check for clipping:
             win_shift = cfg.value('bestWindowShift')
             thresh_fac = cfg.value('bestWindowThresholdFactor')
             percentile = cfg.value('bestWindowThresholdPercentile')
-            threshold = percentile_threshold(data_seg, samplerate,
-                                             win_shift, thresh_fac=thresh_fac,
+            threshold = percentile_threshold(data_seg,
+                                             int(win_shift*samplerate),
+                                             thresh_fac=thresh_fac,
                                              percentile=percentile)
             peak_idx, trough_idx = detect_peaks(data_seg, threshold)
             p_idx, t_idx = trim_to_peak(peak_idx, trough_idx)
             if len(p_idx) > 0:
                 p2t_ampl = data_seg[p_idx] - data_seg[t_idx]
                 clipped = float(np.sum(data_seg[p_idx] > max_clip) +
                                 np.sum(data_seg[t_idx] < min_clip))/2/len(p2t_ampl)
     if found_bestwindow:
         return data[idx0:idx1], idx0, idx1, clipped, min_clip, max_clip
     else:
         return data, 0, 0, False, min_clip, max_clip
 
 
-if __name__ == "__main__":
-    print("Checking bestwindow module ...")
-    import sys
-
-    title = "bestwindow"
-    if len(sys.argv) < 2:
+def main(data_file=None):
+    title = 'bestwindow'
+    if data_file is None:
         # generate data:
-        print("generate waveform...")
+        print('generate waveform...')
         rate = 100000.0
         time = np.arange(0.0, 1.0, 1.0 / rate)
         f = 600.0
         snippets = []
         amf = 20.0
         for ampl in [0.2, 0.5, 0.8]:
             for am_ampl in [0.0, 0.3, 0.9]:
                 data = ampl * np.sin(2.0 * np.pi * f * time) * (1.0 + am_ampl * np.sin(2.0 * np.pi * amf * time))
                 data[data > 1.3] = 1.3
                 data[data < -1.3] = -1.3
                 snippets.extend(data)
         data = np.asarray(snippets)
-        title = "test sines"
+        title = 'test sines'
         data += 0.01 * np.random.randn(len(data))
     else:
-        from .dataloader import load_data
-
-        print("load %s ..." % sys.argv[1])
-        data, rate, unit = load_data(sys.argv[1], 0)
-        title = sys.argv[1]
+        from thunderlab.dataloader import load_data
+        print(f'load {data_file} ...')
+        data, rate, unit, amax = load_data(data_file)
+        data = data[:,0]
+        title = data_file
 
     # determine clipping amplitudes:
     clip_win_size = 0.5
     min_clip_fac = 2.0
     min_clip, max_clip = clip_amplitudes(data, int(clip_win_size * rate),
                                          min_fac=min_clip_fac)
     # min_clip, max_clip = clip_amplitudes(data, int(clip_win_size*rate),
     #                                      min_fac=min_clip_fac,
     #                                      plot_hist_func=plot_clipping)
 
     # setup plots:
-    fig, ax = plt.subplots(5, sharex=True, figsize=(20, 12))
-    fig.canvas.set_window_title(title)
+    fig, ax = plt.subplots(5, 1, sharex=True, figsize=(20, 12))
+    fig.canvas.manager.set_window_title(title)
 
     # compute best window:
-    print("call bestwindow() function...")
-    best_window_indices(data, rate, expand=False,
-                        win_size=4.0, win_shift=0.5, thresh_fac=0.8, percentile=0.1,
+    best_window_indices(data, rate, expand=False, win_size=4.0,
+                        win_shift=0.5, thresh_fac=0.8, percentile=0.1,
                         min_clip=min_clip, max_clip=max_clip,
                         w_cv_ampl=10.0, tolerance=0.5,
                         plot_data_func=plot_best_window, ax=ax)
 
     plt.tight_layout()
     plt.show()
+
+    
+if __name__ == '__main__':
+    import sys
+    data_file = sys.argv[1] if len(sys.argv) > 1 else None
+    main(data_file)
```

### Comparing `thunderfish-1.9.9/thunderfish/checkpulse.py` & `thunderfish-2.0.0/src/thunderfish/checkpulse.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 - `add_check_pulse_config()`: add parameters for `check_pulse()` to configuration.
 - `check_pulse_args()`: retrieve parameters for `check_pulse()` from configuration.
 
 """
 
 import numpy as np
-from .eventdetection import percentile_threshold, detect_peaks, trim
+from thunderlab.eventdetection import percentile_threshold, detect_peaks, trim
 
 
 def check_pulse(data, sem, samplerate, thresh_fac=0.8, percentile=0.0,
                 sem_fac=0.05, pulse_thresh=0.15, verbose=0):
     """Detects if a fish is pulse- or wave-type based on the proportion of the time distance
     between a peak and its following trough, relative to the time between consecutive peaks.
 
@@ -55,15 +55,15 @@
         from peak-2-peak time distance, i.e. pulse width relative to pulse interval.
     """
 
     def ratio(peak_idx, trough_idx):
         if len(peak_idx) < 2:
             return 1.0 if len(peak_idx)+len(trough_idx) < 1 else 0.0
         # ratio of peak-to-trough to peak-to-peak time distances:
-        ratios = np.abs((trough_idx - peak_idx))[:-1].astype(np.float) / np.diff(peak_idx)
+        ratios = np.abs((trough_idx - peak_idx))[:-1].astype(float) / np.diff(peak_idx)
         # fix for cases where trough of eod comes before peak:
         ratios[ratios > 0.5] = 1.0 - ratios[ratios > 0.5]
         return np.median(ratios)
 
     # threshold for peak detection:
     pp_ampl = percentile_threshold(data, thresh_fac=1.0, percentile=percentile)
     threshold = thresh_fac*pp_ampl
@@ -155,16 +155,16 @@
     elif sys.argv[1] == '-m':
         data = pulsefish_eods('monophasic', 80.0, rate, 8.0)
     elif sys.argv[1] == '-b':
         data = pulsefish_eods('biphasic', 80.0, rate, 8.0)
     elif sys.argv[1] == '-t':
         data = pulsefish_eods('triphasic', 80.0, rate, 8.0)
     else:  # load data given by the user
-        from .dataloader import load_data
+        from thunderlab.dataloader import load_data
 
         file_path = sys.argv[1]
         print("loading %s ...\n" % file_path)
-        rawdata, rate, unit = load_data(sys.argv[1], 0)
-        data, _ = best_window(rawdata, rate)
+        rawdata, rate, unit, amax = load_data(sys.argv[1])
+        data, _ = best_window(rawdata[:,0], rate)
         
     # run pulse-width-based detector:
     pulse_fish, ratio = check_pulse(data, None, rate)
```

### Comparing `thunderfish-1.9.9/thunderfish/chirp.py` & `thunderfish-2.0.0/src/thunderfish/chirp.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 - `chirp_analysis()`: calculates spectrogram, detects fishes and extracts chirp times(combined for all fishes).
                   !!! recommended for short recordings (up to 5 min) where only the chirp times shall be extracted !!!
 - `chirp_detection()`: extracts chirp times with help of given spectrogram and fishlist.
 """
 
 import numpy as np
-from .harmonics import harmonic_groups
-from .powerspectrum import spectrogram
-from .eventdetection import std_threshold, detect_peaks, trim_to_peak
 import matplotlib.pyplot as plt
+from thunderlab.powerspectrum import spectrogram
+from thunderlab.eventdetection import std_threshold, detect_peaks, trim_to_peak
+from .harmonics import harmonic_groups
 
 
 def true_chirp_power_drop(chirp_time_idx, power, power_window=100):
     """
     Chirp is only accepted as such if the power of the frequency drops down as expected.
 
     :param chirp_time_idx: (array) indices of chirps.
@@ -61,15 +61,15 @@
 
 
 def chirp_detection(spectrum, freqs, time, fishlist=None, fundamentals=None, min_power= 0.005, freq_tolerance=1., chirp_th=1.,
                     plot_data_func=None):
     """
     Detects chirps on the basis of a spectrogram.
 
-    :param spectrum: (2d-array) spectrum calulated with the numpy.spectrogram function.
+    :param spectrum: (2d-array) spectrum calulated with the `spectrogram()` function.
     :param freqs: (array) frequencies of the spectrum.
     :param time: (array) time of the nffts used in the spectrum.
     :param fishlist: (array) power und frequncy for each fundamental/harmonic of a detected fish.
                      fishlist[fish][harmonic][frequency, power]
     :param min_power: (float) minimum power of the fundamental frequency for each fish to participate in chirp detection.
     :param freq_tolerance: (float) frequency tolerance in the spectrum to detect the power of a certain frequency.
     :param chirp_th: (float) minimum chirp duration to be accepted as a chirp.
@@ -166,15 +166,15 @@
     For further documentation see functions chirp_spectrogram() and chirp_detection().
     !!! recommended for short recordings (up to 5 min) where only the chirp times shall be extracted !!!
 
     :param data: (array) data.
     :param samplerate: (float) smaplerate of the data.
     :param min_power: (float) minimal power of the fish fundamental to include this fish in chirp detection.
     """
-    spectrum, freqs, time = spectrogram(data, samplerate, freq_resolution=2., overlap_frac=0.95)
+    freqs, time, spectrum = spectrogram(data, samplerate, freq_resolution=2., overlap_frac=0.95)
 
     power = np.mean(spectrum, axis=1) # spectrum[:, t0:t1] to only let spectrum of certain time....
 
     fishlist = harmonic_groups(freqs, power)[0]
 
     chirp_time, chirp_freq = chirp_detection(spectrum, freqs, time, fishlist, plot_data_func=chirp_detection_plot)
 
@@ -186,15 +186,15 @@
 if __name__ == '__main__':
     ###
     # If you want to test the code I propose to use the file '60427L05.WAV' of the transect
     # '2016_04_27__downstream_stonewall_at_pool' made in colombia, 2016.
     ###
     import sys
     import matplotlib.pyplot as plt
-    from .dataloader import load_data
+    from thunderlab.dataloader import load_data
 
     data_file = sys.argv[1]
-    raw_data, samplerate, unit = load_data(data_file, 0)
+    raw_data, samplerate, unit, amax = load_data(data_file)
 
-    chirp_time, chirp_freq = chirp_analysis(raw_data, samplerate)
+    chirp_time, chirp_freq = chirp_analysis(raw_data[:,0], samplerate)
 
     # power = np.mean(spectrum[:, t:t + nffts_per_psd], axis=1)
```

### Comparing `thunderfish-1.9.9/thunderfish/collectfish.py` & `thunderfish-2.0.0/src/thunderfish/collectfish.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """
 Collect data generated by thunderfish in a wavefish and a pulsefish table.
 """
 
 import os
 import glob
+import io
+import zipfile
 import sys
 import argparse
 import numpy as np
+from thunderlab.configfile import ConfigFile
+from thunderlab.tabledata import TableData, add_write_table_config, write_table_args
 from .version import __version__, __year__
-from .configfile import ConfigFile
-from .tabledata import TableData, add_write_table_config, write_table_args
 from .harmonics import add_harmonic_groups_config
 from .eodanalysis import wave_similarity, pulse_similarity
 from .eodanalysis import load_species_waveforms, add_species_config
 from .eodanalysis import wave_quality, wave_quality_args, add_eod_quality_config
 from .eodanalysis import pulse_quality, pulse_quality_args
 from .eodanalysis import adjust_eodf
+from .eodanalysis import parse_filename
 
 
 def collect_fish(files, simplify_file=False,
                  meta_data=None, meta_recordings=None, skip_recordings=False,
                  temp_col=None, q10=1.62, max_fish=0, harmonics=None,
                  peaks0=None, peaks1=None, cfg=None, verbose=0):
     """Combine all *-wavefish.* and/or *-pulsefish.* files into respective summary tables.
@@ -88,35 +91,69 @@
         Summary table for all wave-type fish.
     pulse_table: TableData
         Summary table for all pulse-type fish.
     all_table: TableData
         Summary table for all wave-type and pulse-type fish.
 
     """
+    def file_iter(files):
+        """ Iterate over analysis files.
+
+        Parameters
+        ----------
+        files: list of str
+            Input files.
+
+        Yields
+        ------
+        zf: ZipFile or None
+            In case an input file is a zip archive, the open archive.
+        file_path: str
+            The full path of a single file to be processed.
+            I.e. a '*-wavefish.*' or  '*-pulsefish.*' file.
+        fish_type: str
+            Either 'wave' or 'pulse'.
+        """
+        for file_path in files:
+            _, _, _, _, ftype, _, ext = parse_filename(file_path)
+            if ext == 'zip':
+                zf = zipfile.ZipFile(file_path)
+                file_pathes = sorted(zf.namelist())
+                for zfile in file_pathes:
+                    _, _, _, _, ftype, _, _ = parse_filename(zfile)
+                    if ftype in ['wavefish', 'pulsefish']:
+                        yield zf, zfile, ftype[:-4]
+            elif ftype in ['wavefish', 'pulsefish']:
+                yield None, file_path, ftype[:-4]
+            else:
+                continue
+
+            
     def find_recording(recording, meta_recordings):
         """ Find row of a recording in meta data.
 
         Parameters
         ----------
         recording: string
-            Base name of a recording.
+            Path and base name of a recording.
         meta_recordings: list of string
             List of meta data recordings where to find `recording`.
         """
         if meta_data is not None:
             rec = os.path.splitext(os.path.basename(recording))[0]
             for i in range(len(meta_recordings)):
+                # TODO: strip extension!
                 if rec == meta_recordings[i]:
                     return i
         return -1
         
     # prepare meta recodings names:
     meta_recordings_used = None
     if meta_recordings is not None:
-        meta_recordings_used = np.zeros(len(meta_recordings), dtype=np.bool)
+        meta_recordings_used = np.zeros(len(meta_recordings), dtype=bool)
         for r in range(len(meta_recordings)):
             meta_recordings[r] = os.path.splitext(os.path.basename(meta_recordings[r]))[0]
     # prepare adjusted temperatures:
     if meta_data is not None and temp_col is not None:
         temp_idx = meta_data.index(temp_col)
         temp = meta_data[:,temp_idx]
         mean_tmp = np.round(np.nanmean(temp)/0.1)*0.1
@@ -128,42 +165,21 @@
     wave_max_rms = cfg.value('maximumWaveSpeciesRMS')
     pulse_max_rms = cfg.value('maximumPulseSpeciesRMS')
     # load data:    
     wave_table = None
     pulse_table = None
     all_table = None
     file_pathes = []
-    for file_name in files:
+    for zf, file_name, fish_type in file_iter(files):
         # file name:
         table = None
-        base_path, file_ext = os.path.splitext(file_name)[0:2]
-        if base_path.endswith('-pulsefish'):
-            base_path = base_path[:-10]
-            fish_type = 'pulse'
-        elif base_path.endswith('-wavefish'):
-            base_path = base_path[:-9]
-            fish_type = 'wave'
-        else:
-            continue
-        if base_path.startswith('./'):
-            base_path = base_path[2:]
-        recording = base_path
-        # extract time:
-        start_time = None
         window_time = None
-        rs = recording.split('-')
-        if len(rs) > 0 and rs[-1][0] == 't':
-            start_time = float(rs[-1][1:-1])
-            rs = rs[:-1]
-        # extract channel:
-        channel = None
-        if len(rs) > 0 and rs[-1][0] == 'c':
-            channel = int(rs[-1][1:])
-            rs = rs[:-1]
-        recording = '-'.join(rs)
+        recording, base_path, channel, start_time, _, _, file_ext = \
+            parse_filename(file_name)
+        file_ext = os.extsep + file_ext
         file_pathes.append(os.path.normpath(recording).split(os.path.sep))
         if verbose > 2:
             print('processing %s (%s):' % (file_name, recording))
         # find row in meta_data:
         mr = -1
         if meta_data is not None:
             mr = find_recording(recording, meta_recordings)
@@ -173,19 +189,21 @@
                         print('skip recording %s: no metadata found' % recording)
                     continue
                 elif verbose > 0:
                     print('no metadata found for recording %s' % recording)
             else:
                 meta_recordings_used[mr] = True
         # data:
+        if zf is not None:
+            file_name = io.TextIOWrapper(zf.open(file_name, 'r'))
         data = TableData(file_name)
-        if 'tstart' in data:
-            start_time = data[0, 'tstart']
-            window_time = data[0, 'twindow']
-            data.remove(['tstart', 'twindow'])
+        if 'twin' in data:
+            start_time = data[0, 'twin']
+            window_time = data[0, 'window']
+            data.remove(['twin', 'window'])
         table = wave_table if fish_type == 'wave' else pulse_table
         # prepare tables:
         if not table:
             df = TableData(data)
             df.clear_data()
             if meta_data is not None:
                 if data.nsecs > 0:
@@ -193,19 +211,22 @@
                 for c in range(meta_data.columns()):
                     df.insert(c, *meta_data.column_head(c))
             df.insert(0, ['recording']*data.nsecs + ['file'], '', '%-s')
             if window_time is not None:
                 df.insert(1, 'window', 's', '%.2f')
             if start_time is not None:
                 df.insert(1, 'time', 's', '%.2f')
-            if channel is not None:
+            if channel >= 0:
                 df.insert(1, 'channel', '', '%d')
             if fish_type == 'wave':
                 if harmonics is not None:
-                    wave_spec = TableData(base_path + '-wavespectrum-0' + file_ext)
+                    fn = base_path + '-wavespectrum-0' + file_ext
+                    if zf is not None:
+                        fn = io.TextIOWrapper(zf.open(fn, 'r'))
+                    wave_spec = TableData(fn)
                     if data.nsecs > 0:
                         df.append_section('harmonics')
                     for h in range(min(harmonics, wave_spec.rows())+1):
                         df.append('ampl%d' % h, wave_spec.unit('amplitude'),
                                       wave_spec.format('amplitude'))
                         if h > 0:
                             df.append('relampl%d' % h, '%', '%.2f')
@@ -215,15 +236,18 @@
                     if data.nsecs > 0:
                         df.append_section('species')
                     for species in wave_names:
                         df.append(species, '%', '%.0f')
                     df.append('species', '', '%-s')
             else:
                 if peaks0 is not None:
-                    pulse_peaks = TableData(base_path + '-pulsepeaks-0' + file_ext)
+                    fn = base_path + '-pulsepeaks-0' + file_ext
+                    if zf is not None:
+                        fn = io.TextIOWrapper(zf.open(fn, 'r'))
+                    pulse_peaks = TableData(fn)
                     if data.nsecs > 0:
                         df.append_section('peaks')
                     for p in range(peaks0, peaks1+1):
                         if p != 1:
                             df.append('P%dtime' % p, 'ms', '%.3f')
                         df.append('P%dampl' % p, pulse_peaks.unit('amplitude'),
                                   pulse_peaks.format('amplitude'))
@@ -241,20 +265,20 @@
                 table = wave_table
             else:
                 pulse_table = df
                 table = pulse_table
             if not all_table:
                 df = TableData()
                 df.append('file', '', '%-s')
+                if channel >= 0:
+                    df.append('channel', '', '%d')
                 if start_time is not None:
                     df.append('time', 's', '%.1f')
                 if window_time is not None:
                     df.append('window', 's', '%.1f')
-                if channel is not None:
-                    df.append('channel', '', '%d')
                 if meta_data is not None:
                     for c in range(meta_data.columns()):
                         df.append(*meta_data.column_head(c))
                 df.append('index', '', '%d')
                 df.append('EODf', 'Hz', '%.1f')
                 df.append('type', '', '%-5s')
                 if len(wave_names) + len(pulse_names) > 0:
@@ -266,15 +290,18 @@
             # fish index:
             idx = r
             if 'index' in data:
                 idx = data[r,'index']
             # check quality:
             skips = ''
             if fish_type == 'wave':
-                wave_spec = TableData(base_path + '-wavespectrum-%d'%idx + file_ext)
+                fn = base_path + '-wavespectrum-%d'%idx + file_ext
+                if zf is not None:
+                    fn = io.TextIOWrapper(zf.open(fn, 'r'))
+                wave_spec = TableData(fn)
                 if cfg is not None:
                     spec_data = wave_spec.array()
                     props = data.row_dict(r)
                     if 'clipped' in props:
                         props['clipped'] *= 0.01 
                     if 'noise' in props:
                         props['noise'] *= 0.01 
@@ -297,15 +324,15 @@
                     print('skip fish %2d from %s: %s' % (idx, recording, skips))
                 continue
             # fill in data:
             data_col = 0
             table.append_data(recording, data_col)
             all_table.append_data(recording, data_col)
             data_col += 1
-            if channel is not None:
+            if channel >= 0:
                 table.append_data(channel, data_col)
                 all_table.append_data(channel, data_col)
                 data_col += 1
             if start_time is not None:
                 table.append_data(start_time, data_col)
                 all_table.append_data(start_time, data_col)
                 data_col += 1
@@ -333,50 +360,59 @@
                     for h in range(min(harmonics, wave_spec.rows())+1):
                         table.append_data(wave_spec[h,'amplitude'])
                         if h > 0:
                             table.append_data(wave_spec[h,'relampl'])
                             table.append_data(wave_spec[h,'relpower'])
                         table.append_data(wave_spec[h,'phase'])
                 if len(wave_names) > 0:
-                    wave_eod = TableData(base_path + '-eodwaveform-%d'%idx + file_ext).array()
+                    fn = base_path + '-eodwaveform-%d'%idx + file_ext
+                    if zf is not None:
+                        fn = io.TextIOWrapper(zf.open(fn, 'r'))
+                    wave_eod = TableData(fn).array()
                     wave_eod[:,0] *= 0.001
                     for species, eod in zip(wave_names, wave_eods):
                         rms = wave_similarity(eod, wave_eod, 1.0, eodf)
                         if rms < species_rms and rms < wave_max_rms:
                             species_name = species
                             species_rms = rms
                         table.append_data(100.0*rms)
                     table.append_data(species_name)
             else:
                 if peaks0 is not None:
-                    pulse_peaks = TableData(base_path + '-pulsepeaks-%d'%idx + file_ext)
+                    fn = base_path + '-pulsepeaks-%d'%idx + file_ext
+                    if zf is not None:
+                        fn = io.TextIOWrapper(zf.open(fn, 'r'))
+                    pulse_peaks = TableData(fn)
                     for p in range(peaks0, peaks1+1):
                         for pr in range(pulse_peaks.rows()):
                             if pulse_peaks[pr,'P'] == p:
                                 break
                         else:
                             continue
                         if p != 1:
                             table.append_data(pulse_peaks[pr,'time'], 'P%dtime' % p)
                         table.append_data(pulse_peaks[pr,'amplitude'], 'P%dampl' % p)
                         if p != 1:
                             table.append_data(pulse_peaks[pr,'relampl'], 'P%drelampl' % p)
                         table.append_data(pulse_peaks[pr,'width'], 'P%dwidth' % p)
                 if len(pulse_names) > 0:
-                    pulse_eod = TableData(base_path + '-eodwaveform-%d'%idx + file_ext).array()
+                    fn = base_path + '-eodwaveform-%d'%idx + file_ext
+                    if zf is not None:
+                        fn = io.TextIOWrapper(zf.open(fn, 'r'))
+                    pulse_eod = TableData(fn).array()
                     pulse_eod[:,0] *= 0.001
                     for species, eod in zip(pulse_names, pulse_eods):
                         rms = pulse_similarity(eod, pulse_eod)
                         if rms < species_rms and rms < pulse_max_rms:
                             species_name = species
                             species_rms = rms
                         table.append_data(100.0*rms)
                     table.append_data(species_name)
-            if len(wave_names) + len(pulse_names) > 0:
-                all_table.append_data(species_name)
+            #if len(wave_names) + len(pulse_names) > 0:
+            #    all_table.append_data(species_name)
             table.fill_data()
             all_table.fill_data()
     # check coverage of meta data:
     if meta_recordings_used is not None:
         if np.all(meta_recordings_used):
             if verbose > 0:
                 print('found recordings for all meta data')
```

### Comparing `thunderfish-1.9.9/thunderfish/consistentfishes.py` & `thunderfish-2.0.0/src/thunderfish/consistentfishes.py`

 * *Files identical despite different names*

### Comparing `thunderfish-1.9.9/thunderfish/efield.py` & `thunderfish-2.0.0/src/thunderfish/efield.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Simulations of spatial electric fields.
+"""Simulations of spatial electric fields.
 
 ## Electric monopoles
 
 For simulating the spatial geometry of electric fields generated by electric fishes
 and perturbed by objects, first generate monopoles and charges:
 
 - `efish_monopoles()`: monopoles for simulating the electric field of an electric fish.
@@ -26,15 +25,15 @@
 
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.patches import FancyArrowPatch
 
 
 def efish_monopoles(pos=(0, 0), direction=(1, 0), size=10.0, bend=0, nneg=1):
-    """ Monopoles for simulating the electric field of an electric fish.
+    """Monopoles for simulating the electric field of an electric fish.
 
     This implements the model published in
     Chen, House, Krahe, Nelson (2005) "Modeling signal and background
     components of electrosensory scenes", J Comp Physiol A 191: 331-345
 
     Ten monopoles per unit size are uniformly distributed along the fish's body axis.
     The first (tail) nneg monopoles get negative charges that equal in sum
@@ -103,15 +102,15 @@
     poles[:,:2] = np.dot(poles[:,:2], rm)
     # translation:
     poles += pos
     return poles, charges
 
 
 def object_monopoles(pos=(0, 0), radius=1.0, chi=1.0, *args):
-    """ Monopoles for simulating a circular object.
+    """Monopoles for simulating a circular object.
 
     The circular object is approximated by an induced dipole, as
     sugested by Rasnow B (1996) "The effects of simple objects on the
     electric field of Apteronotus", J Comp Physiol A 178:397-411 and
     Chen, House, Krahe, Nelson (2005) "Modeling signal and background
     components of electrosensory scenes", J Comp Physiol A 191: 331-345.
 
@@ -175,15 +174,15 @@
     poles[0,:] = -eobj*0.5*eps/eobjnorm   # distance between monopoles
     poles[1,:] = +eobj*0.5*eps/eobjnorm   # distance between monopoles
     poles += pos                          # translation to required position
     return poles, charges
 
 
 def epotential(pos, *args):
-    """ Simulation of electric field potentials.
+    """Simulation of electric field potentials.
 
     Parameters
     ----------
     pos: 2D array of floats
         Each row contains the coordinates (2D or 3D)
         for which the potential should be computed.
     args: list of tuples
@@ -205,15 +204,15 @@
             rnorm = np.linalg.norm(r, axis=1)
             rnorm[np.abs(rnorm) < 1e-12] = 1.0e-12
             pot += c/rnorm
     return pot
 
 
 def epotential_meshgrid(xx, yy, zz, *args):
-    """ Simulation of electric field potentials on a mesh grid.
+    """Simulation of electric field potentials on a mesh grid.
 
     This is a simple wrapper for epotential().
 
     Parameters
     ----------
     xx: 2D array of floats
         Range of x coordinates as returned by numpy.meshgrid().
@@ -263,15 +262,15 @@
     """
     pos = np.vstack((xx.ravel(), yy.ravel())).T
     pot = epotential(pos, *args)
     return pot.reshape(xx.shape)
 
     
 def efield(pos, *args):
-    """ Simulation of electric field given a set of electric monopoles.
+    """Simulation of electric field given a set of electric monopoles.
 
     Parameters
     ----------
     pos: array of floats
         Each row contains the coordinates (2D or 3D)
         for which the potential should be computed.
         A single (1D) position is also accepted.
@@ -298,15 +297,15 @@
             rnorm[np.abs(rnorm) < 1e-12] = 1.0e-12
             fac = c/rnorm**3
             field += r*fac[:,np.newaxis]
     return field[0] if onedim else field
 
 
 def efield_meshgrid(xx, yy, zz, *args):
-    """ Simulation of electric field on a mesh grid.
+    """Simulation of electric field on a mesh grid.
 
     This is a simple wrapper for efield().
     
     Parameters
     ----------
     xx: 2D array of floats
         Range of x coordinates as returned by numpy.meshgrid().
@@ -370,15 +369,15 @@
     else:
         pos = np.vstack((xx.ravel(), yy.ravel(), zz.ravel())).T
         ef = efield(pos, *args)
         return ef[:,0].reshape(xx.shape), ef[:,1].reshape(xx.shape), ef[:,2].reshape(xx.shape)
 
 
 def projection(ex, ey, ez, nx, ny, nz):
-    """ Projection of electric field on surface normals.
+    """Projection of electric field on surface normals.
 
     Parameters
     ----------
     ex: array of floats
         x-coordinates of the electric field.
     ey: array of floats
         y-coordinates of the electric field.
@@ -394,15 +393,15 @@
     ef = np.vstack((ex.ravel(), ey.ravel(), ez.ravel())).T
     nf = np.vstack((nx.ravel(), ny.ravel(), nz.ravel())).T
     proj = np.sum(ef*nf, axis=1)
     return proj.reshape(ex.shape)
 
 
 def fieldline(pos0, bounds, *args, eps=0.1, maxiter=1000):
-    """ Compute an electric field line.
+    """Compute an electric field line.
 
     From the initial position `pos0` the field line is computed in both directions
     until it leaves the area defined by `bounds`.
 
     Parameters
     ----------
     pos0: array of floats
@@ -465,15 +464,15 @@
         uv /= np.linalg.norm(uv)
         p = p - eps*uv
     fl = np.vstack((flb[::-2], flf[::2]))
     return fl
 
 
 def squareroot_transform(values, thresh=0.0):
-    """ Square-root transformation keeping the sign.
+    """Square-root transformation keeping the sign.
 
     Takes the square root of positive values and takes the square root
     of the absolute values of negative values and negates the results.
 
     Then truncate symmetrically both positive and negative values to
     a threshold.
 
@@ -505,15 +504,15 @@
     if thresh > 0:
         values[values>thresh] = thresh
         values[values<-thresh] = -thresh
     return values
 
 
 def plot_fieldlines(ax, flines, pos=5, **kwargs):
-    """ Plot field lines with arrows.
+    """Plot field lines with arrows.
 
     Parameters
     ----------
     ax: matplotlib axes
         Axes in which to plot the field lines.
     flines: list of 2D arrays
         The field lines.
```

### Comparing `thunderfish-1.9.9/thunderfish/eodanalysis.py` & `thunderfish-2.0.0/src/thunderfish/eodanalysis.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,14 +41,20 @@
 - `load_pulse_fish()`: load properties of pulse EODs from file.
 - `save_wave_spectrum()`: save amplitude and phase spectrum of wave EOD to file.
 - `load_wave_spectrum()`: load amplitude and phase spectrum of wave EOD from file.
 - `save_pulse_spectrum()`: save power spectrum of pulse EOD to file.
 - `load_pulse_spectrum()`: load power spectrum of pulse EOD from file.
 - `save_pulse_peaks()`: save peak properties of pulse EOD to file.
 - `load_pulse_peaks()`: load peak properties of pulse EOD from file.
+- `save_pulse_times()`: save times of pulse EOD to file.
+- `load_pulse_times()`: load times of pulse EOD from file.
+- `parse_filename()`: parse components of an EOD analysis file name.
+- `save_analysis(): save EOD analysis results to files.
+- `load_analysis()`: load EOD analysis files.
+- `load_recording()`: load recording.
 
 ## Fit functions
 
 - `fourier_series()`: Fourier series of sine waves with amplitudes and phases.
 - `exp_decay()`: exponential decay.
 
 ## Filter functions
@@ -64,23 +70,27 @@
 - `add_species_config()`: add parameters needed for assigning EOD waveforms to species.
 - `add_eod_quality_config()`: add parameters needed for assesing the quality of an EOD waveform.
 - `wave_quality_args()`: retrieve parameters for `wave_quality()` from configuration.
 - `pulse_quality_args()`: retrieve parameters for `pulse_quality()` from configuration.
 """
 
 import os
+import io
+import glob
+import zipfile
 import numpy as np
 from scipy.optimize import curve_fit
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
-from .eventdetection import percentile_threshold, detect_peaks, snippets, peak_width
-from .eventdetection import threshold_crossings, threshold_crossing_times, merge_events
-from .powerspectrum import next_power_of_two, nfft, decibel
+from thunderlab.eventdetection import percentile_threshold, detect_peaks, snippets, peak_width
+from thunderlab.eventdetection import threshold_crossings, threshold_crossing_times, merge_events
+from thunderlab.powerspectrum import next_power_of_two, nfft, decibel
+from thunderlab.tabledata import TableData
+from thunderlab.dataloader import load_data
 from .harmonics import fundamental_freqs_and_power
-from .tabledata import TableData
 
 
 def eod_waveform(data, samplerate, eod_times, win_fac=2.0, min_win=0.01,
                  min_sem=False, max_eods=None, unfilter_cutoff=0.0):
     """Detect EODs in the given data, extract data snippets around each EOD,
     and compute a mean waveform with standard error.
 
@@ -117,24 +127,25 @@
     Parameters
     ----------
     data: 1-D array of float
         The data to be analysed.
     samplerate: float
         Sampling rate of the data in Hertz.
     eod_times: 1-D array of float
-        Array of EOD times in seconds over which the waveform should be averaged.
+        Array of EOD times in seconds over which the waveform should be
+        averaged.
         WARNING: The first data point must be at time zero!
     win_fac: float
-        The snippet size is the EOD period times `win_fac`. The EOD period is determined
-        as the minimum interval between EOD times.
+        The snippet size is the EOD period times `win_fac`. The EOD period
+        is determined as the minimum interval between EOD times.
     min_win: float
         The minimum size of the snippets in seconds.
     min_sem: bool
-        If set, check for minimum in s.e.m. to set the maximum numbers of EODs to be used
-        for computing the average waveform.
+        If set, check for minimum in s.e.m. to set the maximum numbers
+        of EODs to be used for computing the average waveform.
     max_eods: int or None
         Maximum number of EODs to be used for averaging.
     unfilter_cutoff: float
         If not zero, the cutoff frequency for an inverse high-pass filter
         applied to the mean EOD waveform.
     
     Returns
@@ -143,15 +154,15 @@
         Average of the EOD snippets. First column is time in seconds,
         second column the mean eod, third column the standard error.
     eod_times: 1-D array
         Times of EOD peaks in seconds that have been actually used to calculate the
         averaged EOD waveform.
     """
     # indices of EOD times:
-    eod_idx = np.round(eod_times * samplerate).astype(np.int)
+    eod_idx = np.round(eod_times * samplerate).astype(int)
         
     # window size:
     period = np.min(np.diff(eod_times))
     win = 0.5*win_fac*period
     if 2*win < min_win:
         win = 0.5*min_win
     win_inx = int(win * samplerate)
@@ -192,22 +203,23 @@
     # time axis:
     mean_eod[:,0] = (np.arange(len(mean_eod)) - win_inx) / samplerate
     
     return mean_eod, eod_times
 
 
 def unfilter(data, samplerate, cutoff):
-    """
-    Apply inverse high-pass filter on data.
+    """Apply inverse high-pass filter on data.
 
-    Assumes high-pass filter \\[ \\tau \\dot y = -y + \\tau \\dot x \\] has
-    been applied on the original data \\(x\\), where \\(\\tau=(2\\pi
-    f_{cutoff})^{-1}\\) is the time constant of the filter. To recover \\(x\\)
-    the ODE \\[ \\tau \\dot x = y + \\tau \\dot y \\] is applied on the
-    filtered data \\(y\\).
+    Assumes high-pass filter
+    \\[ \\tau \\dot y = -y + \\tau \\dot x \\]
+    has been applied on the original data \\(x\\), where
+    \\(\\tau=(2\\pi f_{cutoff})^{-1}\\) is the time constant of the
+    filter. To recover \\(x\\) the ODE
+    \\[ \\tau \\dot x = y + \\tau \\dot y \\]
+    is applied on the filtered data \\(y\\).
 
     Parameters
     ----------
     data: ndarray
         High-pass filtered original data.
     samplerate: float
         Sampling rate of `data` in Hertz.
@@ -229,16 +241,15 @@
         x += (d1 - d0) + d0/fac
         data[k] = x
         d0 = d1
     return data
 
 
 def fourier_series(t, freq, *ap):
-    """
-    Fourier series of sine waves with amplitudes and phases.
+    """Fourier series of sine waves with amplitudes and phases.
 
     x(t) = sum_{i=0}^n ap[2*i]*sin(2 pi (i+1) freq t + ap[2*i+1])
     
     Parameters
     ----------
     t: float or array
         Time.
@@ -255,85 +266,103 @@
     omega = 2.0*np.pi*freq
     x = 0.0
     for i, (a, p) in enumerate(zip(ap[0:-1:2], ap[1::2])):
         x += a*np.sin((i+1)*omega*t+p)
     return x
 
 
-def analyze_wave(eod, freq, n_harm=10, power_n_harmonics=0, n_harmonics=3, flip_wave='none'):
-    """
-    Analyze the EOD waveform of a wave fish.
+def analyze_wave(eod, freq, n_harm=10, power_n_harmonics=0,
+                 n_harmonics=3, flip_wave='none'):
+    """Analyze the EOD waveform of a wave fish.
     
     Parameters
     ----------
     eod: 2-D array
-        The eod waveform. First column is time in seconds, second column the EOD waveform,
-        third column, if present, is the standard error of the EOD waveform,
-        Further columns are optional but not used.
+        The eod waveform. First column is time in seconds, second
+        column the EOD waveform, third column, if present, is the
+        standard error of the EOD waveform, Further columns are
+        optional but not used.
     freq: float or 2-D array
-        The frequency of the EOD or the list of harmonics (rows)
-        with frequency and peak height (columns) as returned from `harmonics.harmonic_groups()`.
+        The frequency of the EOD or the list of harmonics (rows) with
+        frequency and peak height (columns) as returned from
+        `harmonics.harmonic_groups()`.
     n_harm: int
         Maximum number of harmonics used for the Fourier decomposition.
     power_n_harmonics: int
-        Sum over the first `power_n_harmonics` harmonics for computing the total power.
-        If 0 sum over all harmonics.
+        Sum over the first `power_n_harmonics` harmonics for computing
+        the total power.  If 0 sum over all harmonics.
     n_harmonics: int
-        The maximum power of higher harmonics is computed from harmonics higher than the
-        maximum harmonics within the first three harmonics plus `n_harmonics`.
+        The maximum power of higher harmonics is computed from
+        harmonics higher than the maximum harmonics within the first
+        three harmonics plus `n_harmonics`.
     flip_wave: 'auto', 'none', 'flip'
         - 'auto' flip waveform such that the larger extremum is positive.
         - 'flip' flip waveform.
         - 'none' do not flip waveform.
     
     Returns
     -------
     meod: 2-D array of floats
-        The eod waveform. First column is time in seconds, second column the eod waveform.
-        Further columns are kept from the input `eod`. And a column is added with the
-        fit of the fourier series to the waveform.
+        The eod waveform. First column is time in seconds, second
+        column the eod waveform.  Further columns are kept from the
+        input `eod`. And a column is added with the fit of the fourier
+        series to the waveform.
     props: dict
         A dictionary with properties of the analyzed EOD waveform.
 
         - type: set to 'wave'.
         - EODf: is set to the EOD fundamental frequency.
         - p-p-amplitude: peak-to-peak amplitude of the Fourier fit.
         - flipped: True if the waveform was flipped.
         - amplitude: amplitude factor of the Fourier fit.
-        - rmssem: root-mean squared standard error mean of the averaged EOD waveform
-          relative to the p-p amplitude.
-        - rmserror: root-mean-square error between Fourier-fit and EOD waveform relative to
-          the p-p amplitude. If larger than about 0.05 the data are bad.
+        - noise: root-mean squared standard error mean of the averaged
+          EOD waveform relative to the p-p amplitude.
+        - rmserror: root-mean-square error between Fourier-fit and
+          EOD waveform relative to the p-p amplitude. If larger than
+          about 0.05 the data are bad.
         - ncrossings: number of zero crossings per period
-        - peakwidth: width of the peak at the averaged amplitude relative to EOD period.
-        - troughwidth: width of the trough at the averaged amplitude relative to EOD period.
-        - leftpeak: time from positive zero crossing to peak relative to EOD period.
-        - rightpeak: time from peak to negative zero crossing relative to EOD period.
-        - lefttrough: time from negative zero crossing to trough relative to EOD period.
-        - righttrough: time from trough to positive zero crossing relative to EOD period.
+        - peakwidth: width of the peak at the averaged amplitude relative
+          to EOD period.
+        - troughwidth: width of the trough at the averaged amplitude
+          relative to EOD period.
+        - leftpeak: time from positive zero crossing to peak relative
+          to EOD period.
+        - rightpeak: time from peak to negative zero crossing relative to
+          EOD period.
+        - lefttrough: time from negative zero crossing to trough relative to
+          EOD period.
+        - righttrough: time from trough to positive zero crossing relative to
+          EOD period.
         - p-p-distance: time between peak and trough relative to EOD period.
         - reltroughampl: amplitude of trough relative to peak amplitude.
-        - power: summed power of all harmonics of the extracted EOD waveform in decibel relative to one.
-        - datapower: summed power of all harmonics of the original data in decibel relative to one. Only if `freq` is a list of harmonics.
-        - thd: total harmonic distortion, i.e. square root of sum of amplitudes squared
-          of harmonics relative to amplitude of fundamental.  
-        - dbdiff: smoothness of power spectrum as standard deviation of differences in decibel power.
-        - maxdb: maximum power of higher harmonics relative to peak power in decibel.
+        - power: summed power of all harmonics of the extracted EOD waveform
+          in decibel relative to one.
+        - datapower: summed power of all harmonics of the original data in
+          decibel relative to one. Only if `freq` is a list of harmonics.
+        - thd: total harmonic distortion, i.e. square root of sum of
+          amplitudes squared of harmonics relative to amplitude
+          of fundamental.  
+        - dbdiff: smoothness of power spectrum as standard deviation of
+          differences in decibel power.
+        - maxdb: maximum power of higher harmonics relative to peak power
+          in decibel.
 
     spec_data: 2-D array of floats
-        First size columns are from the spectrum of the extracted waveform.
-        First column is the index of the harmonics, second column its frequency,
-        third column its amplitude, fourth column its amplitude relative to the fundamental,
-        fifth column is power of harmonics relative to fundamental in decibel,
-        and sixth column the phase shift relative to the fundamental.
-        If `freq` is a list of harmonics, a seventh column is added to `spec_data`
-        that contains the powers of the harmonics from the original power spectrum of the
-        raw data.
-        Rows are the harmonics, first row is the fundamental frequency with index 0,
-        relative amplitude of one, relative power of 0dB, and phase shift of zero.
+        First size columns are from the spectrum of the extracted
+        waveform.  First column is the index of the harmonics, second
+        column its frequency, third column its amplitude, fourth
+        column its amplitude relative to the fundamental, fifth column
+        is power of harmonics relative to fundamental in decibel, and
+        sixth column the phase shift relative to the fundamental.
+        If `freq` is a list of harmonics, a seventh column is added to
+        `spec_data` that contains the powers of the harmonics from the
+        original power spectrum of the raw data.  Rows are the
+        harmonics, first row is the fundamental frequency with index
+        0, relative amplitude of one, relative power of 0dB, and phase
+        shift of zero.
     error_str: string
         If fitting of the fourier series failed,
         this is reported in this string.
 
     Raises
     ------
     IndexError:
@@ -410,16 +439,16 @@
     # fit fourier series:
     ampl = 0.5*(np.max(meod[:,1])-np.min(meod[:,1]))
     while n_harm > 1:
         params = [freq0]
         for i in range(1, n_harm+1):
             params.extend([ampl/i, 0.0])
         try:
-            popt, pcov = curve_fit(fourier_series, meod[i0:i1,0], meod[i0:i1,1],
-                                   params, maxfev=2000)
+            popt, pcov = curve_fit(fourier_series, meod[i0:i1,0],
+                                   meod[i0:i1,1], params, maxfev=2000)
             break
         except (RuntimeError, TypeError):
             error_str += '%.1f Hz wave fish: fit of fourier series failed for %d harmonics. ' % (freq0, n_harm)
             n_harm //= 2
     for i in range(n_harm):
         # make all amplitudes positive:
         if popt[i*2+1] < 0.0:
@@ -429,34 +458,50 @@
         popt[i*2+2] %= 2.0*np.pi
         if popt[i*2+2] > np.pi:
             popt[i*2+2] -= 2.0*np.pi
     # store fourier fit:
     meod[:,-1] = fourier_series(meod[:,0], *popt)
     # store fourier spectrum:
     if hasattr(freq, 'shape'):
-        spec_data = np.zeros((n_harm, 7))
-        powers = freq[:n_harm, 1]
-        spec_data[:len(powers), 6] = powers
+        n = n_harm
+        n += np.sum(freq[:,0] > (n_harm+0.5)*freq[0,0])
+        spec_data = np.zeros((n, 7))
+        spec_data[:,:] = np.nan
+        k = 0
+        for i in range(n_harm):
+            while k < len(freq) and freq[k,0] < (i+0.5)*freq0:
+                k += 1
+            if k >= len(freq):
+                break
+            if freq[k,0] < (i+1.5)*freq0:
+                spec_data[i,6] = freq[k,1]
+                k += 1
+        for i in range(n_harm, n):
+            if k >= len(freq):
+                break
+            spec_data[i,:2] = [np.round(freq[k,0]/freq0)-1, freq[k,0]]
+            spec_data[i,6] = freq[k,1]
+            k += 1
     else:
         spec_data = np.zeros((n_harm, 6))
     for i in range(n_harm):
         spec_data[i,:6] = [i, (i+1)*freq0, popt[i*2+1], popt[i*2+1]/popt[1],
                            decibel((popt[i*2+1]/popt[1])**2.0), popt[i*2+2]]
     # smoothness of power spectrum:
-    db_powers = decibel(spec_data[:,2]**2)
+    db_powers = decibel(spec_data[:n_harm,2]**2)
     db_diff = np.std(np.diff(db_powers))
     # maximum relative power of higher harmonics:
     p_max = np.argmax(db_powers[:3])
     db_powers -= db_powers[p_max]
     if len(db_powers[p_max+n_harmonics:]) == 0:
         max_harmonics_power = -100.0
     else:
         max_harmonics_power = np.max(db_powers[p_max+n_harmonics:])
     # total harmonic distortion:
-    thd = np.sqrt(np.sum(spec_data[1:,3]))
+    thd = np.sqrt(np.nansum(spec_data[1:,3]))
 
     # peak and trough amplitudes:
     ppampl = np.max(meod[i0:i1,1]) - np.min(meod[i0:i1,1])
     relptampl = np.min(meod[i0:i1,1])/np.max(meod[i0:i1,1])
     
     # variance and fit error:
     rmssem = np.sqrt(np.mean(meod[i0:i1,2]**2.0))/ppampl if eod.shape[1] > 2 else None
@@ -467,164 +512,177 @@
     props['type'] = 'wave'
     props['EODf'] = freq0
     props['p-p-amplitude'] = ppampl
     props['flipped'] = flipped
     props['amplitude'] = 0.5*ppampl  # remove it
     props['rmserror'] = rmserror
     if rmssem:
-        props['rmssem'] = rmssem
+        props['noise'] = rmssem
     props['ncrossings'] = ncrossings
     props['peakwidth'] = peak_width/period
     props['troughwidth'] = trough_width/period
     props['leftpeak'] = phase1/period
     props['rightpeak'] = phase2/period
     props['lefttrough'] = phase3/period
     props['righttrough'] = phase4/period
     props['p-p-distance'] = distance/period
     props['reltroughampl'] = np.abs(relptampl)
     pnh = power_n_harmonics if power_n_harmonics > 0 else n_harm
+    pnh = min(n_harm, pnh)
     props['power'] = decibel(np.sum(spec_data[:pnh,2]**2.0))
     if hasattr(freq, 'shape'):
         props['datapower'] = decibel(np.sum(freq[:pnh,1]))
     props['thd'] = thd
     props['dbdiff'] = db_diff
     props['maxdb'] = max_harmonics_power
     
     return meod, props, spec_data, error_str
 
 
 def exp_decay(t, tau, ampl, offs):
-    """
-    Exponential decay function.
+    """Exponential decay function.
 
     x(t) = ampl*exp(-t/tau) + offs
 
     Parameters
     ----------
     t: float or array
         Time.
     tau: float
         Time constant of exponential decay.
     ampl: float
-        Amplitude of exponential decay, i.e. initial value minus steady-state value.
+        Amplitude of exponential decay, i.e. initial value minus
+        steady-state value.
     offs: float
         Steady-state value.
     
     Returns
     -------
     x: float or array
         The exponential decay evaluated at times `t`.
-    
+
     """
     return offs + ampl*np.exp(-t/tau)
 
 
-def analyze_pulse(eod, eod_times=None, min_pulse_win=0.001, peak_thresh_fac=0.01,
-                  min_dist=50.0e-6, width_frac = 0.5, fit_frac = 0.5,
-                  freq_resolution=1.0, flip_pulse='none',
-                  ipi_cv_thresh=0.5, ipi_percentile=30.0):
-    """
-    Analyze the EOD waveform of a pulse fish.
+def analyze_pulse(eod, eod_times=None, min_pulse_win=0.001,
+                  peak_thresh_fac=0.01, min_dist=50.0e-6,
+                  width_frac=0.5, fit_frac = 0.5, freq_resolution=1.0,
+                  flip_pulse='none', ipi_cv_thresh=0.5,
+                  ipi_percentile=30.0):
+    """Analyze the EOD waveform of a pulse fish.
     
     Parameters
     ----------
     eod: 2-D array
-        The eod waveform. First column is time in seconds, second column the EOD waveform,
-        third column, if present, is the standard error of the EOD waveform,
-        Further columns are optional but not used.
+        The eod waveform. First column is time in seconds, second
+        column the EOD waveform, third column, if present, is the
+        standard error of the EOD waveform, Further columns are
+        optional but not used.
     eod_times: 1-D array or None
         List of times of detected EOD peaks.
     min_pulse_win: float
         The minimum size of cut-out EOD waveform.
     peak_thresh_fac: float
-        Set the threshold for peak detection to the maximum pulse amplitude times this factor.
+        Set the threshold for peak detection to the maximum pulse
+        amplitude times this factor.
     min_dist: float
         Minimum distance between peak and troughs of the pulse.
     width_frac: float
-        The width of a peak is measured at this fraction of a peak's height (0-1).
+        The width of a peak is measured at this fraction of a peak's
+        height (0-1).
     fit_frac: float or None
-        An exponential is fitted to the tail of the last peak/trough starting where the
-        waveform falls below this fraction of the peak's height (0-1).
+        An exponential is fitted to the tail of the last peak/trough
+        starting where the waveform falls below this fraction of the
+        peak's height (0-1).
     freq_resolution: float
         The frequency resolution of the power spectrum of the single pulse.
     flip_pulse: 'auto', 'none', 'flip'
         - 'auto' flip waveform such that the first large extremum is positive.
         - 'flip' flip waveform.
         - 'none' do not flip waveform.
     ipi_cv_thresh: float
-        If the coefficient of variation of the interpulse intervals are smaller than this
-        threshold, then the EOD frequency is computed as the inverse of the mean of
-        all interpulse intervals. Otherwise only intervals smaller than a certain quantile
-        are used.
+        If the coefficient of variation of the interpulse intervals
+        are smaller than this threshold, then the EOD frequency is
+        computed as the inverse of the mean of all interpulse
+        intervals. Otherwise only intervals smaller than a certain
+        quantile are used.
     ipi_percentile: float
-        When computing the EOD frequency, period, mean and standard deviation of
-        interpulse intervals from a subset of the interpulse intervals,
-        only intervals smaller than this percentile (between 0 and 100) are used.
+        When computing the EOD frequency, period, mean and standard
+        deviation of interpulse intervals from a subset of the
+        interpulse intervals, only intervals smaller than this
+        percentile (between 0 and 100) are used.
     
     Returns
     -------
     meod: 2-D array of floats
         The eod waveform. First column is time in seconds,
         second column the eod waveform.
         Further columns are kept from the input `eod`.
         As a last column the fit to the tail of the last peak is appended.
     props: dict
         A dictionary with properties of the analyzed EOD waveform.
 
         - type: set to 'pulse'.
-        - EODf: the inverse of the median interval between `eod_times`, if provided.
+        - EODf: the inverse of the median interval between `eod_times`,
+          if provided.
         - period: the median interval between `eod_times`, if provided.
         - IPI-mean: the mean interval between `eod_times`, if provided.
-        - IPI-std: the standard deviation of the intervals between `eod_times`, if provided.
-        - max-amplitude: the amplitude of the largest positive peak (P1).
-        - min-amplitude: the amplitude of the largest negative peak (P2).
+        - IPI-std: the standard deviation of the intervals between
+          `eod_times`, if provided.
+        - max-ampl: the amplitude of the largest positive peak (P1).
+        - min-ampl: the amplitude of the largest negative peak (P2).
         - p-p-amplitude: peak-to-peak amplitude of the EOD waveform.
-        - rmssem: root-mean squared standard error mean of the averaged EOD waveform
-          relative to the p-p amplitude.
+        - noise: root-mean squared standard error mean of the averaged
+          EOD waveform relative to the p-p amplitude.
         - tstart: time in seconds where the pulse starts,
           i.e. crosses the threshold for the first time.
         - tend: time in seconds where the pulse ends,
           i.e. crosses the threshold for the last time.
         - width: total width of the pulse in seconds (tend-tstart).
-        - dist: distance between P2 and P1 in seconds.
+        - P2-P1-dist: distance between P2 and P1 in seconds.
         - tau: time constant of exponential decay of pulse tail in seconds.
         - firstpeak: index of the first peak in the pulse (i.e. -1 for P-1)
         - lastpeak: index of the last peak in the pulse (i.e. 3 for P3)
-        - peakfrequency: frequency at peak power of the single pulse spectrum in Hertz.
+        - peakfreq: frequency at peak power of the single pulse spectrum
+          in Hertz.
         - peakpower: peak power of the single pulse spectrum in decibel.
-        - lowfreqattenuation5: how much the average power below 5 Hz is attenuated
+        - poweratt5: how much the average power below 5 Hz is attenuated
           relative to the peak power in decibel.
-        - lowfreqattenuation50: how much the average power below 5 Hz is attenuated
+        - poweratt50: how much the average power below 5 Hz is attenuated
           relative to the peak power in decibel.
-        - powerlowcutoff: frequency at which the power reached half of the peak power
-          relative to the initial power in Hertz.
+        - lowcutoff: frequency at which the power reached half of the
+          peak power relative to the initial power in Hertz.
         - flipped: True if the waveform was flipped.
         - n: number of pulses analyzed  (i.e. `len(eod_times)`), if provided.
-        - times: the times of the detected EOD pulses (i.e. `eod_times`), if provided.
+        - times: the times of the detected EOD pulses (i.e. `eod_times`),
+          if provided.
 
         Empty if waveform is not a pulse EOD.
     peaks: 2-D array
         For each peak and trough (rows) of the EOD waveform
         5 columns: the peak index (1 is P1, i.e. the largest positive peak),
         time relative to largest positive peak, amplitude,
         amplitude normalized to largest postive peak,
         and width of peak/trough at half height.
         Empty if waveform is not a pulse EOD.
     power: 2-D array
-        The power spectrum of a single pulse. First column are the frequencies,
-        second column the power in x^2/Hz such that the integral equals the variance.
-        Empty if waveform is not a pulse EOD.
+        The power spectrum of a single pulse. First column are the
+        frequencies, second column the power in x^2/Hz such that the
+        integral equals the variance.  Empty if waveform is not a
+        pulse EOD.
+
     """
     # storage:
     meod = np.zeros((eod.shape[0], eod.shape[1]+1))
     meod[:,:eod.shape[1]] = eod
     meod[:,-1] = np.nan
     toffs = 0
     
-    # cut out stable estimate if standard deviation:
+    # cut out stable estimate if standard deviation is available:
     if eod.shape[1] > 2 and np.max(meod[:,2]) > 3*np.min(meod[:,2]):
         n = len(meod)
         idx0 = np.argmax(np.abs(meod[n//10:9*n//10,1])) + n//10
         toffs += meod[idx0,0]
         meod[:,0] -= meod[idx0,0]
         # minimum in standard deviation:
         lstd_idx = np.argmin(meod[:idx0-5,2])
@@ -865,85 +923,94 @@
     props = {}
     props['type'] = 'pulse'
     if eod_times is not None:
         props['EODf'] = 1.0/period
         props['period'] = period
         props['IPI-mean'] = ipi_mean
         props['IPI-std'] = ipi_std
-    props['max-amplitude'] = max_ampl
-    props['min-amplitude'] = min_ampl
+    props['max-ampl'] = max_ampl
+    props['min-ampl'] = min_ampl
     props['p-p-amplitude'] = ppampl
     if rmssem:
-        props['rmssem'] = rmssem
+        props['noise'] = rmssem
     props['tstart'] = t0
     props['tend'] = t1
     props['width'] = t1-t0
-    props['dist'] = dist
+    props['P2-P1-dist'] = dist
     if tau:
         props['tau'] = tau
     props['firstpeak'] = peaks[0, 0] if len(peaks) > 0 else 1
     props['lastpeak'] = peaks[-1, 0] if len(peaks) > 0 else 1
-    props['peakfrequency'] = freqs[np.argmax(power)]
+    props['peakfreq'] = freqs[np.argmax(power)]
     props['peakpower'] = decibel(maxpower)
-    props['lowfreqattenuation5'] = att5
-    props['lowfreqattenuation50'] = att50
-    props['powerlowcutoff'] = lowcutoff
+    props['poweratt5'] = att5
+    props['poweratt50'] = att50
+    props['lowcutoff'] = lowcutoff
     props['flipped'] = flipped
     if eod_times is not None:
         props['n'] = len(eod_times)
         props['times'] = eod_times + toffs
     
     return meod, props, peaks, ppower
 
 
 def adjust_eodf(eodf, temp, temp_adjust=25.0, q10=1.62):
-    """ Adjust EOD frequencies to a standard temperature using Q10.
+    """Adjust EOD frequencies to a standard temperature using Q10.
 
     Parameters
     ----------
     eodf: float or ndarray
         EOD frequencies.
     temp: float
-        Temperature in degree celsisus at which EOD frequencies in `eodf` were measured.
+        Temperature in degree celsisus at which EOD frequencies in
+        `eodf` were measured.
     temp_adjust: float
-        Standard temperature in degree celsisus  to which EOD frequencies are adjusted.
+        Standard temperature in degree celsisus to which EOD
+        frequencies are adjusted.
     q10: float
-        Q10 value describing temperature dependence of EOD frequencies.
-        The default of 1.62 is from Dunlap, Smith, Yetka (2000) Brain Behav Evol,
-        measured for Apteronotus lepthorhynchus in the lab.
+        Q10 value describing temperature dependence of EOD
+        frequencies.  The default of 1.62 is from Dunlap, Smith, Yetka
+        (2000) Brain Behav Evol, measured for Apteronotus
+        lepthorhynchus in the lab.
 
     Returns
     -------
     eodf_corrected: float or array
         EOD frequencies adjusted to `temp_adjust` using `q10`.
     """
-    return eodf * q10 ** ((temp_adjust - temp) / 10.0)
+    return eodf*q10**((temp_adjust - temp) / 10.0)
 
 
 def load_species_waveforms(species_file='none'):
-    """ Load template EOD waveforms for species matching.
+    """Load template EOD waveforms for species matching.
     
     Parameters
     ----------
     species_file: string
-        Name of file containing species definitions. The content of this file is as follows:
+        Name of file containing species definitions. The content of
+        this file is as follows:
         
         - Empty lines and line starting with a hash ('#') are skipped.
-        - A line with the key-word 'wavefish' marks the beginning of the table for wave fish.
-        - A line with the key-word 'pulsefish' marks the beginning of the table for wave fish.
-        - Each line in a species table has three fields, separated by colons (':'):
+        - A line with the key-word 'wavefish' marks the beginning of the
+          table for wave fish.
+        - A line with the key-word 'pulsefish' marks the beginning of the
+          table for pulse fish.
+        - Each line in a species table has three fields,
+          separated by colons (':'):
         
           1. First field is an abbreviation of the species name.
-          2. Second field is the filename of the recording containing the EOD waveform.
+          2. Second field is the filename of the recording containing the
+             EOD waveform.
           3. The optional third field is the EOD frequency of the EOD waveform.
 
-          The EOD frequency is used to normalize the time axis of a wave
-          fish EOD to one EOD period. If it is not specified in the third field,
-          it is taken from the corresponding *-wavespectrum-* file, if present.
-          Otherwise the species is excluded and a warning is issued.
+          The EOD frequency is used to normalize the time axis of a
+          wave fish EOD to one EOD period. If it is not specified in
+          the third field, it is taken from the corresponding
+          *-wavespectrum-* file, if present.  Otherwise the species is
+          excluded and a warning is issued.
 
         Example file content:
         ``` plain
         Wavefish
         Aptero : F_91009L20-eodwaveform-0.csv : 823Hz
         Eigen  : C_91008L01-eodwaveform-0.csv
 
@@ -953,24 +1020,27 @@
         ```
     
     Returns
     -------
     wave_names: list of strings
         List of species names of wave-type fish.
     wave_eods: list of 2-D arrays
-        List of EOD waveforms of wave-type fish corresponding to `wave_names`.
-        First column of a waveform is time in seconds, second column is the EOD waveform.
-        The waveforms contain exactly one EOD period.
+        List of EOD waveforms of wave-type fish corresponding to
+        `wave_names`.  First column of a waveform is time in seconds,
+        second column is the EOD waveform.  The waveforms contain
+        exactly one EOD period.
     pulse_names: list of strings
         List of species names of pulse-type fish.
     pulse_eods: list of 2-D arrays
-        List of EOD waveforms of pulse-type fish corresponding to `pulse_names`.
-        First column of a waveform is time in seconds, second column is the EOD waveform.
+        List of EOD waveforms of pulse-type fish corresponding to
+        `pulse_names`.  First column of a waveform is time in seconds,
+        second column is the EOD waveform.
     """
-    if len(species_file) == 0 or species_file == 'none' or not os.path.isfile(species_file):
+    if len(species_file) == 0 or species_file == 'none' or \
+       not os.path.isfile(species_file):
         return [], [], [], []
     wave_names = []
     wave_eods = []
     pulse_names = []
     pulse_eods = []
     fish_type = 'wave'
     with open(species_file, 'r') as sf:
@@ -1041,15 +1111,14 @@
         set the EOD frequency to one (default).
 
     Returns
     -------
     rmse: float
         Root-mean-squared difference between the two EOD waveforms relative to
         their standard deviation over one period.
-
     """
     # copy:
     eod1 = np.array(eod1[:,:2])
     eod2 = np.array(eod2[:,:2])
     # scale to multiples of EOD period:
     eod1[:,0] *= eod1f
     eod2[:,0] *= eod2f
@@ -1128,17 +1197,16 @@
     wfac: float
         Multiply the distance between minimum and maximum by this factor
         to get the window size over which to compute the rms difference.
 
     Returns
     -------
     rmse: float
-        Root-mean-squared difference between the two EOD waveforms relative to
-        their standard deviation over the analysis window.
-
+        Root-mean-squared difference between the two EOD waveforms
+        relative to their standard deviation over the analysis window.
     """
     # copy:
     eod1 = np.array(eod1[:,:2])
     eod2 = np.array(eod2[:,:2])
     # width of the pulses:
     imin1 = np.argmin(eod1[:,1])
     imax1 = np.argmax(eod1[:,1])
@@ -1201,87 +1269,94 @@
     max_clip: float
         Maximum amplitude that is not clipped.
     
     Returns
     -------
     clipped_frac: float
         Fraction of snippets that are clipped.
-
     """
     # snippets:
     idx0 = np.argmin(np.abs(mean_eod[:,0])) # index of time zero
     w0 = -idx0
     w1 = len(mean_eod[:,0]) - idx0
-    eod_idx = np.round(eod_times * samplerate).astype(np.int)
+    eod_idx = np.round(eod_times * samplerate).astype(int)
     eod_snippets = snippets(data, eod_idx, w0, w1)
     # fraction of clipped snippets:
     clipped_frac = np.sum(np.any((eod_snippets > max_clip) |
                                  (eod_snippets < min_clip), axis=1))\
                    / len(eod_snippets)
     return clipped_frac
 
 
-def wave_quality(props, harm_relampl=None, min_freq=0.0, max_freq=2000.0, max_clipped_frac=0.1,
+def wave_quality(props, harm_relampl=None, min_freq=0.0,
+                 max_freq=2000.0, max_clipped_frac=0.1,
                  max_crossings=4, max_rms_sem=0.0, max_rms_error=0.05,
-                 min_power=-100.0, max_thd=0.0, max_db_diff=20.0, max_harmonics_db=-5.0,
-                 max_relampl_harm1=0.0, max_relampl_harm2=0.0, max_relampl_harm3=0.0):
-    """
-    Assess the quality of an EOD waveform of a wave fish.
+                 min_power=-100.0, max_thd=0.0, max_db_diff=20.0,
+                 max_harmonics_db=-5.0, max_relampl_harm1=0.0,
+                 max_relampl_harm2=0.0, max_relampl_harm3=0.0):
+    """Assess the quality of an EOD waveform of a wave fish.
     
     Parameters
     ----------
     props: dict
         A dictionary with properties of the analyzed EOD waveform
         as returned by `analyze_wave()`.
     harm_relampl: 1-D array of floats or None
-        Relative amplitude of at least the first 3 harmonics without the fundamental.
+        Relative amplitude of at least the first 3 harmonics without
+        the fundamental.
     min_freq: float
         Minimum EOD frequency (`props['EODf']`).
     max_freq: float
         Maximum EOD frequency (`props['EODf']`).
     max_clipped_frac: float
-        If larger than zero, maximum allowed fraction of clipped data (`props['clipped']`).
+        If larger than zero, maximum allowed fraction of clipped data
+        (`props['clipped']`).
     max_crossings: int
         If larger than zero, maximum number of zero crossings per EOD period
         (`props['ncrossings']`).
     max_rms_sem: float
-        If larger than zero, maximum allowed standard error of the data relative
-        to p-p amplitude (`props['rmssem']`).
+        If larger than zero, maximum allowed standard error of the
+        data relative to p-p amplitude (`props['noise']`).
     max_rms_error: float
-        If larger than zero, maximum allowed root-mean-square error between EOD waveform and
-        Fourier fit relative to p-p amplitude (`props['rmserror']`).
+        If larger than zero, maximum allowed root-mean-square error
+        between EOD waveform and Fourier fit relative to p-p amplitude
+        (`props['rmserror']`).
     min_power: float
         Minimum power of the EOD in dB (`props['power']`).
     max_thd: float
-        If larger than zero, then maximum total harmonic distortion (`props['thd']`).
+        If larger than zero, then maximum total harmonic distortion
+        (`props['thd']`).
     max_db_diff: float
         If larger than zero, maximum standard deviation of differences between
         logarithmic powers of harmonics in decibel (`props['dbdiff']`).
         Low values enforce smoother power spectra.
     max_harmonics_db:
-        Maximum power of higher harmonics relative to peak power in decibel (`props['maxdb']`).
+        Maximum power of higher harmonics relative to peak power in
+        decibel (`props['maxdb']`).
     max_relampl_harm1: float
         If larger than zero, maximum allowed amplitude of first harmonic
         relative to fundamental.
     max_relampl_harm2: float
         If larger than zero, maximum allowed amplitude of second harmonic
         relative to fundamental.
     max_relampl_harm3: float
         If larger than zero, maximum allowed amplitude of third harmonic
         relative to fundamental.
                                        
     Returns
     -------
     remove: bool
-        If True then this is most likely not an electric fish. Remove it from
-        both the waveform properties and the list of EOD frequencies.
-        If False, keep it in the list of EOD frequencies, but remove it from the
-        waveform properties if `skip_reason` is not empty.
+        If True then this is most likely not an electric fish. Remove
+        it from both the waveform properties and the list of EOD
+        frequencies.  If False, keep it in the list of EOD
+        frequencies, but remove it from the waveform properties if
+        `skip_reason` is not empty.
     skip_reason: string
-        An empty string if the waveform is good, otherwise a string indicating the failure.
+        An empty string if the waveform is good, otherwise a string
+        indicating the failure.
     msg: string
         A textual representation of the values tested.
     """
     remove = False
     msg = []
     skip_reason = []
     # EOD frequency:
@@ -1364,31 +1439,32 @@
                 num_str = ['First', 'Second', 'Third']
                 skip_reason += ['distorted ampl%d=%5.1f%% (maximum%sHarmonicAmplitude=%5.1f%%)' %
                                 (k+1, 100.0*harm_relampl[k], num_str[k], 100.0*max_relampl)]
     return remove, ', '.join(skip_reason), ', '.join(msg)
 
 
 def pulse_quality(props, max_clipped_frac=0.1, max_rms_sem=0.0):
-    """
-    Assess the quality of an EOD waveform of a pulse fish.
+    """Assess the quality of an EOD waveform of a pulse fish.
     
     Parameters
     ----------
     props: dict
         A dictionary with properties of the analyzed EOD waveform
         as returned by `analyze_pulse()`.
     max_clipped_frac: float
         Maximum allowed fraction of clipped data.
     max_rms_sem: float
-        If not zero, maximum allowed standard error of the data relative to p-p amplitude.
+        If not zero, maximum allowed standard error of the data
+        relative to p-p amplitude.
 
     Returns
     -------
     skip_reason: string
-        An empty string if the waveform is good, otherwise a string indicating the failure.
+        An empty string if the waveform is good, otherwise a string
+        indicating the failure.
     msg: string
         A textual representation of the values tested.
     skipped_clipped: bool
         True if waveform was skipped because of clipping.
     """
     msg = []
     skip_reason = []
@@ -1411,31 +1487,30 @@
         msg += ['rms sem waveform=%6.2f%%' % (100.0*rms_sem)]
         if max_rms_sem > 0.0 and rms_sem >= max_rms_sem:
             skip_reason += ['noisy waveform s.e.m.=%6.2f%% (maximumRMSNoise=%6.2f%%)' %
                             (100.0*rms_sem, 100.0*max_rms_sem)]
     return ', '.join(skip_reason), ', '.join(msg), skipped_clipped
 
 
-def plot_eod_recording(ax, data, samplerate, width=0.1, unit=None, toffs=0.0,
-                       kwargs={'lw': 2, 'color': 'red'}):
-    """
-    Plot a zoomed in range of the recorded trace.
+def plot_eod_recording(ax, data, samplerate, unit=None, width=0.1,
+                       toffs=0.0, kwargs={'lw': 2, 'color': 'red'}):
+    """Plot a zoomed in range of the recorded trace.
 
     Parameters
     ----------
     ax: matplotlib axes
         Axes used for plotting.
     data: 1D ndarray
-        Recorded data.
+        Recorded data to be plotted.
     samplerate: float
         Sampling rate of the data in Hertz.
-    width: float
-        Width of data segment to be plotted in seconds.
     unit: string
         Optional unit of the data used for y-label.
+    width: float
+        Width of data segment to be plotted in seconds.
     toffs: float
         Time of first data value in seconds.
     kwargs: dict
         Arguments passed on to the plot command for the recorded trace.
     """
     widx2 = int(width*samplerate)//2
     i0 = len(data)//2 - widx2
@@ -1460,32 +1535,36 @@
     ax.set_ylim(ymin-0.05*dy, ymax+0.05*dy)
     if len(unit) == 0 or unit == 'a.u.':
         ax.set_ylabel('Amplitude')
     else:
         ax.set_ylabel('Amplitude [%s]' % unit)
 
 
-def plot_pulse_eods(ax, data, samplerate, zoom_window, width, eod_props, toffs=0.0,
-                    colors=None, markers=None, marker_size=10,
+def plot_pulse_eods(ax, data, samplerate, zoom_window, width, eod_props,
+                    toffs=0.0, colors=None, markers=None, marker_size=10,
                     legend_rows=8, **kwargs):
-    """
-    Mark pulse EODs in a plot of an EOD recording.
+    """Mark pulse EODs in a plot of an EOD recording.
 
     Parameters
     ----------
     ax: matplotlib axes
         Axes used for plotting.
     data: 1D ndarray
         Recorded data (these are not plotted!).
     samplerate: float
         Sampling rate of the data in Hertz.
+    zoom_window: tuple of floats
+       Start and end time of the data to be plotted in seconds.
+    width: float
+       Minimum width of the data to be plotted in seconds.
     eod_props: list of dictionaries
-            Lists of EOD properties as returned by `analyze_pulse()` and `analyze_wave()`.
-            From the entries with 'type' == 'pulse' the properties 'EODf' and 'times'
-            are used. 'EODf' is the averaged EOD frequency, and 'times' is a list of
+            Lists of EOD properties as returned by `analyze_pulse()`
+            and `analyze_wave()`.  From the entries with 'type' ==
+            'pulse' the properties 'EODf' and 'times' are used. 'EODf'
+            is the averaged EOD frequency, and 'times' is a list of
             detected EOD pulse times.
     toffs: float
         Time of first data value in seconds that will be added
         to the pulse times in `eod_props`.
     colors: list of colors or None
             If not None list of colors for plotting each cluster
     markers: list of markers or None
@@ -1502,34 +1581,37 @@
         if eod['type'] != 'pulse':
             continue
         if 'times' not in eod:
             continue
 
         width = np.min([width, np.diff(zoom_window)[0]])
         while len(eod['peaktimes'][(eod['peaktimes']>(zoom_window[1]-width)) & (eod['peaktimes']<(zoom_window[1]))]) == 0:
-            width = width*2
+            width *= 2
             if zoom_window[1] - width < 0:
                 width = width/2
                 break  
 
         x = eod['peaktimes'] + toffs
-        y = data[np.round(eod['peaktimes']*samplerate).astype(np.int)]
+        pidx = np.round(eod['peaktimes']*samplerate).astype(int)
+        y = data[pidx[(pidx>0)&(pidx<len(data))]]
+        x = x[(pidx>0)&(pidx<len(data))]
         color_kwargs = {}
         #if colors is not None:
         #    color_kwargs['color'] = colors[k%len(colors)]
         if marker_size is not None:
             color_kwargs['ms'] = marker_size
         label = '%6.1f Hz' % eod['EODf']
         if legend_rows > 5 and k >= legend_rows:
             label = None
         if markers is None:
             ax.plot(x, y, 'o', label=label, zorder=-1, **color_kwargs)
         else:
             ax.plot(x, y, linestyle='none', label=label,
-                    marker=markers[k%len(markers)], mec=None, mew=0.0, zorder=-1, **color_kwargs)
+                    marker=markers[k%len(markers)], mec=None, mew=0.0,
+                    zorder=-1, **color_kwargs)
         k += 1
 
     # legend:
     if k > 1:
         if legend_rows > 0:
             if legend_rows > 5:
                 ncol = 1
@@ -1548,18 +1630,19 @@
 
         ymin = np.min(data[i0:i1])
         ymax = np.max(data[i0:i1])
         dy = ymax - ymin
         ax.set_ylim(ymin-0.05*dy, ymax+0.05*dy)
 
         
-def plot_eod_snippets(ax, data, samplerate, tmin, tmax, eod_times, n_snippets=10, flip=False,
-                      kwargs={'zorder': -5, 'scaley': False, 'lw': 0.5, 'color': '#CCCCCC'}):
-    """
-    Plot a few EOD waveform snippets.
+def plot_eod_snippets(ax, data, samplerate, tmin, tmax, eod_times,
+                      n_snippets=10, flip=False,
+                      kwargs={'zorder': -5, 'scaley': False,
+                              'lw': 0.5, 'color': '#CCCCCC'}):
+    """Plot a few EOD waveform snippets.
 
     Parameters
     ----------
     ax: matplotlib axes
         Axes used for plotting.
     data: 1D ndarray
         Recorded data from which the snippets are taken.
@@ -1594,69 +1677,72 @@
         if flip:
             snippet *= -1
         ax.plot(time, snippet - np.mean(snippet[:len(snippet)//4]), **kwargs)
 
         
 def plot_eod_waveform(ax, eod_waveform, props, peaks=None, unit=None,
                       mkwargs={'zorder': 10, 'lw': 2, 'color': 'red'},
-                      skwargs={'zorder': 5, 'color': '#CCCCCC'},
-                      fkwargs={'zorder': 0, 'lw': 6, 'color': 'steelblue'},
-                      zkwargs={'zorder': -10, 'lw': 1, 'color': '#AAAAAA'}):
-    """
-    Plot mean EOD, its standard error, and an optional fit to the EOD.
+                      skwargs={'zorder': -10, 'color': '#CCCCCC'},
+                      fkwargs={'zorder': 5, 'lw': 6, 'color': 'steelblue'},
+                      zkwargs={'zorder': -5, 'lw': 1, 'color': '#AAAAAA'}):
+    """Plot mean EOD, its standard error, and an optional fit to the EOD.
 
     Parameters
     ----------
     ax: matplotlib axes
         Axes used for plotting.
     eod_waveform: 2-D array
-        EOD waveform. First column is time in seconds,
-        second column the (mean) eod waveform. The optional third column is the
-        standard error, and the optional fourth column is a fit on the waveform.
+        EOD waveform. First column is time in seconds, second column
+        the (mean) eod waveform. The optional third column is the
+        standard error, and the optional fourth column is a fit on the
+        waveform.
     props: dict
         A dictionary with properties of the analyzed EOD waveform as
         returned by `analyze_wave()` and `analyze_pulse()`.
     peaks: 2_D arrays or None
         List of peak properties (index, time, and amplitude) of a EOD pulse
         as returned by `analyze_pulse()`.
     unit: string
         Optional unit of the data used for y-label.
     mkwargs: dict
         Arguments passed on to the plot command for the mean EOD.
     skwargs: dict
-        Arguments passed on to the fill_between command for the standard error of the EOD.
+        Arguments passed on to the fill_between command for the
+        standard error of the EOD.
     fkwargs: dict
         Arguments passed on to the plot command for the fitted EOD.
     zkwargs: dict
         Arguments passed on to the plot command for the zero line.
     """
     ax.autoscale(True)
     time = 1000.0 * eod_waveform[:,0]
     # plot zero line:
-    ax.plot([time[0], time[-1]], [0.0, 0.0], **zkwargs)
+    ax.axhline(0.0, **zkwargs)
     # plot fit:
     if eod_waveform.shape[1] > 3:
         ax.plot(time, eod_waveform[:,3], **fkwargs)
     # plot waveform:
     mean_eod = eod_waveform[:,1]
     ax.plot(time, mean_eod, **mkwargs)
     # plot standard error:
     if eod_waveform.shape[1] > 2:
         std_eod = eod_waveform[:,2]
         if np.mean(std_eod)/(np.max(mean_eod) - np.min(mean_eod)) > 0.1:
+            ax.autoscale_view(False)
             ax.autoscale(False)
-        ax.fill_between(time, mean_eod + std_eod, mean_eod - std_eod, **skwargs)
+        ax.fill_between(time, mean_eod + std_eod, mean_eod - std_eod,
+                        **skwargs)
     # ax height dimensions:
     pixely = np.abs(np.diff(ax.get_window_extent().get_points()[:,1]))[0]
     ymin, ymax = ax.get_ylim()
     unity = ymax - ymin
     dyu = np.abs(unity)/pixely
     font_size = plt.rcParams['font.size']*dyu
     # annotate fit:
-    tau = props['tau'] if 'tau' in props else None
+    tau = None if props is None else props.get('tau', None)
     ty = 0.0
     if tau is not None and eod_waveform.shape[1] > 3:
         if tau < 0.001:
             label = u'\u03c4=%.0f\u00b5s' % (1.e6*tau)
         else:
             label = u'\u03c4=%.2fms' % (1.e3*tau)
         inx = np.argmin(np.isnan(eod_waveform[:,3]))
@@ -1700,86 +1786,94 @@
                 dy = ymin + 1.3*font_size - p[2]
             sign = np.sign(p[2])
             if p[0] == np.max(peaks[:,0]) and ty*p[2] > 0.0 and \
                sign*p[2]+dy < sign*ty+1.2*font_size:
                 dy = ty + sign*1.2*font_size - p[2]
             dx = 0.05*time[-1]
             if p[1] >= 0.0:
-                ax.text(1000.0*p[1]+dx, p[2]+dy, label, ha='left', va=va, zorder=20)
+                ax.text(1000.0*p[1]+dx, p[2]+dy, label,
+                        ha='left', va=va, zorder=20)
             else:
-                ax.text(1000.0*p[1]-dx, p[2]+dy, label, ha='right', va=va, zorder=20)
+                ax.text(1000.0*p[1]-dx, p[2]+dy, label,
+                        ha='right', va=va, zorder=20)
     # annotate plot:
     if unit is None or len(unit) == 0 or unit == 'a.u.':
         unit = ''
-    props['unit'] = unit
-    label = 'p-p amplitude = {p-p-amplitude:.3g} {unit}\n'.format(**props)
-    if 'n' in props:
-        props['eods'] = 'EODs' if props['n'] > 1 else 'EOD'
-        label += 'n = {n} {eods}\n'.format(**props)
-    if props['flipped']:
-        label += 'flipped\n'
-    if -eod_waveform[0,0] < 0.6*eod_waveform[-1,0]:
-        ax.text(0.97, 0.97, label, transform = ax.transAxes, va='top', ha='right')
-    else:
-        ax.text(0.03, 0.97, label, transform = ax.transAxes, va='top')
+    if props is not None:
+        props['unit'] = unit
+        label = 'p-p amplitude = {p-p-amplitude:.3g} {unit}\n'.format(**props)
+        if 'n' in props:
+            props['eods'] = 'EODs' if props['n'] > 1 else 'EOD'
+            label += 'n = {n} {eods}\n'.format(**props)
+        if props['flipped']:
+            label += 'flipped\n'
+        if -eod_waveform[0,0] < 0.6*eod_waveform[-1,0]:
+            ax.text(0.97, 0.97, label, transform=ax.transAxes,
+                    va='top', ha='right', zorder=20)
+        else:
+            ax.text(0.03, 0.97, label, transform=ax.transAxes,
+                    va='top', zorder=20)
     # axis:                
-    if props['type'] == 'wave':
+    if props is not None and props['type'] == 'wave':
         lim = 750.0/props['EODf']
         ax.set_xlim([-lim, +lim])
     else:
         ax.set_xlim(time[0], time[-1])
     ax.set_xlabel('Time [msec]')
     if unit:
         ax.set_ylabel('Amplitude [%s]' % unit)
     else:
         ax.set_ylabel('Amplitude')
 
 
-def plot_wave_spectrum(axa, axp, spec, props, unit=None, color='b', lw=2, markersize=10):
+def plot_wave_spectrum(axa, axp, spec, props, unit=None,
+                       color='b', lw=2, markersize=10):
     """Plot and annotate spectrum of wave EOD.
 
     Parameters
     ----------
     axa: matplotlib axes
         Axes for amplitude plot.
     axp: matplotlib axes
         Axes for phase plot.
     spec: 2-D array
-        The amplitude spectrum of a single pulse as returned by `analyze_wave()`.
-        First column is the index of the harmonics, second column its frequency,
-        third column its amplitude, fourth column its amplitude relative to the fundamental,
-        fifth column is power of harmonics relative to fundamental in decibel,
-        and sixth column the phase shift relative to the fundamental.
+        The amplitude spectrum of a single pulse as returned by
+        `analyze_wave()`.  First column is the index of the harmonics,
+        second column its frequency, third column its amplitude,
+        fourth column its amplitude relative to the fundamental, fifth
+        column is power of harmonics relative to fundamental in
+        decibel, and sixth column the phase shift relative to the
+        fundamental.
     props: dict
         A dictionary with properties of the analyzed EOD waveform as
         returned by `analyze_wave()`.
     unit: string
         Optional unit of the data used for y-label.
     color:
         Color for line and points of spectrum.
     lw: float
         Linewidth for spectrum.
     markersize: float
         Size of points on spectrum.
     """
-    n = 9 if len(spec) > 9 else len(spec)
+    n = min(9, np.sum(np.isfinite(spec[:,2])))
     # amplitudes:
     markers, stemlines, _ = axa.stem(spec[:n,0]+1, spec[:n,2], basefmt='none')
     plt.setp(markers, color=color, markersize=markersize, clip_on=False)
     plt.setp(stemlines, color=color, lw=lw)
     axa.set_xlim(0.5, n+0.5)
     axa.set_ylim(bottom=0)
     axa.xaxis.set_major_locator(plt.MultipleLocator(1))
     axa.tick_params('x', direction='out')
     if unit:
         axa.set_ylabel('Amplitude [%s]' % unit)
     else:
         axa.set_ylabel('Amplitude')
     # phases:
-    phases = spec[:,5]
+    phases = spec[:n,5]
     phases[phases<0.0] = phases[phases<0.0] + 2.0*np.pi
     markers, stemlines, _ = axp.stem(spec[:n,0]+1, phases[:n], basefmt='none')
     plt.setp(markers, color=color, markersize=markersize, clip_on=False)
     plt.setp(stemlines, color=color, lw=lw)
     axp.set_xlim(0.5, n+0.5)
     axp.xaxis.set_major_locator(plt.MultipleLocator(1))
     axp.tick_params('x', direction='out')
@@ -1814,86 +1908,88 @@
         Linewidth for spectrum.
     markersize: float
         Size of points on spectrum.
     """
     box = mpatches.Rectangle((1,-60), 49, 60, linewidth=0, facecolor='#DDDDDD',
                              zorder=1)
     ax.add_patch(box)
-    att = props['lowfreqattenuation50']
+    att = props['poweratt50']
     if att < -5.0:
         ax.text(10.0, att+1.0, '%.0f dB' % att, ha='left', va='bottom', zorder=10)
     else:
         ax.text(10.0, att-1.0, '%.0f dB' % att, ha='left', va='top', zorder=10)
     box = mpatches.Rectangle((1,-60), 4, 60, linewidth=0, facecolor='#CCCCCC',
                              zorder=2)
     ax.add_patch(box)
-    att = props['lowfreqattenuation5']
+    att = props['poweratt5']
     if att < -5.0:
         ax.text(4.0, att+1.0, '%.0f dB' % att, ha='right', va='bottom', zorder=10)
     else:
         ax.text(4.0, att-1.0, '%.0f dB' % att, ha='right', va='top', zorder=10)
-    lowcutoff = props['powerlowcutoff']
+    lowcutoff = props['lowcutoff']
     if lowcutoff >= min_freq:
         ax.plot([lowcutoff, lowcutoff, 1.0], [-60.0, 0.5*att, 0.5*att], '#BBBBBB',
                 zorder=3)
         ax.text(1.2*lowcutoff, 0.5*att-1.0, '%.0f Hz' % lowcutoff, ha='left', va='top', zorder=10)
     db = decibel(power[:,1])
     smax = np.nanmax(db)
     ax.plot(power[:,0], db - smax, color, lw=lw, zorder=4)
-    peakfreq = props['peakfrequency']
+    peakfreq = props['peakfreq']
     if peakfreq >= min_freq:
         ax.scatter([peakfreq], [0.0], c=color, edgecolors=color, s=markersize, alpha=0.4, zorder=5)
         ax.text(peakfreq*1.2, 1.0, '%.0f Hz' % peakfreq, va='bottom', zorder=10)
     ax.set_xlim(min_freq, max_freq)
     ax.set_xscale('log')
     ax.set_ylim(-60.0, 2.0)
     ax.set_xlabel('Frequency [Hz]')
     ax.set_ylabel('Power [dB]')
 
-
+    
 def save_eod_waveform(mean_eod, unit, idx, basename, **kwargs):
-    """ Save mean EOD waveform to file.
+    """Save mean EOD waveform to file.
 
     Parameters
     ----------
     mean_eod: 2D array of floats
-        Averaged EOD waveform as returned by `eod_waveform()`, `analyze_wave()`,
-        and `analyze_pulse()`.
+        Averaged EOD waveform as returned by `eod_waveform()`,
+        `analyze_wave()`, and `analyze_pulse()`.
     unit: string
         Unit of the waveform data.
     idx: int or None
         Index of fish.
-    basename: string
-        Path and basename of file.
+    basename: string or stream
+        If string, path and basename of file.
         '-eodwaveform', the fish index, and a file extension are appended.
+        If stream, write EOD waveform data into this stream.
     kwargs:
         Arguments passed on to `TableData.write()`.
 
     Returns
     -------
     filename: string
-        The path and full name of the written file.
+        Path and full name of the written file in case of `basename`
+        being a string. Otherwise, the file name and extension that
+        would have been appended to a basename.
 
     See Also
     --------
     load_eod_waveform()
     """
     td = TableData(mean_eod[:,:3]*[1000.0, 1.0, 1.0], ['time', 'mean', 'sem'],
                    ['ms', unit, unit], ['%.3f', '%.5f', '%.5f'])
     if mean_eod.shape[1] > 3:
         td.append('fit', unit, '%.5f', mean_eod[:,3])
-    fp = basename + '-eodwaveform'
+    fp = '-eodwaveform'
     if idx is not None:
         fp += '-%d' % idx
-    file_name = td.write(fp, **kwargs)
-    return file_name
+    return td.write_file_stream(basename, fp, **kwargs)
 
 
 def load_eod_waveform(file_path):
-    """ Load EOD waveform from file.
+    """Load EOD waveform from file.
 
     Parameters
     ----------
     file_path: string
         Path of the file to be loaded.
 
     Returns
@@ -1915,150 +2011,174 @@
     data = TableData(file_path)
     mean_eod = data.array()
     mean_eod[:,0] *= 0.001
     return mean_eod, data.unit('mean')
 
 
 def save_wave_eodfs(wave_eodfs, wave_indices, basename, **kwargs):
-    """ Save frequencies of wave EODs to file.
+    """Save frequencies of wave EODs to file.
 
     Parameters
     ----------
     wave_eodfs: list of 2D arrays
-        Each item is a matrix with the frequencies and powers (columns) of the
-        fundamental and harmonics (rows) as returned by `harmonics.harmonic_groups()`.
+        Each item is a matrix with the frequencies and powers
+        (columns) of the fundamental and harmonics (rows) as returned
+        by `harmonics.harmonic_groups()`.
     wave_indices: array
         Indices identifying each fish or NaN.
         If None no index column is inserted.
-    basename: string
-        Path and basename of file.
+    basename: string or stream
+        If string, path and basename of file.
         '-waveeodfs' and a file extension are appended.
+        If stream, write EOD frequencies data into this stream.
     kwargs:
         Arguments passed on to `TableData.write()`.
 
     Returns
     -------
     filename: string
-        The path and full name of the written file.
+        Path and full name of the written file in case of `basename`
+        being a string. Otherwise, the file name and extension that
+        would have been appended to a basename.
 
     See Also
     --------
     load_wave_eodfs()
+
     """
     eodfs = fundamental_freqs_and_power(wave_eodfs)
     td = TableData()
     if wave_indices is not None:
         td.append('index', '', '%d', [wi if wi >= 0 else np.nan for wi in wave_indices])
     td.append('EODf', 'Hz', '%7.2f', eodfs[:,0])
     td.append('datapower', 'dB', '%7.2f', eodfs[:,1])
-    fp = basename + '-waveeodfs'
-    file_name = td.write(fp, **kwargs)
-    return file_name
+    fp = '-waveeodfs'
+    return td.write_file_stream(basename, fp, **kwargs)
 
 
 def load_wave_eodfs(file_path):
-    """ Load frequencies of wave EODs from file.
+    """Load frequencies of wave EODs from file.
 
     Parameters
     ----------
     file_path: string
         Path of the file to be loaded.
 
     Returns
     -------
     eodfs: 2D array of floats
-        Indices, EODfs, and power of wave type fish.
+        EODfs and power of wave type fish.
         Indices can contain NaNs.
+    indices: array of ints
+        Corresponding indices of fish, can contain negative numbers to
+        indicate frequencies without fish.
 
     Raises
     ------
     FileNotFoundError:
         If `file_path` does not exist.
 
     See Also
     --------
     save_wave_eodfs()
     """
     data = TableData(file_path)
     eodfs = data.array()
-    if not 'index' in data:
-        indices = np.empty(data.rows())
-        indices[:] = np.nan
-        eodfs = np.column_stack((indices, eodfs))
-    return eodfs
+    if 'index' in data:
+        indices = data[:,'index']
+        indices[~np.isfinite(indices)] = -1
+        indices = np.array(indices, dtype=int)
+        eodfs = eodfs[:,1:]
+    else:
+        indices = np.zeros(data.rows(), dtype=int) - 1
+    return eodfs, indices
 
     
 def save_wave_fish(eod_props, unit, basename, **kwargs):
-    """ Save properties of wave EODs to file.
+    """Save properties of wave EODs to file.
 
     Parameters
     ----------
     eod_props: list of dict
-        Properties of EODs as returned by `analyze_wave()` and `analyze_pulse()`.
-        Only properties of wave fish are saved.
+        Properties of EODs as returned by `analyze_wave()` and
+        `analyze_pulse()`.  Only properties of wave fish are saved.
     unit: string
         Unit of the waveform data.
-    basename: string
-        Path and basename of file.
+    basename: string or stream
+        If string, path and basename of file.
         '-wavefish' and a file extension are appended.
+        If stream, write wave fish properties into this stream.
     kwargs:
         Arguments passed on to `TableData.write()`.
 
     Returns
     -------
     filename: string or None
-        The path and full name of the written file.
-        None if no pulse fish are contained in eod_props and no file was written.
+        Path and full name of the written file in case of `basename`
+        being a string. Otherwise, the file name and extension that
+        would have been appended to a basename.
+        None if no wave fish are contained in eod_props and
+        consequently no file was written.
 
     See Also
     --------
     load_wave_fish()
     """
     wave_props = [p for p in eod_props if p['type'] == 'wave']
     if len(wave_props) == 0:
         return None
     td = TableData()
-    if 'tstart' in wave_props[0]:
+    if 'twin' in wave_props[0] or 'samplerate' in wave_props[0] or \
+       'nfft' in wave_props[0]:
         td.append_section('recording')
-        td.append('tstart', 's', '%7.2f', wave_props, 'tstart')
-        td.append('twindow', 's', '%7.2f', wave_props, 'twindow')
+    if 'twin' in wave_props[0]:
+        td.append('twin', 's', '%7.2f', wave_props)
+        td.append('window', 's', '%7.2f', wave_props)
+        td.append('winclipped', '%', '%.2f', wave_props, 100.0)
+    if 'samplerate' in wave_props[0]:
+        td.append('samplerate', 'kHz', '%.3f', wave_props, 0.001)
+    if 'nfft' in wave_props[0]:
+        td.append('nfft', '', '%d', wave_props)
+        td.append('dfreq', 'Hz', '%.2f', wave_props)
     td.append_section('waveform')
-    td.append('index', '', '%d', wave_props, 'index')
-    td.append('EODf', 'Hz', '%7.2f', wave_props, 'EODf')
-    td.append('p-p-amplitude', unit, '%.5f', wave_props, 'p-p-amplitude')
-    td.append('power', 'dB', '%7.2f', wave_props, 'power')
+    td.append('index', '', '%d', wave_props)
+    td.append('EODf', 'Hz', '%7.2f', wave_props)
+    td.append('p-p-amplitude', unit, '%.5f', wave_props)
+    td.append('power', 'dB', '%7.2f', wave_props)
     if 'datapower' in wave_props[0]:
-        td.append('datapower', 'dB', '%7.2f', wave_props, 'datapower')
-    td.append('thd', '%', '%.2f', wave_props, 'thd', 100.0)
-    td.append('dbdiff', 'dB', '%7.2f', wave_props, 'dbdiff')
-    td.append('maxdb', 'dB', '%7.2f', wave_props, 'maxdb')
-    if 'rmssem' in wave_props[0]:
-        td.append('noise', '%', '%.1f', wave_props, 'rmssem', 100.0)
-    td.append('rmserror', '%', '%.2f', wave_props, 'rmserror', 100.0)
+        td.append('datapower', 'dB', '%7.2f', wave_props)
+    td.append('thd', '%', '%.2f', wave_props, 100.0)
+    td.append('dbdiff', 'dB', '%7.2f', wave_props)
+    td.append('maxdb', 'dB', '%7.2f', wave_props)
+    if 'noise' in wave_props[0]:
+        td.append('noise', '%', '%.1f', wave_props, 100.0)
+    td.append('rmserror', '%', '%.2f', wave_props, 100.0)
     if 'clipped' in wave_props[0]:
-        td.append('clipped', '%', '%.1f', wave_props, 'clipped', 100.0)
-    td.append('flipped', '', '%d', wave_props, 'flipped')
-    td.append('n', '', '%5d', wave_props, 'n')
+        td.append('clipped', '%', '%.1f', wave_props, 100.0)
+    td.append('flipped', '', '%d', wave_props)
+    td.append('n', '', '%5d', wave_props)
     td.append_section('timing')
-    td.append('ncrossings', '', '%d', wave_props, 'ncrossings')
-    td.append('peakwidth', '%', '%.2f', wave_props, 'peakwidth', 100.0)
-    td.append('troughwidth', '%', '%.2f', wave_props, 'troughwidth', 100.0)
-    td.append('leftpeak', '%', '%.2f', wave_props, 'leftpeak', 100.0)
-    td.append('rightpeak', '%', '%.2f', wave_props, 'rightpeak', 100.0)
-    td.append('lefttrough', '%', '%.2f', wave_props, 'lefttrough', 100.0)
-    td.append('righttrough', '%', '%.2f', wave_props, 'righttrough', 100.0)
-    td.append('p-p-distance', '%', '%.2f', wave_props, 'p-p-distance', 100.0)
-    td.append('reltroughampl', '%', '%.2f', wave_props, 'reltroughampl', 100.0)
-    fp = basename + '-wavefish'
-    file_name = td.write(fp, **kwargs)
-    return file_name
+    td.append('ncrossings', '', '%d', wave_props)
+    td.append('peakwidth', '%', '%.2f', wave_props, 100.0)
+    td.append('troughwidth', '%', '%.2f', wave_props, 100.0)
+    td.append('leftpeak', '%', '%.2f', wave_props, 100.0)
+    td.append('rightpeak', '%', '%.2f', wave_props, 100.0)
+    td.append('lefttrough', '%', '%.2f', wave_props, 100.0)
+    td.append('righttrough', '%', '%.2f', wave_props, 100.0)
+    td.append('p-p-distance', '%', '%.2f', wave_props, 100.0)
+    td.append('reltroughampl', '%', '%.2f', wave_props, 100.0)
+    fp = '-wavefish'
+    return td.write_file_stream(basename, fp, **kwargs)
 
 
 def load_wave_fish(file_path):
-    """ Load properties of wave EODs from file.
+    """Load properties of wave EODs from file.
+
+    All times are scaled to seconds, all frequencies to Hertz and all
+    percentages to fractions.
 
     Parameters
     ----------
     file_path: string
         Path of the file to be loaded.
 
     Returns
@@ -2070,104 +2190,126 @@
     ------
     FileNotFoundError:
         If `file_path` does not exist.
 
     See Also
     --------
     save_wave_fish()
+
     """
     data = TableData(file_path)
     eod_props = data.dicts()
     for props in eod_props:
+        if 'winclipped' in props:
+            props['winclipped'] /= 100
+        if 'samplerate' in props:
+            props['samplerate'] *= 1000
+        if 'nfft' in props:
+            props['nfft'] = int(props['nfft'])
+        props['index'] = int(props['index'])
+        props['n'] = int(props['n'])
         props['type'] = 'wave'
         props['thd'] /= 100
         props['noise'] /= 100
-        if 'rmssem' in props:
-            props['rmssem'] /= 100
         props['rmserror'] /= 100
         if 'clipped' in props:
             props['clipped'] /= 100
+        props['ncrossings'] = int(props['ncrossings'])
         props['peakwidth'] /= 100
         props['troughwidth'] /= 100
         props['leftpeak'] /= 100
         props['rightpeak'] /= 100
         props['lefttrough'] /= 100
         props['righttrough'] /= 100
         props['p-p-distance'] /= 100
         props['reltroughampl'] /= 100
     return eod_props
 
 
 def save_pulse_fish(eod_props, unit, basename, **kwargs):
-    """ Save properties of pulse EODs to file.
+    """Save properties of pulse EODs to file.
 
     Parameters
     ----------
     eod_props: list of dict
-        Properties of EODs as returned by `analyze_wave()` and `analyze_pulse()`.
-        Only properties of pulse fish are saved.
+        Properties of EODs as returned by `analyze_wave()` and
+        `analyze_pulse()`.  Only properties of pulse fish are saved.
     unit: string
         Unit of the waveform data.
-    basename: string
-        Path and basename of file.
+    basename: string or stream
+        If string, path and basename of file.
         '-pulsefish' and a file extension are appended.
+        If stream, write pulse fish properties into this stream.
     kwargs:
         Arguments passed on to `TableData.write()`.
 
     Returns
     -------
     filename: string or None
-        The path and full name of the written file.
-        None if no pulse fish are contained in eod_props and no file was written.
+        Path and full name of the written file in case of `basename`
+        being a string. Otherwise, the file name and extension that
+        would have been appended to a basename.
+        None if no pulse fish are contained in eod_props and
+        consequently no file was written.
 
     See Also
     --------
     load_pulse_fish()
     """
     pulse_props = [p for p in eod_props if p['type'] == 'pulse']
     if len(pulse_props) == 0:
         return None
     td = TableData()
-    if 'tstart' in pulse_props[0]:
+    if 'twin' in pulse_props[0] or 'samplerate' in pulse_props[0] or \
+       'nfft' in pulse_props[0]:
         td.append_section('recording')
-        td.append('tstart', 's', '%7.2f', pulse_props, 'tstart')
-        td.append('twindow', 's', '%7.2f', pulse_props, 'twindow')
+    if 'twin' in pulse_props[0]:
+        td.append('twin', 's', '%7.2f', pulse_props)
+        td.append('window', 's', '%7.2f', pulse_props)
+        td.append('winclipped', '%', '%.2f', pulse_props, 100.0)
+    if 'samplerate' in pulse_props[0]:
+        td.append('samplerate', 'kHz', '%.3f', pulse_props, 0.001)
+    if 'nfft' in pulse_props[0]:
+        td.append('nfft', '', '%d', pulse_props)
+        td.append('dfreq', 'Hz', '%.2f', pulse_props)
     td.append_section('waveform')
-    td.append('index', '', '%d', pulse_props, 'index')
-    td.append('EODf', 'Hz', '%7.2f', pulse_props, 'EODf')
-    td.append('period', 'ms', '%7.2f', pulse_props, 'period', 1000.0)
-    td.append('max-ampl', unit, '%.5f', pulse_props, 'max-amplitude')
-    td.append('min-ampl', unit, '%.5f', pulse_props, 'min-amplitude')
-    td.append('p-p-amplitude', unit, '%.5f', pulse_props, 'p-p-amplitude')
-    if 'rmssem' in pulse_props[0]:
-        td.append('noise', '%', '%.1f', pulse_props, 'rmssem', 100.0)
+    td.append('index', '', '%d', pulse_props)
+    td.append('EODf', 'Hz', '%7.2f', pulse_props)
+    td.append('period', 'ms', '%7.2f', pulse_props, 1000.0)
+    td.append('max-ampl', unit, '%.5f', pulse_props)
+    td.append('min-ampl', unit, '%.5f', pulse_props)
+    td.append('p-p-amplitude', unit, '%.5f', pulse_props)
+    if 'noise' in pulse_props[0]:
+        td.append('noise', '%', '%.1f', pulse_props, 100.0)
     if 'clipped' in pulse_props[0]:
-        td.append('clipped', '%', '%.1f', pulse_props, 'clipped', 100.0)
-    td.append('flipped', '', '%d', pulse_props, 'flipped')
-    td.append('tstart', 'ms', '%.3f', pulse_props, 'tstart', 1000.0)
-    td.append('tend', 'ms', '%.3f', pulse_props, 'tend', 1000.0)
-    td.append('width', 'ms', '%.3f', pulse_props, 'width', 1000.0)
-    td.append('P2-P1-dist', 'ms', '%.3f', pulse_props, 'dist', 1000.0)
-    td.append('tau', 'ms', '%.3f', pulse_props, 'tau', 1000.0)
-    td.append('firstpeak', '', '%d', pulse_props, 'firstpeak')
-    td.append('lastpeak', '', '%d', pulse_props, 'lastpeak')
-    td.append('n', '', '%d', pulse_props, 'n')
+        td.append('clipped', '%', '%.1f', pulse_props, 100.0)
+    td.append('flipped', '', '%d', pulse_props)
+    td.append('tstart', 'ms', '%.3f', pulse_props, 1000.0)
+    td.append('tend', 'ms', '%.3f', pulse_props, 1000.0)
+    td.append('width', 'ms', '%.3f', pulse_props, 1000.0)
+    td.append('P2-P1-dist', 'ms', '%.3f', pulse_props, 1000.0)
+    td.append('tau', 'ms', '%.3f', pulse_props, 1000.0)
+    td.append('firstpeak', '', '%d', pulse_props)
+    td.append('lastpeak', '', '%d', pulse_props)
+    td.append('n', '', '%d', pulse_props)
     td.append_section('power spectrum')
-    td.append('peakfreq', 'Hz', '%.2f', pulse_props, 'peakfrequency')
-    td.append('peakpower', 'dB', '%.2f', pulse_props, 'peakpower')
-    td.append('poweratt5', 'dB', '%.2f', pulse_props, 'lowfreqattenuation5')
-    td.append('poweratt50', 'dB', '%.2f', pulse_props, 'lowfreqattenuation50')
-    td.append('lowcutoff', 'Hz', '%.2f', pulse_props, 'powerlowcutoff')
-    fp = basename + '-pulsefish'
-    file_name = td.write(fp, **kwargs)
-    return file_name
+    td.append('peakfreq', 'Hz', '%.2f', pulse_props)
+    td.append('peakpower', 'dB', '%.2f', pulse_props)
+    td.append('poweratt5', 'dB', '%.2f', pulse_props)
+    td.append('poweratt50', 'dB', '%.2f', pulse_props)
+    td.append('lowcutoff', 'Hz', '%.2f', pulse_props)
+    fp = '-pulsefish'
+    return td.write_file_stream(basename, fp, **kwargs)
 
 
 def load_pulse_fish(file_path):
-    """ Load properties of pulse EODs from file.
+    """Load properties of pulse EODs from file.
+
+    All times are scaled to seconds, all frequencies to Hertz and all
+    percentages to fractions.
 
     Parameters
     ----------
     file_path: string
         Path of the file to be loaded.
 
     Returns
@@ -2179,86 +2321,100 @@
     ------
     FileNotFoundError:
         If `file_path` does not exist.
 
     See Also
     --------
     save_pulse_fish()
+
     """
     data = TableData(file_path)
     eod_props = data.dicts()
     for props in eod_props:
+        if 'winclipped' in props:
+            props['winclipped'] /= 100
+        if 'samplerate' in props:
+            props['samplerate'] *= 1000
+        if 'nfft' in props:
+            props['nfft'] = int(props['nfft'])
+        props['index'] = int(props['index'])
+        props['n'] = int(props['n'])
+        props['firstpeak'] = int(props['firstpeak'])
+        props['lastpeak'] = int(props['lastpeak'])
         props['type'] = 'pulse'
-        if 'rmssem' in props:
-            props['rmssem'] /= 100
         if 'clipped' in props:
             props['clipped'] /= 100
-        props['noise'] /= 100
         props['period'] /= 1000
+        props['noise'] /= 100
         props['tstart'] /= 1000
         props['tend'] /= 1000
         props['width'] /= 1000
         props['P2-P1-dist'] /= 1000
         props['tau'] /= 1000
     return eod_props
 
 
 def save_wave_spectrum(spec_data, unit, idx, basename, **kwargs):
-    """ Save amplitude and phase spectrum of wave EOD to file.
+    """Save amplitude and phase spectrum of wave EOD to file.
 
     Parameters
     ----------
     spec_data: 2D array of floats
-        Amplitude and phase spectrum of wave EOD as returned by `analyze_wave()`.
+        Amplitude and phase spectrum of wave EOD as returned by
+        `analyze_wave()`.
     unit: string
         Unit of the waveform data.
     idx: int or None
         Index of fish.
-    basename: string
-        Path and basename of file.
+    basename: string or stream
+        If string, path and basename of file.
         '-wavespectrum', the fish index, and a file extension are appended.
+        If stream, write wave spectrum into this stream.
     kwargs:
         Arguments passed on to `TableData.write()`.
 
     Returns
     -------
     filename: string
-        The path and full name of the written file.
+        Path and full name of the written file in case of `basename`
+        being a string. Otherwise, the file name and extension that
+        would have been appended to a basename.
 
     See Also
     --------
     load_wave_spectrum()
+
     """
     td = TableData(spec_data[:,:6]*[1.0, 1.0, 1.0, 100.0, 1.0, 1.0],
                    ['harmonics', 'frequency', 'amplitude', 'relampl', 'relpower', 'phase'],
                    ['', 'Hz', unit, '%', 'dB', 'rad'],
-                   ['%.0f', '%.2f', '%.5f', '%10.2f', '%6.2f', '%8.4f'])
+                   ['%.0f', '%.2f', '%.6f', '%10.2f', '%6.2f', '%8.4f'])
     if spec_data.shape[1] > 6:
         td.append('datapower', '%s^2/Hz' % unit, '%11.4e', spec_data[:,6])
-    fp = basename + '-wavespectrum'
+    fp = '-wavespectrum'
     if idx is not None:
         fp += '-%d' % idx
-    file_name = td.write(fp, **kwargs)
-    return file_name
+    return td.write_file_stream(basename, fp, **kwargs)
 
 
 def load_wave_spectrum(file_path):
-    """ Load amplitude and phase spectrum of wave EOD from file.
+    """Load amplitude and phase spectrum of wave EOD from file.
 
     Parameters
     ----------
     file_path: string
         Path of the file to be loaded.
 
     Returns
     -------
     spec: 2D array of floats
         Amplitude and phase spectrum of wave EOD:
         harmonics, frequency, amplitude, relative amplitude in dB,
         relative power in dB, phase, data power in unit squared.
+        Can contain NaNs.
     unit: string
         Unit of amplitudes.
 
     Raises
     ------
     FileNotFoundError:
         If `file_path` does not exist.
@@ -2270,50 +2426,52 @@
     data = TableData(file_path)
     spec = data.array()
     spec[:,3] *= 0.01
     return spec, data.unit('amplitude')
 
                         
 def save_pulse_spectrum(spec_data, unit, idx, basename, **kwargs):
-    """ Save power spectrum of pulse EOD to file.
+    """Save power spectrum of pulse EOD to file.
 
     Parameters
     ----------
     spec_data: 2D array of floats
         Power spectrum of single pulse as returned by `analyze_pulse()`.
     unit: string
         Unit of the waveform data.
     idx: int or None
         Index of fish.
-    basename: string
-        Path and basename of file.
+    basename: string or stream
+        If string, path and basename of file.
         '-pulsespectrum', the fish index, and a file extension are appended.
+        If stream, write pulse spectrum into this stream.
     kwargs:
         Arguments passed on to `TableData.write()`.
 
     Returns
     -------
     filename: string
-        The path and full name of the written file.
+        Path and full name of the written file in case of `basename`
+        being a string. Otherwise, the file name and extension that
+        would have been appended to a basename.
 
     See Also
     --------
     load_pulse_spectrum()
     """
     td = TableData(spec_data[:,:2], ['frequency', 'power'],
                    ['Hz', '%s^2/Hz' % unit], ['%.2f', '%.4e'])
-    fp = basename + '-pulsespectrum'
+    fp = '-pulsespectrum'
     if idx is not None:
         fp += '-%d' % idx
-    file_name = td.write(fp, **kwargs)
-    return file_name
+    return td.write_file_stream(basename, fp, **kwargs)
 
 
 def load_pulse_spectrum(file_path):
-    """ Load power spectrum of pulse EOD from file.
+    """Load power spectrum of pulse EOD from file.
 
     Parameters
     ----------
     file_path: string
         Path of the file to be loaded.
 
     Returns
@@ -2330,56 +2488,59 @@
     --------
     save_pulse_spectrum()
     """
     data = TableData(file_path)
     spec = data.array()
     return spec
 
-                        
+
 def save_pulse_peaks(peak_data, unit, idx, basename, **kwargs):
-    """ Save peak properties of pulse EOD to file.
+    """Save peak properties of pulse EOD to file.
 
     Parameters
     ----------
     peak_data: 2D array of floats
-        Properties of peaks and troughs of pulse EOD as returned by `analyze_pulse()`.
+        Properties of peaks and troughs of pulse EOD as returned by
+        `analyze_pulse()`.
     unit: string
         Unit of the waveform data.
     idx: int or None
         Index of fish.
-    basename: string
-        Path and basename of file.
+    basename: string or stream
+        If string, path and basename of file.
         '-pulsepeaks', the fish index, and a file extension are appended.
+        If stream, write pulse peaks into this stream.
     kwargs:
         Arguments passed on to `TableData.write()`.
 
     Returns
     -------
     filename: string
-        The path and full name of the written file.
+        Path and full name of the written file in case of `basename`
+        being a string. Otherwise, the file name and extension that
+        would have been appended to a basename.
 
     See Also
     --------
     load_pulse_peaks()
     """
     if len(peak_data) == 0:
         return None
     td = TableData(peak_data[:,:5]*[1.0, 1000.0, 1.0, 100.0, 1000.0],
                    ['P', 'time', 'amplitude', 'relampl', 'width'],
                    ['', 'ms', unit, '%', 'ms'],
                    ['%.0f', '%.3f', '%.5f', '%.2f', '%.3f'])
-    fp = basename + '-pulsepeaks'
+    fp = '-pulsepeaks'
     if idx is not None:
         fp += '-%d' % idx
-    file_name = td.write(fp, **kwargs)
-    return file_name
+    return td.write_file_stream(basename, fp, **kwargs)
 
 
 def load_pulse_peaks(file_path):
-    """ Load peak properties of pulse EOD from file.
+    """Load peak properties of pulse EOD from file.
 
     Parameters
     ----------
     file_path: string
         Path of the file to be loaded.
 
     Returns
@@ -2402,33 +2563,450 @@
     data = TableData(file_path)
     peaks = data.array()
     peaks[:,1] *= 0.001
     peaks[:,3] *= 0.01
     peaks[:,4] *= 0.001
     return peaks, data.unit('amplitude')
 
+
+def save_pulse_times(pulse_times, idx, basename, **kwargs):
+    """Save times of pulse EOD to file.
+
+    Parameters
+    ----------
+    pulse_times: dict or array of floats
+        Times of EOD pulses. Either as array of times or
+        `props['peaktimes']` or `props['times']` as returned by
+        `analyze_pulse()`.
+    idx: int or None
+        Index of fish.
+    basename: string or stream
+        If string, path and basename of file.
+        '-pulsetimes', the fish index, and a file extension are appended.
+        If stream, write pulse times into this stream.
+    kwargs:
+        Arguments passed on to `TableData.write()`.
+
+    Returns
+    -------
+    filename: string
+        Path and full name of the written file in case of `basename`
+        being a string. Otherwise, the file name and extension that
+        would have been appended to a basename.
+
+    See Also
+    --------
+    load_pulse_times()
+    """
+    if isinstance(pulse_times, dict):
+        props = pulse_times
+        pulse_times = props.get('times', [])
+        pulse_times = props.get('peaktimes', pulse_times)
+    if len(pulse_times) == 0:
+        return None
+    td = TableData()
+    td.append('time', 's', '%.4f', pulse_times)
+    fp = '-pulsetimes'
+    if idx is not None:
+        fp += '-%d' % idx
+    return td.write_file_stream(basename, fp, **kwargs)
+
+
+def load_pulse_times(file_path):
+    """Load times of pulse EOD from file.
+
+    Parameters
+    ----------
+    file_path: string
+        Path of the file to be loaded.
+
+    Returns
+    -------
+    pulse_times: array of floats
+        Times of pulse EODs in seconds.
+
+    Raises
+    ------
+    FileNotFoundError:
+        If `file_path` does not exist.
+
+    See Also
+    --------
+    save_pulse_times()
+    """
+    data = TableData(file_path)
+    pulse_times = data.array()[:,0]
+    return pulse_times
+
+
+file_types = ['waveeodfs', 'wavefish', 'pulsefish', 'eodwaveform',
+              'wavespectrum', 'pulsepeaks', 'pulsespectrum', 'pulsetimes']
+"""List of all file types generated and supported by the `save_*` and `load_*` functions."""
+
+
+def parse_filename(file_path):
+    """Parse components of an EOD analysis file name.
+
+    Analysis files generated by the `eodanalysis` module are named
+    according to
+    ```plain
+    PATH/RECORDING-CHANNEL-TIME-FTYPE-N.EXT
+    ```
+
+    Parameters
+    ----------
+    file_path: string
+        Path of the file to be parsed.
+
+    Returns
+    -------
+    recording: string
+        Path and basename of the recording, i.e. 'PATH/RECORDING'.
+        A leading './' is removed.
+    base_path: string
+        Path and basename of the analysis results,
+        i.e. 'PATH/RECORDING-CHANNEL-TIME'. A leading './' is removed.
+    channel: int
+        Channel of the recording
+        ('CHANNEL' component of the file name if present).
+        -1 if not present in `file_path`.
+    time: float
+        Start time of analysis window in seconds
+        ('TIME' component of the file name if present).
+        `None` if not present in `file_path`.
+    ftype: string
+        Type of analysis file (e.g. 'wavespectrum', 'pulsepeaks', etc.),
+        ('FTYPE' component of the file name if present).
+        See `file_types` for a list of all supported file types.
+        Empty string if not present in `file_path`.
+    index: int
+        Index of the EOD.
+        ('N' component of the file name if present).
+        -1 if not present in `file_path`.
+    ext: string
+        File extension *without* leading period
+        ('EXT' component of the file name).
+
+    """
+    name, ext = os.path.splitext(file_path)
+    ext = ext[1:]
+    parts = name.split('-')
+    index = -1
+    if len(parts) > 0 and parts[-1].isdigit():
+        index = int(parts[-1])
+        parts = parts[:-1]
+    ftype = ''
+    if len(parts) > 0:
+        ftype = parts[-1]
+        parts = parts[:-1]
+    base_path = '-'.join(parts)
+    if base_path.startswith('./'):
+        base_path = base_path[2:]
+    time = None
+    if len(parts) > 0 and len(parts[-1]) > 0 and \
+       parts[-1][0] == 't' and parts[-1][-1] == 's' and \
+       parts[-1][1:-1].isdigit():
+        time = float(parts[-1][1:-1])
+        parts = parts[:-1]
+    channel = -1
+    if len(parts) > 0 and len(parts[-1]) > 0 and \
+       parts[-1][0] == 'c' and parts[-1][1:].isdigit():
+        channel = int(parts[-1][1:])
+        parts = parts[:-1]
+    recording = '-'.join(parts)
+    if recording.startswith('./'):
+        recording = recording[2:]
+    return recording, base_path, channel, time, ftype, index, ext
+
+            
+def save_analysis(output_basename, zip_file, eod_props, mean_eods,
+                  spec_data, peak_data, wave_eodfs, wave_indices, unit,
+                  verbose, **kwargs):
+    """Save EOD analysis results to files.
+
+    Parameters
+    ----------
+    output_basename: string
+        Path and basename of files to be saved.
+    zip_file: bool
+        If `True`, write all analysis results into a zip archive.
+    eod_props: list of dict
+        Properties of EODs as returned by `analyze_wave()` and
+        `analyze_pulse()`.
+    mean_eods: list of 2D array of floats
+        Averaged EOD waveforms as returned by `eod_waveform()`,
+        `analyze_wave()`, and `analyze_pulse()`.
+    spec_data: list of 2D array of floats
+        Power spectra of single pulses as returned by
+        `analyze_pulse()`.
+    peak_data: list of 2D array of floats
+        Properties of peaks and troughs of pulse EODs as returned by
+        `analyze_pulse()`.
+    wave_eodfs: list of 2D array of float
+        Each item is a matrix with the frequencies and powers
+        (columns) of the fundamental and harmonics (rows) as returned
+        by `harmonics.harmonic_groups()`.
+    wave_indices: array of int
+        Indices identifying each fish in `wave_eodfs` or NaN.  unit:
+        string Unit of the waveform data.
+    verbose: int
+        Verbosity level.
+    kwargs:
+        Arguments passed on to `TableData.write()`.
+    """
+    def write_file_zip(zf, save_func, output, *args, **kwargs):
+        if zf is None:
+            fp = save_func(*args, basename=output, **kwargs)
+            if verbose > 0 and fp is not None:
+                print('wrote file %s' % fp)
+        else:
+            with io.StringIO() as df:
+                fp = save_func(*args, basename=df, **kwargs)
+                if fp is not None:
+                    fp = output_basename + fp
+                    zf.writestr(os.path.basename(fp), df.getvalue())
+                    if verbose > 0:
+                        print('zipped file %s' % fp)
+
+    
+    if 'table_format' in kwargs and kwargs['table_format'] == 'py':
+        with open(output_basename+'.py', 'w') as f:
+            name = os.path.basename(output_basename)
+            for k, sdata in enumerate(spec_data):
+                # save wave fish only:
+                if len(sdata)>0 and sdata.shape[1] > 2:
+                    fish = dict(amplitudes=sdata[:,3], phases=sdata[:,5])
+                    fish = normalize_wavefish(fish)
+                    export_wavefish(fish, name+'-%d_harmonics' % k, f)
+    else:
+        zf = None
+        if zip_file:
+            zf = zipfile.ZipFile(output_basename + '.zip', 'w')
+        # all wave fish in wave_eodfs:
+        if len(wave_eodfs) > 0:
+            write_file_zip(zf, save_wave_eodfs, output_basename,
+                           wave_eodfs, wave_indices, **kwargs)
+        # all wave and pulse fish:
+        for i, (mean_eod, sdata, pdata, props) in enumerate(zip(mean_eods, spec_data, peak_data, eod_props)):
+            write_file_zip(zf, save_eod_waveform, output_basename,
+                           mean_eod, unit, i, **kwargs)
+            # power spectrum:
+            if len(sdata)>0:
+                if sdata.shape[1] == 2:
+                    write_file_zip(zf, save_pulse_spectrum, output_basename,
+                                   sdata, unit, i, **kwargs)
+                else:
+                    write_file_zip(zf, save_wave_spectrum, output_basename,
+                                   sdata, unit, i, **kwargs)
+            # peaks:
+            write_file_zip(zf, save_pulse_peaks, output_basename,
+                           pdata, unit, i, **kwargs)
+            # times:
+            write_file_zip(zf, save_pulse_times, output_basename,
+                           props, i, **kwargs)
+        # wave fish properties:
+        write_file_zip(zf, save_wave_fish, output_basename,
+                       eod_props, unit, **kwargs)
+        # pulse fish properties:
+        write_file_zip(zf, save_pulse_fish, output_basename,
+                       eod_props, unit, **kwargs)
+
+
+def load_analysis(file_pathes):
+    """Load all EOD analysis files.
+
+    Parameters
+    ----------
+    file_pathes: list of string
+        Pathes of the analysis files of a single recording to be loaded.
+
+    Returns
+    -------
+    mean_eods: list of 2D array of floats
+        Averaged EOD waveforms: time in seconds, mean, standard deviation, fit.
+    wave_eodfs: 2D array of floats
+        EODfs and power of wave type fish.
+    wave_indices: array of ints
+        Corresponding indices of fish, can contain negative numbers to
+        indicate frequencies without fish.
+    eod_props: list of dict
+        Properties of EODs. The 'index' property is an index into the
+        reurned lists.
+    spec_data: list of 2D array of floats
+        Amplitude and phase spectrum of wave-type EODs with columns
+        harmonics, frequency, amplitude, relative amplitude in dB,
+        relative power in dB, phase, data power in unit squared.
+        Power spectrum of single pulse-type EODs with columns frequency, power
+    peak_data: list of 2D array of floats
+        Properties of peaks and troughs of pulse-type EODs with columns
+        P, time, amplitude, relampl, width
+    recording: string
+        Path and base name of the recording file.
+    channel: int
+        Analysed channel of the recording.
+    unit: string
+        Unit of EOD waveform.
+    """
+    recording = None
+    channel = -1
+    eod_props = []
+    zf = None
+    if len(file_pathes) == 1 and os.path.splitext(file_pathes[0])[1][1:] == 'zip':
+        zf = zipfile.ZipFile(file_pathes[0])
+        file_pathes = sorted(zf.namelist())
+    # first, read wave- and pulse-fish summaries:
+    pulse_fish = False
+    wave_fish = False
+    for f in file_pathes:
+        recording, _, channel, _, ftype, _, _ = parse_filename(f)
+        if zf is not None:
+            f = io.TextIOWrapper(zf.open(f, 'r'))
+        if ftype == 'wavefish':
+            eod_props.extend(load_wave_fish(f))
+            wave_fish = True
+        elif ftype == 'pulsefish':
+            eod_props.extend(load_pulse_fish(f))
+            pulse_fish = True
+    idx_offs = 0
+    if wave_fish and not pulse_fish:
+        idx_offs = sorted([ep['index'] for ep in eod_props])[0]
+    # then load all other files:
+    neods = len(eod_props)
+    if neods < 1:
+        neods = 1
+        eod_props = [None]
+    wave_eodfs = np.array([])
+    wave_indices = np.array([])
+    mean_eods = [None]*neods
+    spec_data = [None]*neods
+    peak_data = [None]*neods
+    unit = None
+    for f in file_pathes:
+        recording, _, channel, _, ftype, idx, _ = parse_filename(f)
+        if neods == 1 and idx > 0:
+            idx = 0
+        idx -= idx_offs
+        if zf is not None:
+            f = io.TextIOWrapper(zf.open(f, 'r'))
+        if ftype == 'waveeodfs':
+            wave_eodfs, wave_indices = load_wave_eodfs(f)
+        elif ftype == 'eodwaveform':
+            mean_eods[idx], unit = load_eod_waveform(f)
+        elif ftype == 'wavespectrum':
+            spec_data[idx], unit = load_wave_spectrum(f)
+        elif ftype == 'pulsepeaks':
+            peak_data[idx], unit = load_pulse_peaks(f)
+        elif ftype == 'pulsetimes':
+            pulse_times = load_pulse_times(f)
+            eod_props[idx]['times'] = pulse_times
+            eod_props[idx]['peaktimes'] = pulse_times
+        elif ftype == 'pulsespectrum':
+            spec_data[idx] = load_pulse_spectrum(f)
+    # fix wave spectra:
+    wave_eodfs = [fish.reshape(1, 2) if len(fish)>0 else fish
+                  for fish in wave_eodfs]
+    if len(wave_eodfs) > 0 and len(spec_data) > 0:
+        eodfs = []
+        for idx, fish in zip(wave_indices, wave_eodfs):
+            if idx >= 0:
+                spec = spec_data[idx]
+                specd = np.zeros((np.sum(np.isfinite(spec[:,-1])),
+                                  2))
+                specd[:,0] = spec[np.isfinite(spec[:,-1]),1]
+                specd[:,1] = spec[np.isfinite(spec[:,-1]),-1]
+                eodfs.append(specd)
+            else:
+                specd = np.zeros((10, 2))
+                specd[:,0] = np.arange(len(specd))*fish[0,0]
+                specd[:,1] = np.nan
+                eodfs.append(specd)
+        wave_eodfs = eodfs
+    return mean_eods, wave_eodfs, wave_indices, eod_props, spec_data, \
+        peak_data, recording, channel, unit
+
+
+def load_recording(file_path, channel=0, load_kwargs={},
+                   eod_props=None, verbose=0):
+    """Load recording.
+
+    Parameters
+    ----------
+    file_path: string
+        Full path of the file with the recorded data.
+        Extension is optional. If absent, look for the first file
+        with a reasonable extension.
+    channel: int
+        Channel of the recording to be returned.
+    load_kwargs: dict
+        Keyword arguments that are passed on to the 
+        format specific loading functions.
+    eod_props: list of dict or None
+        List of EOD properties from which start and end times of
+        analysis window are extracted.
+    verbose: int
+        Verbosity level passed on to load function.
+
+    Returns
+    -------
+    data: array of float
+        Data of the requested `channel`.
+    samplerate: float
+        Sampling rate in Hertz.
+    idx0: int
+        Start index of the analysis window.
+    idx1: int
+        End index of the analysis window.
+    data_file: str
+        Full path and name of the loaded file inclusively extension.
+
+    """
+    data = None
+    samplerate = 0.0
+    idx0 = 0
+    idx1 = 0
+    data_file = ''
+    if len(os.path.splitext(file_path)[1]) > 1:
+        data_file = file_path
+    else:
+        data_files = glob.glob(file_path + os.extsep + '*')
+        for dfile in data_files:
+            if not os.path.splitext(dfile)[1][1:] in ['zip'] + list(TableData.ext_formats.values()):
+                data_file = dfile
+                break
+    if os.path.exists(data_file):
+        data, samplerate, unit, amax = load_data(data_file,
+                                                 verbose=verbose,
+                                                 **load_kwargs)
+        idx0 = 0
+        idx1 = len(data)
+        if eod_props is not None and len(eod_props) > 0 and 'twin' in eod_props[0]:
+            idx0 = int(eod_props[0]['twin']*samplerate)
+        if len(eod_props) > 0 and 'window' in eod_props[0]:
+            idx1 = idx0 + int(eod_props[0]['window']*samplerate)
+    return data[:,channel], samplerate, idx0, idx1, data_file
+
         
 def add_eod_analysis_config(cfg, thresh_fac=0.8, percentile=0.1,
                             win_fac=2.0, min_win=0.01, max_eods=None,
                             min_sem=False, unfilter_cutoff=0.0,
                             flip_wave='none', flip_pulse='none',
                             n_harm=10, min_pulse_win=0.001,
                             peak_thresh_fac=0.01, min_dist=50.0e-6,
                             width_frac = 0.5, fit_frac = 0.5,
                             ipi_cv_thresh=0.5, ipi_percentile=30.0):
-    """ Add all parameters needed for the eod analysis functions as
-    a new section to a configuration.
+    """Add all parameters needed for the eod analysis functions as a new
+    section to a configuration.
 
     Parameters
     ----------
     cfg: ConfigFile
         The configuration.
         
-    See `eod_waveform()`, `analyze_wave()`, and `analyze_pulse()` for details on
-    the remaining arguments.
+    See `eod_waveform()`, `analyze_wave()`, and `analyze_pulse()` for
+    details on the remaining arguments.
     """
     cfg.add_section('EOD analysis:')
     cfg.add('eodSnippetFac', win_fac, '', 'The duration of EOD snippets is the EOD period times this factor.')
     cfg.add('eodMinSnippet', min_win, 's', 'Minimum duration of cut out EOD snippets.')
     cfg.add('eodMaxEODs', max_eods or 0, '', 'The maximum number of EODs used to compute the average EOD. If 0 use all EODs.')
     cfg.add('eodMinSem', min_sem, '', 'Use minimum of s.e.m. to set maximum number of EODs used to compute the average EOD.')
     cfg.add('unfilterCutoff', unfilter_cutoff, 'Hz', 'If non-zero remove effect of high-pass filter with this cut-off frequency.')
@@ -2441,18 +3019,19 @@
     cfg.add('eodPulseWidthFraction', width_frac, '', 'The width of a pulse is measured at this fraction of the pulse height.')
     cfg.add('eodExponentialFitFraction', fit_frac, '', 'An exponential function is fitted on the tail of a pulse starting at this fraction of the height of the last peak.')
     cfg.add('ipiCVThresh', ipi_cv_thresh, '', 'If coefficient of variation of interpulse intervals is smaller than this threshold, then use all intervals for computing EOD frequency.')
     cfg.add('ipiPercentile', ipi_percentile, '%', 'Use only interpulse intervals shorter than this percentile to compute EOD frequency.')
 
 
 def eod_waveform_args(cfg):
-    """ Translates a configuration to the
-    respective parameter names of the function `eod_waveform()`.
+    """Translates a configuration to the respective parameter names of
+    the function `eod_waveform()`.
     
-    The return value can then be passed as key-word arguments to this function.
+    The return value can then be passed as key-word arguments to this
+    function.
 
     Parameters
     ----------
     cfg: ConfigFile
         The configuration.
 
     Returns
@@ -2466,18 +3045,19 @@
                  'max_eods': 'eodMaxEODs',
                  'min_sem': 'eodMinSem', 
                  'unfilter_cutoff': 'unfilterCutoff'})
     return a
 
 
 def analyze_wave_args(cfg):
-    """ Translates a configuration to the
-    respective parameter names of the function `analyze_wave()`.
+    """Translates a configuration to the respective parameter names of
+    the function `analyze_wave()`.
     
-    The return value can then be passed as key-word arguments to this function.
+    The return value can then be passed as key-word arguments to this
+    function.
 
     Parameters
     ----------
     cfg: ConfigFile
         The configuration.
 
     Returns
@@ -2489,18 +3069,19 @@
     a = cfg.map({'n_harm': 'eodHarmonics',
                  'power_n_harmonics': 'powerNHarmonics',
                  'flip_wave': 'flipWaveEOD'})
     return a
 
 
 def analyze_pulse_args(cfg):
-    """ Translates a configuration to the
-    respective parameter names of the function `analyze_pulse()`.
+    """Translates a configuration to the respective parameter names of
+    the function `analyze_pulse()`.
     
-    The return value can then be passed as key-word arguments to this function.
+    The return value can then be passed as key-word arguments to this
+    function.
 
     Parameters
     ----------
     cfg: ConfigFile
         The configuration.
 
     Returns
@@ -2516,30 +3097,34 @@
                  'fit_frac': 'eodExponentialFitFraction',
                  'flip_pulse': 'flipPulseEOD',
                  'ipi_cv_thresh': 'ipiCVThresh',
                  'ipi_percentile': 'ipiPercentile'})
     return a
 
 
-def add_species_config(cfg, species_file='none', wave_max_rms=0.2, pulse_max_rms=0.2):
+def add_species_config(cfg, species_file='none', wave_max_rms=0.2,
+                       pulse_max_rms=0.2):
     """Add parameters needed for assigning EOD waveforms to species.
 
     Parameters
     ----------
     cfg: ConfigFile
         The configuration.
     species_file: string
-        File path to a file containing species names and corresponding file names
-        of EOD waveform templates. If 'none', no species assignemnt is performed.
+        File path to a file containing species names and corresponding
+        file names of EOD waveform templates. If 'none', no species
+        assignemnt is performed.
     wave_max_rms: float
-        Maximum allowed rms difference (relative to standard deviation of EOD waveform)
-        to an EOD waveform template for assignment to a wave fish species.
+        Maximum allowed rms difference (relative to standard deviation
+        of EOD waveform) to an EOD waveform template for assignment to
+        a wave fish species.
     pulse_max_rms: float
-        Maximum allowed rms difference (relative to standard deviation of EOD waveform)
-        to an EOD waveform template for assignment to a pulse fish species.
+        Maximum allowed rms difference (relative to standard deviation
+        of EOD waveform) to an EOD waveform template for assignment to
+        a pulse fish species.
     """
     cfg.add_section('Species assignment:')
     cfg.add('speciesFile', species_file, '', 'File path to a file containing species names and corresponding file names of EOD waveform templates.')
     cfg.add('maximumWaveSpeciesRMS', wave_max_rms, '', 'Maximum allowed rms difference (relative to standard deviation of EOD waveform) to an EOD waveform template for assignment to a wave fish species.')
     cfg.add('maximumPulseSpeciesRMS', pulse_max_rms, '', 'Maximum allowed rms difference (relative to standard deviation of EOD waveform) to an EOD waveform template for assignment to a pulse fish species.')
 
 
@@ -2566,18 +3151,19 @@
     cfg.add('maximumCrossings', max_crossings, '', 'Maximum number of zero crossings per EOD period.')
     cfg.add('maximumFirstHarmonicAmplitude', max_relampl_harm1, '', 'Skip waveform of wave fish if the amplitude of the first harmonic is higher than this factor times the amplitude of the fundamental. If set to zero do not check.')
     cfg.add('maximumSecondHarmonicAmplitude', max_relampl_harm2, '', 'Skip waveform of wave fish if the ampltude of the second harmonic is higher than this factor times the amplitude of the fundamental. That is, the waveform appears to have twice the frequency than the fundamental. If set to zero do not check.')
     cfg.add('maximumThirdHarmonicAmplitude', max_relampl_harm3, '', 'Skip waveform of wave fish if the ampltude of the third harmonic is higher than this factor times the amplitude of the fundamental. If set to zero do not check.')
 
 
 def wave_quality_args(cfg):
-    """ Translates a configuration to the
-    respective parameter names of the function `wave_quality()`.
+    """Translates a configuration to the respective parameter names of
+    the function `wave_quality()`.
     
-    The return value can then be passed as key-word arguments to this function.
+    The return value can then be passed as key-word arguments to this
+    function.
 
     Parameters
     ----------
     cfg: ConfigFile
         The configuration.
 
     Returns
@@ -2599,18 +3185,19 @@
                  'max_relampl_harm1': 'maximumFirstHarmonicAmplitude',
                  'max_relampl_harm2': 'maximumSecondHarmonicAmplitude',
                  'max_relampl_harm3': 'maximumThirdHarmonicAmplitude'})
     return a
 
 
 def pulse_quality_args(cfg):
-    """ Translates a configuration to the
-    respective parameter names of the function `pulse_quality()`.
+    """Translates a configuration to the respective parameter names of
+    the function `pulse_quality()`.
     
-    The return value can then be passed as key-word arguments to this function.
+    The return value can then be passed as key-word arguments to this
+    function.
 
     Parameters
     ----------
     cfg: ConfigFile
         The configuration.
 
     Returns
@@ -2620,38 +3207,34 @@
         and their values as supplied by `cfg`.
     """
     a = cfg.map({'max_clipped_frac': 'maximumClippedFraction',
                  'max_rms_sem': 'maximumRMSNoise'})
     return a
 
 
-if __name__ == '__main__':
-    import sys
+def main():
     import matplotlib.pyplot as plt
-    from .fakefish import pulsefish_eod
-    from .eventdetection import detect_peaks
+    from .fakefish import pulsefish_eods
 
     print('Analysis of EOD waveforms.')
 
     # data:
     samplerate = 44100.0
-    data = pulsefish_eod('biphasic', 83.0, samplerate, 5.0, noise_std=0.05)
+    data = pulsefish_eods('Triphasic', 83.0, samplerate, 5.0, noise_std=0.02)
     unit = 'mV'
     eod_idx, _ = detect_peaks(data, 1.0)
     eod_times = eod_idx/samplerate
 
     # analyse EOD:
     mean_eod, eod_times = eod_waveform(data, samplerate, eod_times)
     mean_eod, props, peaks, power = analyze_pulse(mean_eod, eod_times)
 
     # plot:
-    fig = plt.figure()
-    ax = fig.add_subplot(1, 2, 1)
-    plot_eod_waveform(ax, mean_eod, peaks, unit=unit)
-    props['unit'] = unit
-    label = '{type} fish\nEODf = {EODf:.1f} Hz\np-p amplitude = {p-p-amplitude:.3g} {unit}\nn = {n} EODs\n'.format(**props)
-    if props['flipped']:
-        label += 'flipped\n'
-    ax.text(0.03, 0.97, label, transform = ax.transAxes, va='top')
-    ax = fig.add_subplot(1, 2, 2)
-    plot_pulse_spectrum(ax, power, props)
+    fig, axs = plt.subplots(1, 2)
+    plot_eod_waveform(axs[0], mean_eod, props, peaks, unit=unit)
+    axs[0].set_title('{type} fish: EODf = {EODf:.1f} Hz'.format(**props))
+    plot_pulse_spectrum(axs[1], power, props)
     plt.show()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `thunderfish-1.9.9/thunderfish/eodexplorer.py` & `thunderfish-2.0.0/src/thunderfish/eodexplorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-"""
-View and explore properties of EOD waveforms.
+"""View and explore properties of EOD waveforms.
 """
 
 import os
 import glob
 import sys
 import argparse
 import numpy as np
 import scipy.signal as sig
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
 from multiprocessing import Pool, freeze_support, cpu_count
+from thunderlab.configfile import ConfigFile
+from thunderlab.tabledata import TableData, add_write_table_config, write_table_args
+from thunderlab.dataloader import load_data
+from thunderlab.multivariateexplorer import MultivariateExplorer
+from thunderlab.powerspectrum import decibel
 from .version import __version__, __year__
-from .configfile import ConfigFile
-from .tabledata import TableData, add_write_table_config, write_table_args
-from .dataloader import load_data
-from .multivariateexplorer import MultivariateExplorer
 from .harmonics import add_harmonic_groups_config
 from .eodanalysis import add_species_config
 from .eodanalysis import wave_quality, wave_quality_args, add_eod_quality_config
 from .eodanalysis import pulse_quality, pulse_quality_args
-from .powerspectrum import decibel
 from .bestwindow import analysis_window
 from .thunderfish import configuration, detect_eods, plot_eods
 
 
 basename = ''
 
 
@@ -39,16 +38,16 @@
     - `select_EOD_properties()`: select data columns to be explored.
     - `select_color_property()`: select column from data table for colorizing the data.
     """
     
     def __init__(self, data, data_cols, wave_fish, eod_data,
                  add_waveforms, loaded_spec, rawdata_path):
         """
-        Parameter
-        ---------
+        Parameters
+        ----------
         data: TableData
             Full table of EOD properties. Each row is a fish.
         data_cols: list of string or ints
             Names or indices of columns in `data` to be explored.
             You may use the static function `select_EOD_properties()`
             for assisting the selection of columns.
         wave_fish: boolean
@@ -158,15 +157,15 @@
         - Limits for amplitude and time like quantities start at zero.
         - Phases a labeled with multuples of pi.
         - Species labels are rotated.
         """
         if any(l in label for l in ['ampl', 'power', 'width',
                                     'time', 'tau', 'P2-P1-dist',
                                     'var', 'peak', 'trough',
-                                    'dist', 'rms', 'noise']):
+                                    'P2-P1-dist', 'rms', 'noise']):
             if np.all(data[np.isfinite(data)] >= 0.0):
                 if axis == 'x':
                     ax.set_xlim(0.0, None)
                 elif axis == 'y':
                     ax.set_ylim(0.0, None)
                 elif axis == 'c':
                     return 0.0, np.max(data), None
@@ -202,15 +201,15 @@
             elif axis == 'c':
                 if ax is not None:
                     ax.set_ylabel('')
         return np.min(data), np.max(data), None
 
     
     def fix_waveform_plot(self, axs, indices):
-        """ Adapt waveform plots to EOD waveforms, derivatives, and spectra.
+        """Adapt waveform plots to EOD waveforms, derivatives, and spectra.
         """
         if len(indices) == 0:
             axs[0].text(0.5, 0.5, 'Click to plot EOD waveforms',
                         transform = axs[0].transAxes, ha='center', va='center')
             axs[0].text(0.5, 0.3, 'n = %d' % len(self.raw_data),
                         transform = axs[0].transAxes, ha='center', va='center')
         elif len(indices) == 1:
@@ -270,15 +269,15 @@
                     ax.yaxis.set_major_locator(ticker.MultipleLocator(20.0))
         if len(indices) > 0:
             for ax in axs:
                 ax.axhline(c='k', lw=1)
 
             
     def list_selection(self, indices):
-        """ List file names and indices of selection.
+        """List file names and indices of selection.
 
         If only a single EOD is selected, list all of its properties.
         """
         if 'index' in self.eoddata and \
            np.any(self.eoddata[:,'index'] != self.eoddata[0,'index']):
             for i in indices:
                 file_name = self.eoddata[i,'file'] if 'file' in self.eoddata else basename
@@ -302,27 +301,28 @@
                     keylen = len(k)
             for k, v in zip(keys, values):
                 fs = '%%-%ds: %%s' % keylen
                 print(fs % (k, v.strip()))
 
                 
     def analyze_selection(self, index):
-        """ Launch thunderfish on the selected EOD.
+        """Launch thunderfish on the selected EOD.
         """
         # load data:
         file_base = self.eoddata[index,'file'] if 'file' in self.eoddata else basename
         bp = os.path.join(self.path, file_base)
         fn = glob.glob(bp + '.*')
         if len(fn) == 0:
             print('no recording found for %s' % bp)
             return
         recording = fn[0]
         channel = 0
         try:
-            raw_data, samplerate, unit = load_data(recording, channel)
+            raw_data, samplerate, unit, ampl_max = load_data(recording)
+            raw_data = raw_data[:,channel]
         except IOError as e:
             print('%s: failed to open file: did you provide a path to the raw data (-P option)?' % (recording))
             return
         if len(raw_data) <= 1:
             print('%s: empty data file' % recording)
             return
         # load configuration:
@@ -330,50 +330,52 @@
         cfg = configuration(cfgfile, False, recording)
         cfg.load_files(cfgfile, recording, 4)
         if 'flipped' in self.eoddata:
             fs = 'flip' if self.eoddata[index,'flipped'] else 'none'
             cfg.set('flipWaveEOD', fs)
             cfg.set('flipPulseEOD', fs)
         # best_window:
-        data, idx0, idx1, clipped, min_clip, max_clip = analysis_window(raw_data, samplerate, cfg.value('windowPosition'), cfg)
+        data, idx0, idx1, clipped, min_clip, max_clip = \
+            analysis_window(raw_data, samplerate, ampl_max,
+                            cfg.value('windowPosition'), cfg)
         # detect EODs in the data:
         psd_data, fishlist, _, eod_props, mean_eods, \
           spec_data, peak_data, power_thresh, skip_reason, zoom_window = \
           detect_eods(data, samplerate, min_clip, max_clip, recording, 0, 0, cfg)
         # plot EOD:
         idx = int(self.eoddata[index,'index']) if 'index' in self.eoddata else 0
         for k in ['toolbar', 'keymap.back', 'keymap.forward',
                   'keymap.zoom', 'keymap.pan']:
             plt.rcParams[k] = self.plt_params[k]
-        fig = plot_eods(file_base, raw_data, samplerate, None, idx0, idx1,
+        fig = plot_eods(file_base, None, raw_data, samplerate, None, idx0, idx1,
                         clipped, psd_data[0], fishlist, None,
                         mean_eods, eod_props, peak_data, spec_data,
                         [idx], unit, zoom_window, 10, None, True, False,
                         'auto', False, 0.0, 3000.0,
                         interactive=True, verbose=0)
-        fig.canvas.set_window_title('thunderfish: %s' % file_base)
+        fig.canvas.manager.set_window_title('thunderfish: %s' % file_base)
         plt.show(block=False)
 
 
-    """ Names of groups of data columns that can be selected by the select_EOD_properties() function.
+    """Names of groups of data columns that can be selected by the select_EOD_properties() function.
     """
     groups = ['all', 'allpower', 'noise', 'timing',
               'ampl', 'relampl', 'power', 'relpower', 'phase',
               'time', 'width', 'peaks', 'none']
     
     @staticmethod
     def select_EOD_properties(data, wave_fish, max_n, column_groups, add_columns):
-        """ Select data columns to be explored.
+        """Select data columns to be explored.
 
         First, groups of columns are selected, then individual
         columns. Columns that are selected twice are removed from the
         selection.
 
-        Parameter
-        ---------
+        Parameters
+        ----------
         data: TableData
             Table with EOD properties from which columns are selected.
         wave_fish: boolean.
             Indicates if data contains properties of wave- or pulse-type electric fish.
         max_n: int
             Maximum number of harmonics (wae-type fish) or peaks (pulse-type fish)
             to be  selected.
@@ -508,20 +510,20 @@
             else:
                 data_cols.append(idx)
         return data_cols, None
 
     
     @staticmethod
     def select_color_property(data, data_cols, color_col):
-        """ Select column from data table for colorizing the data.
+        """Select column from data table for colorizing the data.
 
         Pass the output of this function on to MultivariateExplorer.set_colors().
 
-        Parameter
-        ---------
+        Parameters
+        ----------
         data: TableData
             Table with all EOD properties from which columns are selected.
         data_cols: list of int
             List of columns selected to be explored.
         color_col: string or int
             Column to be selected for coloring the data.
             If 'row' then use the row index of the data in the table for coloring.
```

### Comparing `thunderfish-1.9.9/thunderfish/fakefish.py` & `thunderfish-2.0.0/src/thunderfish/fakefish.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Simulate EOD waveforms.
+"""Simulate EOD waveforms.
 
 
 ## Species names
 
 - `species_name`: translate species ids to full species names.
 - `abbrv_genus()`: abbreviate genus in a species name.
 
@@ -26,31 +25,30 @@
 
 
 ## Interactive waveform generation
 
 - `generate_waveform()`: interactively generate audio file with simulated EOD waveforms.
 """
 
-from __future__ import print_function
 import sys
 import numpy as np
 
 
 species_name = dict(Sine='Sinewave',
                     Alepto='Apteronotus leptorhynchus',
                     Arostratus='Apteronotus rostratus',
                     Eigenmannia='Eigenmannia spec.',
                     Sternarchella='Sternarchella terminalis',
                     Sternopygus='Sternopygus dariensis')
-""" Translate species ids used by wavefish_harmonics and pulsefish_eodpeaks to full species names.
+"""Translate species ids used by wavefish_harmonics and pulsefish_eodpeaks to full species names.
 """
 
 
 def abbrv_genus(name):
-    """ Abbreviate genus in a species name.
+    """Abbreviate genus in a species name.
 
     Parameters
     ----------
     name: string
         Full species name of the form 'Genus species subspecies'
 
     Returns
@@ -94,19 +92,19 @@
 
 wavefish_harmonics = dict(Sine=Sine_harmonics,
                           Alepto=Apteronotus_leptorhynchus_harmonics,
                           Arostratus=Apteronotus_rostratus_harmonics,
                           Eigenmannia=Eigenmannia_harmonics,
                           Sternarchella=Sternarchella_terminalis_harmonics,
                           Sternopygus=Sternopygus_dariensis_harmonics)
-""" Amplitudes and phases of EOD waveforms of various species of wave-type electric fish. """
+"""Amplitudes and phases of EOD waveforms of various species of wave-type electric fish."""
 
 
 def wavefish_spectrum(fish):
-    """ Amplitudes and phases of a wavefish EOD.
+    """Amplitudes and phases of a wavefish EOD.
 
     Parameters
     ----------
     fish: string, dict or tuple of lists/arrays
         Specify relative amplitudes and phases of the fundamental and its harmonics.
         If string then take amplitudes and phases from the `wavefish_harmonics` dictionary.
         If dictionary then take amplitudes and phases from the 'amlitudes' and 'phases' keys.
@@ -137,20 +135,26 @@
         if not fish in wavefish_harmonics:
             raise KeyError('unknown wavefish. Choose one of ' +
                            ', '.join(wavefish_harmonics.keys()))
         amplitudes = wavefish_harmonics[fish]['amplitudes']
         phases = wavefish_harmonics[fish]['phases']
     if len(amplitudes) != len(phases):
         raise IndexError('need exactly as many phases as amplitudes')
+    # remove NaNs:
+    for k in reversed(range(len(amplitudes))):
+        if np.isfinite(amplitudes[k]) or np.isfinite(phases[k]):
+            amplitudes = amplitudes[:k+1]
+            phases = phases[:k+1]
+            break
     return amplitudes, phases
 
 
 def wavefish_eods(fish='Eigenmannia', frequency=100.0, samplerate=44100.0,
                   duration=1.0, phase0=0.0, noise_std=0.05):
-    """ Simulate EOD waveform of a wave-type fish.
+    """Simulate EOD waveform of a wave-type fish.
                   
     The waveform is constructed by superimposing sinewaves of integral
     multiples of the fundamental frequency - the fundamental and its
     harmonics.  The fundamental frequency of the EOD (EODf) is given by
     `frequency`. With `fish` relative amplitudes and phases of the
     fundamental and its harmonics are specified.
 
@@ -197,64 +201,80 @@
         phase = np.arange(0, duration, 1.0/samplerate)
         phase *= frequency
     else:
         phase = np.cumsum(frequency)/samplerate
     # generate EOD:
     data = np.zeros(len(phase))
     for har, (ampl, phi) in enumerate(zip(amplitudes, phases)):
-        data += ampl * np.sin(2*np.pi*(har+1)*phase + phi - (har+1)*phase0)
+        if np.isfinite(ampl) and np.isfinite(phi):
+            data += ampl * np.sin(2*np.pi*(har+1)*phase + phi - (har+1)*phase0)
     # add noise:
     data += noise_std * np.random.randn(len(data))
     return data
 
 
-def normalize_wavefish(fish):
-    """ Normalize amplitudes and phases of wave-type EOD waveform.
+def normalize_wavefish(fish, mode='peak'):
+    """Normalize amplitudes and phases of wave-type EOD waveform.
 
-    The amplitudes and phases of the Fourier components are adjusted such
-    that the resulting EOD waveform has a peak-to-peak amplitude of two
-    and the peak of the waveform is at time zero.
+    The amplitudes and phases of the Fourier components are adjusted
+    such that the resulting EOD waveform has a peak-to-peak amplitude
+    of two and the peak of the waveform is at time zero (mode is set
+    to 'peak') or that the fundamental has an amplitude of one and a
+    phase of 0 (mode is set to 'zero').
 
     Parameters
     ----------
     fish: string, dict or tuple of lists/arrays
         Specify relative amplitudes and phases of the fundamental and its harmonics.
         If string then take amplitudes and phases from the `wavefish_harmonics` dictionary.
         If dictionary then take amplitudes and phases from the 'amlitudes' and 'phases' keys.
         If tuple then the first element is the list of amplitudes and
         the second one the list of relative phases in radians.
+    mode: 'peak' or 'zero'
+        How to normalize amplitude and phases:
+        - 'peak': normalize waveform to a peak-to-peak amplitude of two
+          and shift it such that its peak is at time zero.
+        - 'zero': scale amplitude of fundamental to one and its phase to zero.
 
     Returns
     -------
     amplitudes: array of floats
         Adjusted amplitudes of the fundamental and its harmonics.
     phases: array of floats
         Adjusted phases in radians of the fundamental and its harmonics.
+
     """
     # get relative amplitude and phases:
     amplitudes, phases = wavefish_spectrum(fish)
-    # generate waveform:
-    eodf = 100.0
-    rate = 100000.0
-    data = wavefish_eods(fish, eodf, rate, 2.0/eodf, noise_std=0.0)
-    # normalize amplitudes:
-    ampl = 0.5*(np.max(data) - np.min(data))
-    newamplitudes = np.array(amplitudes)/ampl
-    # shift phases:
-    deltat = np.argmax(data[:int(rate/eodf)])/rate
-    deltap = 2.0*np.pi*deltat*eodf
-    newphases = np.array([p+(k+1)*deltap for k, p in enumerate(phases)])
-    newphases %= 2.0*np.pi
-    newphases[newphases>np.pi] -= 2.0*np.pi
-    # return:
-    return newamplitudes, newphases
+    if mode == 'zero':
+        newamplitudes = np.array(amplitudes)/amplitudes[0]
+        newphases = np.array([p+(k+1)*(-phases[0]) for k, p in enumerate(phases)])
+        newphases %= 2.0*np.pi
+        newphases[newphases>np.pi] -= 2.0*np.pi
+        return newamplitudes, newphases
+    else:
+        # generate waveform:
+        eodf = 100.0
+        rate = 100000.0
+        data = wavefish_eods(fish, eodf, rate, 2.0/eodf, noise_std=0.0)
+        # normalize amplitudes:
+        ampl = 0.5*(np.max(data) - np.min(data))
+        newamplitudes = np.array(amplitudes)/ampl
+        # shift phases:
+        deltat = np.argmax(data[:int(rate/eodf)])/rate
+        deltap = 2.0*np.pi*deltat*eodf
+        newphases = np.array([p+(k+1)*deltap for k, p in enumerate(phases)])
+        newphases %= 2.0*np.pi
+        newphases[newphases>np.pi] -= 2.0*np.pi
+        # return:
+        return newamplitudes, newphases
 
 
 def export_wavefish(fish, name='Unknown_harmonics', file=None):
-    """ Serialize wavefish parameter to python code.
+    """Serialize wavefish parameter to python code.
 
     Add output to the wavefish_harmonics dictionary!
 
     Parameters
     ----------
     fish: string, dict or tuple of lists/arrays
         Specify relative amplitudes and phases of the fundamental and its harmonics.
@@ -282,38 +302,38 @@
         closeit = False
     except AttributeError:
         file = open(file, 'w')
         closeit = True
     n = 6
     file.write(name + ' = \\\n')
     file.write('    dict(amplitudes=(')
-    file.write(', '.join(['%.5g' % a for a in amplitudes[:n]]))
+    file.write(', '.join([f'{a:.5g}' for a in amplitudes[:n]]))
     for k in range(n, len(amplitudes), n):
         file.write(',\n')
         file.write(' ' * (9+12))
-        file.write(', '.join(['%.5g' % a for a in amplitudes[k:k+n]]))
+        file.write(', '.join([f'{a:.5g}' for a in amplitudes[k:k+n]]))
     file.write('),\n')
     file.write(' ' * 9 + 'phases=(')
-    file.write(', '.join(['%.5g' % p for p in phases[:n]]))
+    file.write(', '.join(['{p:.5g}' for p in phases[:n]]))
     for k in range(n, len(phases), n):
         file.write(',\n')
         file.write(' ' * (9+8))
-        file.write(', '.join(['%.5g' % p for p in phases[k:k+n]]))
+        file.write(', '.join([f'{p:.5g}' for p in phases[k:k+n]]))
     file.write('))\n')
     if closeit:
         file.close()
     # return dictionary:
     harmonics = dict(amplitudes=amplitudes,
                      phases=phases)
     return harmonics
 
 
 def chirps(eodf=100.0, samplerate=44100.0, duration=1.0, chirp_freq=5.0,
            chirp_size=100.0, chirp_width=0.01, chirp_kurtosis=1.0, chirp_contrast=0.05):
-    """ Simulate frequency trace with chirps.
+    """Simulate frequency trace with chirps.
 
     A chirp is modeled as a Gaussian frequency modulation.
     The first chirp is placed at 0.5/chirp_freq.
 
     Parameters
     ----------
     eodf: float
@@ -368,15 +388,15 @@
         frequency[i0:i1] += chirp_size * gauss[gi0:gi1]
         am[i0:i1] -= chirp_contrast * gauss[gi0:gi1]
     return frequency, am
 
 
 def rises(eodf=100.0, samplerate=44100.0, duration=1.0, rise_freq=0.1,
           rise_size=10.0, rise_tau=1.0, decay_tau=10.0):
-    """ Simulate frequency trace with rises.
+    """Simulate frequency trace with rises.
 
     A rise is modeled as a double exponential frequency modulation.
 
     Parameters
     ----------
     eodf: float
         EOD frequency of the fish in Hertz.
@@ -435,20 +455,21 @@
     dict(times=(3e-05, 0.00018, 0.00043),
          amplitudes=(1.2382, -0.9906, 0.12382),
          stdevs=(0.0001, 0.0001, 0.0002))
 
 pulsefish_eodpeaks = dict(Monophasic=Monophasic_peaks,
                           Biphasic=Biphasic_peaks,
                           Triphasic=Triphasic_peaks)
-""" Standard deviations, amplitudes and positions of Gaussians that make up
-    EOD waveforms of pulse-type electric fish. """
+"""Standard deviations, amplitudes and positions of Gaussians that
+    make up EOD waveforms of pulse-type electric fish.
+"""
 
 
 def pulsefish_peaks(fish):
-    """ Position, amplitudes and standard deviations of peaks in pulsefish EOD waveforms.
+    """Position, amplitudes and standard deviations of peaks in pulsefish EOD waveforms.
 
     Parameters
     ----------
     fish: string, dict or tuple of floats/lists/arrays
         Specify positions, amplitudes and standard deviations Gaussians peaks that are
         superimposed to simulate EOD waveforms of pulse-type electric fishes. 
         If string then take positions, amplitudes and standard deviations 
@@ -494,15 +515,15 @@
         raise IndexError('need exactly as many standard deviations as amplitudes and times')
     return peak_times, peak_amplitudes, peak_stdevs
                               
 
 def pulsefish_eods(fish='Biphasic', frequency=100.0, samplerate=44100.0,
                    duration=1.0, noise_std=0.01, jitter_cv=0.1,
                    first_pulse=None):
-    """ Simulate EOD waveform of a pulse-type fish.
+    """Simulate EOD waveform of a pulse-type fish.
 
     Pulses are spaced by 1/frequency, jittered as determined by jitter_cv. Each pulse is
     a combination of Gaussian peaks, whose positions, amplitudes and widths are
     given by 'fish'.
 
     The generated waveform is duration seconds long and is sampled with samplerate Hertz.
     Gaussian white noise with a standard deviation of noise_std is added to the generated
@@ -568,22 +589,22 @@
     data = np.random.randn(len(time)) * noise_std
     period = 1.0/frequency
     jitter_std = period * jitter_cv
     if first_pulse is None:
         first_pulse = np.max([pulse_duration, 3.0*jitter_std])
     pulse_times = np.arange(first_pulse, duration, period )
     pulse_times += jitter_std*np.random.randn(len(pulse_times))
-    pulse_indices = np.round(pulse_times * samplerate).astype(np.int)
+    pulse_indices = np.round(pulse_times * samplerate).astype(int)
     for inx in pulse_indices[(pulse_indices>=poffs)&(pulse_indices-poffs+len(pulse)<len(data))]:
         data[inx-poffs:inx-poffs+len(pulse)] += pulse
     return data
 
 
 def normalize_pulsefish(fish):
-    """ Normalize times and stdevs of pulse-type EOD waveform.
+    """Normalize times and stdevs of pulse-type EOD waveform.
 
     The positions and amplitudes of Gaussian peaks are adjusted such
     that the resulting EOD waveform has a maximum peak amplitude of one
     and has the largest peak at time zero.
 
     Parameters
     ----------
@@ -623,15 +644,15 @@
     peaks = dict(times=newtimes,
                  amplitudes=newamplitudes,
                  stdevs=peak_stdevs)
     return peaks
 
 
 def export_pulsefish(fish, name='Unknown_peaks', file=None):
-    """ Serialize pulsefish parameter to python code.
+    """Serialize pulsefish parameter to python code.
 
     Add output to the pulsefish_eodpeaks dictionary!
 
     Parameters
     ----------
     fish: string, dict or tuple of floats/lists/arrays
         Specify positions, amplitudes and standard deviations Gaussians peaks that are
@@ -663,63 +684,63 @@
         closeit = False
     except AttributeError:
         file = open(file, 'w')
         closeit = True
     n = 6
     file.write(name + ' = \\\n')
     file.write('    dict(times=(')
-    file.write(', '.join(['%.5g' % a for a in peak_times[:n]]))
+    file.write(', '.join([f'{a:.5g}' for a in peak_times[:n]]))
     for k in range(n, len(peak_times), n):
         file.write(',\n')
         file.write(' ' * (9+12))
-        file.write(', '.join(['%.5g' % a for a in peak_times[k:k+n]]))
+        file.write(', '.join([f'{a:.5g}' for a in peak_times[k:k+n]]))
     if len(peak_times) == 1:
         file.write(',')
     file.write('),\n')
     file.write(' ' * 9 + 'amplitudes=(')
-    file.write(', '.join(['%.5g' % p for p in peak_amplitudes[:n]]))
+    file.write(', '.join([f'{p:.5g}' for p in peak_amplitudes[:n]]))
     for k in range(n, len(peak_amplitudes), n):
         file.write(',\n')
         file.write(' ' * (9+8))
-        file.write(', '.join(['%.5g' % p for p in peak_amplitudes[k:k+n]]))
+        file.write(', '.join([f'{p:.5g}' for p in peak_amplitudes[k:k+n]]))
     if len(peak_amplitudes) == 1:
         file.write(',')
     file.write('),\n')
     file.write(' ' * 9 + 'stdevs=(')
-    file.write(', '.join(['%.5g' % p for p in peak_stdevs[:n]]))
+    file.write(', '.join([f'{p:.5g}' for p in peak_stdevs[:n]]))
     for k in range(n, len(peak_stdevs), n):
         file.write(',\n')
         file.write(' ' * (9+8))
-        file.write(', '.join(['%.5g' % p for p in peak_stdevs[k:k+n]]))
+        file.write(', '.join([f'{p:.5g}' for p in peak_stdevs[k:k+n]]))
     if len(peak_stdevs) == 1:
         file.write(',')
     file.write('))\n')
     if closeit:
         file.close()
     # return dictionary:
     peaks = dict(times=peak_times,
                  amplitudes=peak_amplitudes,
                  stdevs=peak_stdevs)
     return peaks
 
 
 def generate_waveform(filename):
-    """ Interactively generate audio file with simulated EOD waveforms.
+    """Interactively generate audio file with simulated EOD waveforms.
 
     Parameters needed to generate EOD waveforms are take from console input.
 
     Parameters
     ----------
     filename: string
         Name of file inclusively extension (e.g. '.wav')
         used to store the simulated EOD waveforms.
     """
     import os
-    from audioio.audiowriter import write_audio
-    from .consoleinput import read, select, save_inputs
+    from audioio import write_audio
+    from thunderlab.consoleinput import read, select, save_inputs
     # generate file:
     samplerate = read('Sampling rate in Hz', '44100', float, 1.0)
     duration = read('Duration in seconds', '10', float, 0.001)
     nfish = read('Number of fish', '1', int, 1)
     ndata = read('Number of electrodes', '1', int, 1)
     fish_spread = 1
     if ndata > 1:
@@ -758,42 +779,42 @@
                 eodfreq, _ = chirps(eodf, samplerate, duration,
                                     chirp_freq, chirp_size, chirp_width, chirp_kurtosis)
             elif eodsig == 'r':
                 rise_freq = read('Number of rises per second', '%g'%rise_freq, float, 0.00001)
                 rise_size = read('Size of rise in Hz', '%g'%rise_size, float, 0.01)
                 rise_tau = read('Time-constant of rise onset in seconds', '%g'%rise_tau, float, 0.01)
                 rise_decay_tau = read('Time-constant of rise decay in seconds', '%g'%rise_decay_tau, float, 0.01)
-                eodfreq = rises_frequency(eodf, samplerate, duration,
-                                          rise_freq, rise_size, rise_tau, rise_decay_tau)
+                eodfreq = rises(eodf, samplerate, duration,
+                                rise_freq, rise_size, rise_tau, rise_decay_tau)
             if eodt == 'a':
                 fishdata = eoda*wavefish_eods('Alepto', eodfreq, samplerate, duration,
                                               phase0=0.0, noise_std=0.0)
             elif eodt == 'e':
                 fishdata = eoda*wavefish_eods('Eigenmannia', eodfreq, samplerate,
                                               duration, phase0=0.0, noise_std=0.0)
         else:
             pulse_jitter = read(fish + 'CV of pulse jitter', '%g'%pulse_jitter, float, 0.0, 2.0)
             if eodt == '1':
-                fishdata = eoda*pulsefish_eods('monophasic', eodf, samplerate, duration,
+                fishdata = eoda*pulsefish_eods('Monophasic', eodf, samplerate, duration,
                                                jitter_cv=pulse_jitter, noise_std=0.0)
             elif eodt == '2':
-                fishdata = eoda*pulsefish_eods('biphasic', eodf, samplerate, duration,
+                fishdata = eoda*pulsefish_eods('Biphasic', eodf, samplerate, duration,
                                                jitter_cv=pulse_jitter, noise_std=0.0)
             elif eodt == '3':
-                fishdata = eoda*pulsefish_eods('triphasic', eodf, samplerate, duration,
+                fishdata = eoda*pulsefish_eods('Triphasic', eodf, samplerate, duration,
                                                jitter_cv=pulse_jitter, noise_std=0.0)
         i = fish_indices[k]
         for j in range(fish_spread):
             data[:, (i+j)%ndata] += fishdata*(0.2**j)
 
     maxdata = np.max(np.abs(data))
     write_audio(filename, 0.9*data/maxdata, samplerate)
     input_file = os.path.splitext(filename)[0] + '.inp' 
     save_inputs(input_file)
-    print('\nWrote fakefish data to file "%s".' % filename)
+    print(f'\nWrote fakefish data to file "{filename}".')
             
 
 def demo():
     import matplotlib.pyplot as plt
     samplerate = 40000.0 # in Hz
     duration = 10.0      # in sec
 
@@ -803,15 +824,15 @@
 
     # generate data:
     eodf = 400.0
     wavefish = wavefish_eods('Alepto', eodf, samplerate, duration, noise_std=0.02)
     eodf = 650.0
     wavefish += 0.5*wavefish_eods('Eigenmannia', eodf, samplerate, duration)
 
-    pulsefish = pulsefish_eods('biphasic', 80.0, samplerate, duration,
+    pulsefish = pulsefish_eods('Biphasic', 80.0, samplerate, duration,
                                noise_std=0.02, jitter_cv=0.1, first_pulse=inset_len/2)
     time = np.arange(len(wavefish))/samplerate
 
     fig, ax = plt.subplots(nrows=2, ncols=2, figsize=(19, 10))
 
     # get proper wavefish ylim
     ymin = np.min(wavefish)
@@ -871,36 +892,37 @@
     ax[0].set_ylim(0.0, 3000.0)
     ax[0].set_ylabel('Frequency [Hz]')
 
     nfft = 4096
     ax[1].set_title('Rises')
     ax[1].specgram(rises_data, Fs=samplerate, NFFT=nfft, noverlap=nfft//2)
     time = np.arange(len(rises_freq))/samplerate
-    ax[1].plot(time[:-nfft/4], rises_freq[nfft/4:], '-k', lw=2)
+    ax[1].plot(time[:-nfft//4], rises_freq[nfft//4:], '-k', lw=2)
     ax[1].set_ylim(500.0, 700.0)
     ax[1].set_ylabel('Frequency [Hz]')
     ax[1].set_xlabel('Time [s]')
     plt.tight_layout()
 
     plt.show()
 
 
-def main():
-    import sys
+def main(args=[]):
+    from .version import __year__
     
-    if len(sys.argv) > 1:
-        if len(sys.argv) == 2 or sys.argv[1] != '-s':
+    if len(args) > 0:
+        if len(args) == 1 or args[0] != '-s':
             print('usage: fakefish [-h|--help] [-s audiofile]')
             print('')
             print('Without arguments, run a demo for illustrating fakefish functionality.')
             print('')
             print('-s audiofile: writes audiofile with user defined simulated electric fishes.')
             print('')
-            print('by bendalab (2020)')
+            print(f'by bendalab ({__year__})')
         else:
-            generate_waveform(sys.argv[2])
+            generate_waveform(args[1])
     else:
         demo()
 
             
 if __name__ == '__main__':
-    main()
+    import sys
+    main(sys.argv[1:])
```

### Comparing `thunderfish-1.9.9/thunderfish/fishfinder.py` & `thunderfish-2.0.0/src/thunderfish/fishfinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import sys
 import os
 import warnings
 import argparse
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.mlab as ml
-from audioio.playaudio import PlayAudio, fade
-from audioio.audiowriter import write_audio
+from audioio import PlayAudio, fade, write_audio
+from thunderlab.configfile import ConfigFile
+from thunderlab.dataloader import DataLoader
+from thunderlab.powerspectrum import nfft, decibel, psd, spectrogram
+from thunderlab.powerspectrum import add_multi_psd_config, multi_psd_args
 from .version import __version__, __year__
-from .configfile import ConfigFile
-from .dataloader import open_data
-from .powerspectrum import nfft, decibel, psd, spectrogram
-from .powerspectrum import add_multi_psd_config, multi_psd_args
 from .harmonics import harmonic_groups, harmonic_groups_args, psd_peak_detection_args
 from .harmonics import add_psd_peak_detection_config, add_harmonic_groups_config, colors_markers
 from .bestwindow import clip_amplitudes, clip_args, best_window_indices
 from .bestwindow import best_window_args
 from .thunderfish import configuration, save_configuration
 # check: import logging https://docs.python.org/2/howto/logging.html#logging-basic-tutorial
 
@@ -69,20 +68,20 @@
         # set key bindings:
         plt.rcParams['keymap.fullscreen'] = 'ctrl+f'
         plt.rcParams['keymap.pan'] = 'ctrl+m'
         plt.rcParams['keymap.quit'] = 'ctrl+w, alt+q, q'
         plt.rcParams['keymap.yscale'] = ''
         plt.rcParams['keymap.xscale'] = ''
         plt.rcParams['keymap.grid'] = ''
-        plt.rcParams['keymap.all_axes'] = ''
+        #plt.rcParams['keymap.all_axes'] = ''
 
         # the figure:
         plt.ioff()
         self.fig = plt.figure(figsize=(15, 9))
-        self.fig.canvas.set_window_title(self.filename + ' channel {0:d}'.format(self.channel))
+        self.fig.canvas.manager.set_window_title(self.filename + ' channel {0:d}'.format(self.channel))
         self.fig.canvas.mpl_connect('key_press_event', self.keypress)
         self.fig.canvas.mpl_connect('button_press_event', self.buttonpress)
         self.fig.canvas.mpl_connect('pick_event', self.onpick)
         self.fig.canvas.mpl_connect('resize_event', self.resize)
         # trace plot:
         self.axt = self.fig.add_axes([0.1, 0.7, 0.87, 0.25])
         self.axt.set_ylabel('Amplitude [{:s}]'.format(self.unit))
@@ -133,15 +132,15 @@
         self.helptext.append(ht)
         # plot:
         for ht in self.helptext:
             ht.set_visible(self.help)
         self.update_plots(False)
         plt.show()
 
-    def __del(self):
+    def __del__(self):
         self.audio.close()
 
     def remove_peak_annotation(self):
         for fm in self.peak_specmarker:
             fm.remove()
         self.peak_specmarker = []
         for fa in self.peak_annotation:
@@ -184,17 +183,17 @@
         self.axt.set_xlim(self.toffset, self.toffset + self.twindow)
         t0 = int(np.round(self.toffset * self.samplerate))
         t1 = int(np.round((self.toffset + self.twindow) * self.samplerate))
         if t1>len(self.data):
             t1 = len(self.data)
         time = np.arange(t0, t1) / self.samplerate
         if self.trace_artist == None:
-            self.trace_artist, = self.axt.plot(time, self.data[t0:t1])
+            self.trace_artist, = self.axt.plot(time, self.data[t0:t1,self.channel])
         else:
-            self.trace_artist.set_data(time, self.data[t0:t1])
+            self.trace_artist.set_data(time, self.data[t0:t1,self.channel])
         self.axt.set_ylim(self.ymin, self.ymax)
 
         # compute power spectrum:
         n_fft = nfft(self.samplerate, self.freq_resolution)
         t00 = t0
         t11 = t1
         w = t11 - t00
@@ -204,27 +203,28 @@
             t11 = t00 + w
         if t11 >= len(self.data):
             t11 = len(self.data)
             t00 = t11 - w
         if t00 < 0:
             t00 = 0
             t11 = w
-        freqs, power = psd(self.data[t00:t11], self.samplerate,
+        freqs, power = psd(self.data[t00:t11,self.channel], self.samplerate,
                            self.freq_resolution, detrend=ml.detrend_mean)
         self.deltaf = freqs[1] - freqs[0]
         # detect fish:
         h_kwargs = psd_peak_detection_args(self.cfg)
         h_kwargs.update(harmonic_groups_args(self.cfg))
         self.fishlist, fzero_harmonics, self.mains, self.allpeaks, peaks, lowth, highth, center = harmonic_groups(freqs, power, verbose=self.verbose, **h_kwargs)
         highth = center + highth - 0.5 * lowth
         lowth = center + 0.5 * lowth
 
         # spectrogram:
         t2 = t1 + n_fft
-        specpower, freqs, bins = spectrogram(self.data[t0:t2], self.samplerate,
+        freqs, bins, specpower = spectrogram(self.data[t0:t2,self.channel],
+                                             self.samplerate,
                                              self.freq_resolution,
                                              detrend=ml.detrend_mean)
         z = decibel(specpower)
         z = np.flipud(z)
         extent = self.toffset, self.toffset + np.amax(bins), freqs[0], freqs[-1]
         self.axs.set_xlim(self.toffset, self.toffset + self.twindow)
         if self.spectrogram_artist == None:
@@ -314,15 +314,15 @@
                 labels.append('%4.2f Hz' % fpeaks[0])
             elif self.deltaf < 1.0:
                 labels.append('%4.1f Hz' % fpeaks[0])
             else:
                 labels.append('%4.0f Hz' % fpeaks[0])
         if len(self.mains) > 0:
             fpeaks = self.mains[:, 0]
-            fpeakinx = np.array([np.round(fp / self.deltaf) for fp in fpeaks if fp < freqs[-1]], dtype=np.int)
+            fpeakinx = np.array([np.round(fp / self.deltaf) for fp in fpeaks if fp < freqs[-1]], dtype=int)
             fishpoints, = self.axp.plot(fpeaks[:len(fpeakinx)],
                                         power[fpeakinx], linestyle='None',
                                         marker='.', color='k', ms=10, mec=None, mew=0.0, zorder=2)
             self.peak_artists.append(fishpoints)
             labels.append('%3.0f Hz mains' % self.cfg.value('mainsFreq'))
         ncol = (len(labels)-1) // 8 + 1
         self.legendhandle = self.axs.legend(self.peak_artists[:len(labels)], labels, loc='upper right', ncol=ncol)
@@ -357,21 +357,23 @@
                 self.toffset -= 0.5 * self.twindow
                 if self.toffset < 0.0:
                     self.toffset = 0.0
                 self.update_plots()
         elif event.key == 'a':
             if self.min_clip == 0.0 or self.max_clip == 0.0:
                 self.min_clip, self.max_clip = clip_amplitudes(
-                    self.data, **clip_args(self.cfg, self.samplerate))
+                    self.data[:,self.channel],
+                    **clip_args(self.cfg, self.samplerate))
             try:
                 if self.cfg.value('windowSize') <= 0.0:
                     self.cfg.set('windowSize', (len(self.data)-1)/self.samplerate)
                 idx0, idx1, clipped = best_window_indices(
-                    self.data, self.samplerate, min_clip=self.min_clip,
-                    max_clip=self.max_clip, **best_window_args(self.cfg))
+                    self.data[:,self.channel], self.samplerate,
+                    min_clip=self.min_clip, max_clip=self.max_clip,
+                    **best_window_args(self.cfg))
                 if idx1 > 0:
                     self.toffset = idx0 / self.samplerate
                     self.twindow = (idx1 - idx0) / self.samplerate
                     self.twindow *= 2.0/(self.cfg.value('numberPSDWindows')+1.0)
                     self.update_plots()
             except UserWarning as e:
                 if self.verbose > 0:
@@ -418,16 +420,16 @@
             self.ymin = c - h
             self.ymax = c + h
             self.axt.set_ylim(self.ymin, self.ymax)
             self.fig.canvas.draw()
         elif event.key == 'v':
             t0 = int(np.round(self.toffset * self.samplerate))
             t1 = int(np.round((self.toffset + self.twindow) * self.samplerate))
-            min = np.min(self.data[t0:t1])
-            max = np.max(self.data[t0:t1])
+            min = np.min(self.data[t0:t1,self.channel])
+            max = np.max(self.data[t0:t1,self.channel])
             h = 0.5 * (max - min)
             c = 0.5 * (max + min)
             self.ymin = c - h
             self.ymax = c + h
             self.axt.set_ylim(self.ymin, self.ymax)
             self.fig.canvas.draw()
         elif event.key == 'V':
@@ -651,47 +653,48 @@
         if t1>len(self.data):
             t1 = len(self.data)
         time = np.arange(t0, t1) / self.samplerate
         if self.twindow < 1.0:
             ax.set_xlabel('Time [ms]')
             ax.set_xlim(1000.0 * self.toffset,
                         1000.0 * (self.toffset + self.twindow))
-            ax.plot(1000.0 * time, self.data[t0:t1])
+            ax.plot(1000.0 * time, self.data[t0:t1,self.channel])
         else:
             ax.set_xlabel('Time [s]')
             ax.set_xlim(self.toffset, self.toffset + self.twindow)
-            ax.plot(time, self.data[t0:t1])
+            ax.plot(time, self.data[t0:t1,self.channel])
         ax.set_ylabel('Amplitude [{:s}]'.format(self.unit))
         fig.tight_layout()
         fig.savefig(figfile)
         fig.clear()
         plt.close(fig)
         print('saved waveform figure to', figfile)
 
     def play_segment(self):
         t0 = int(np.round(self.toffset * self.samplerate))
         t1 = int(np.round((self.toffset + self.twindow) * self.samplerate))
-        playdata = 1.0 * self.data[t0:t1]
+        playdata = 1.0 * self.data[t0:t1,self.channel]
         fade(playdata, self.samplerate, 0.1)
         self.audio.play(playdata, self.samplerate, blocking=False)
 
     def save_segment(self):
         t0s = int(np.round(self.toffset))
         t1s = int(np.round(self.toffset + self.twindow))
         t0 = int(np.round(self.toffset * self.samplerate))
         t1 = int(np.round((self.toffset + self.twindow) * self.samplerate))
-        savedata = 1.0 * self.data[t0:t1]
+        savedata = 1.0 * self.data[t0:t1,self.channel]
         filename = self.filename.split('.')[0]
         segmentfilename = '{name}-{time0:.4g}s-{time1:.4g}s.wav'.format(
                 name=filename, time0=t0s, time1 = t1s)
         write_audio(segmentfilename, savedata, self.data.samplerate)
         print('saved segment to: ' , segmentfilename)
         
     def play_all(self):
-        self.audio.play(self.data[:], self.samplerate, blocking=False)
+        self.audio.play(self.data[:,self.channel], self.samplerate,
+                        blocking=False)
         
     def play_tone( self, frequency ) :
         self.audio.beep(1.0, frequency)
 
 
 def short_user_warning(message, category, filename, lineno, file=None, line=''):
     if file is None:
@@ -745,20 +748,15 @@
     cfg = configuration()
     cfg.load_files(cfgfile, filepath, 4, verbose-1)
 
     # load data:
     filename = os.path.basename(filepath)
     channel = args.channel
     # TODO: add blocksize and backsize as configuration parameter!
-    with open_data(filepath, channel, 60.0, 10.0, verbose) as data:
-        # plot:
-        ## if len(data) < 10**8:
-        ##     # data[:].copy() makes bestwindow much faster (it's slow in eventdetection):
-        ##     SignalPlot(data[:].copy(), data.samplerate, data.unit, filename, channel)
-        ## else:
+    with DataLoader(filepath, 60.0, 10.0, verbose) as data:
         SignalPlot(data, data.samplerate, data.unit, filename, channel, verbose, cfg)
 
         
 if __name__ == '__main__':
     main()
```

### Comparing `thunderfish-1.9.9/thunderfish/fishshapes.py` & `thunderfish-2.0.0/src/thunderfish/fishshapes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,50 @@
-"""
-Manipulate and plot fish outlines.
+"""Manipulate and plot fish outlines.
 
 ## Fish shapes
 
+Fish shapes are dictionaries with the keys 'body', 'fin0', 'fin1' ...,
+and 'eye'. The values are 2D arrays with x-y coordinates (first
+dimension is points, second dimension coordinates) of the respective
+pathes.
+
 All fish shapes of this module are accessible via these dictionaries:
 
 - `fish_shapes`: dictionary holding all electric fish shapes.
 - `fish_top_shapes`: dictionary holding electric fish shapes viewed from top.
 - `fish_side_shapes`: dictionary holding electric fish shapes viewed from the side.
 
 These are the shapes of various fish species:
 
 - `Alepto_top`: *Apteronotus leptorhynchus* viewed from top.
 - `Alepto_male_side`: Male *Apteronotus leptorhynchus* viewed from the side.
 - `Eigenmannia_top`: *Eigenmannia virescens* viewed from top.
 - `Eigenmannia_side`: *Eigenmannia virescens* viewed from the side.
 
+Helper function for selecting a particular fish shape:
+
+- `fish_shape()`: get a dictinary containing shapes of a fish.
+
 ## Plotting
 
-- `plot_fish()`: plot body and fin of an electric fish.
+- `plot_fish()`: plot body, fins and eye of an electric fish.
 - `plot_object()`: plot circular object.
+- `plot_fishfinder()`: plot a fishfinder with electrodes and wires.
 - `plot_pathes()`: plot pathes.
 
 ## Fish surface and normals from shapes
 
 - `fish_surface()`: generate meshgrid of one side of the fish from shape.
 - `surface_normals()`: normal vectors on a surface.
 
 ## General path manipulations
 
-You may use these functions to extract and fine tune pathes from SVG files in order
-to assemble fish shapes for this module. See `export_fish_demo()` for a use case.
+You may use these functions to extract and fine tune pathes from SVG
+files in order to assemble fish shapes for this module. See
+`export_fish_demo()` for a use case.
 
 - `extract_path()`: convert SVG coordinates to numpy array with path coordinates.
 - `bbox_pathes()`: common bounding box of pathes.
 - `translate_pathes()`: translate pathes in place.
 - `center_pathes()`: translate pathes to their common origin in place.
 - `rotate_pathes()`: rotate pathes in place.
 - `flipy_pathes()`: flip pathes in y-direction in place.
@@ -44,21 +54,23 @@
 - `normalize_path()`: normalize fish outline to unit length.
 - `bend_path()`: bend and scale a path.
 
 ## Exporting fish outlines from pathes
 
 - `export_fish()`: serialize coordinates of fish outlines as a dictionary.
 - `export_fish_demo()`: code demonstrating how to export fish outlines from SVG.
+
 """
 
 import numpy as np
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from matplotlib.path import Path
-from matplotlib.patches import PathPatch, Circle
+from matplotlib.patches import PathPatch, Circle, Rectangle
+import matplotlib.transforms as mpt
 
 
 Alepto_top = dict(body=np.array([
     [-5.00000000e-01, 0.00000000e+00], [-4.99802704e-01, 1.23222860e-03],
     [-4.95374557e-01, 2.57983066e-03], [-4.84420392e-01, 3.29085947e-03],
     [-4.72487909e-01, 4.03497963e-03], [-4.13995354e-01, 4.39637211e-03],
     [-3.90529212e-01, 5.14049228e-03], [-3.67089631e-01, 5.88461244e-03],
@@ -116,15 +128,15 @@
     [-2.38198570e-01, -1.03918950e-02], [-2.61664711e-01, -9.24382081e-03],
     [-2.79461930e-01, -8.49142780e-03], [-2.97063253e-01, -8.11708180e-03],
     [-3.20104187e-01, -7.39418800e-03], [-3.43596916e-01, -6.65006783e-03],
     [-3.67089631e-01, -5.88461244e-03], [-3.90529212e-01, -5.14049228e-03],
     [-4.13995354e-01, -4.39637211e-03], [-4.72487909e-01, -4.03497963e-03],
     [-4.84420392e-01, -3.29085947e-03], [-4.95374557e-01, -2.57983066e-03],
     [-4.99802704e-01, -1.23222860e-03], [-5.00000000e-01, -0.00000000e+00],]))
-""" Outline of an *Apteronotus leptorhynchus* viewed from top, modified from Krahe 2004. """
+"""Outline of an *Apteronotus leptorhynchus* viewed from top, modified from Krahe 2004."""
 
 Alepto_male_side = dict(body=np.array([
     [2.80332097e-01, 5.51361973e-02], [2.41127905e-01, 5.93460338e-02],
     [1.91463866e-01, 6.22667811e-02], [1.37379023e-01, 6.17716006e-02],
     [6.91234340e-02, 5.72953633e-02], [-1.36051588e-02, 4.74838393e-02],
     [-7.55221954e-02, 3.64211032e-02], [-1.60157310e-01, 2.45651115e-02],
     [-2.32035003e-01, 1.55421483e-02], [-2.99079447e-01, 9.70960800e-03],
@@ -181,15 +193,15 @@
     [-1.68443229e-01, -3.68996138e-02], [-1.12717944e-01, -4.88585839e-02],
     [-7.07908982e-02, -5.51259999e-02], [-1.80906639e-02, -6.16068166e-02],
     [2.75299392e-02, -6.53080983e-02], [7.71390030e-02, -6.85205021e-02],
     [1.21071140e-01, -7.25104674e-02], [1.78723549e-01, -7.85286909e-02],
     [2.32100395e-01, -8.40268652e-02], [2.74938812e-01, -8.74456073e-02],
     [3.10041908e-01, -8.43007220e-02],]),
     eye=np.array([0.4, 0.0, 0.01]))
-""" Outline of an *Apteronotus leptorhynchus* male viewed from the side. """
+"""Outline of an *Apteronotus leptorhynchus* male viewed from the side."""
 
 Eigenmannia_top = dict(body=np.array([
     [-5.00000000e-01, 0.00000000e+00], [-4.84515329e-01, 4.41536208e-03],
     [-4.76913801e-01, 5.34924846e-03], [-3.94680346e-01, 8.25734868e-03],
     [-2.74106007e-01, 8.94059314e-03], [-1.35145770e-01, 1.09559947e-02],
     [2.36080412e-02, 1.40941342e-02], [1.36968804e-01, 1.51550643e-02],
     [2.15041020e-01, 1.96734219e-02], [2.83582110e-01, 2.36895289e-02],
@@ -221,15 +233,15 @@
     [3.62525174e-01, -3.12766064e-02], [3.68462758e-01, -2.97229886e-02],
     [3.46646908e-01, -2.77590937e-02], [3.20834553e-01, -2.63067663e-02],
     [2.83582110e-01, -2.36895289e-02], [2.15041020e-01, -1.96734219e-02],
     [1.36968804e-01, -1.51550643e-02], [2.36080412e-02, -1.40941342e-02],
     [-1.35145770e-01, -1.09559947e-02], [-2.74106007e-01, -8.94059314e-03],
     [-3.94680346e-01, -8.25734868e-03], [-4.76913801e-01, -5.34924846e-03],
     [-4.84515329e-01, -4.41536208e-03], [-5.00000000e-01, -0.00000000e+00],]))
-""" Outline of an *Eigenmannia virescens* viewed from top. """
+"""Outline of an *Eigenmannia virescens* viewed from top."""
 
 Eigenmannia_side = dict(body=np.array([
     [7.39835590e-02, 4.57421567e-02], [1.36190672e-01, 5.20008556e-02],
     [1.88575637e-01, 5.31087788e-02], [2.55693889e-01, 4.90162062e-02],
     [2.91989388e-01, 4.57421567e-02], [3.30997244e-01, 4.08310609e-02],
     [3.60079352e-01, 3.50312357e-02], [3.86267547e-01, 2.72057399e-02],
     [4.09748495e-01, 1.88510343e-02], [4.30914243e-01, 1.02069720e-02],
@@ -300,34 +312,61 @@
     [1.25654422e-01, -5.85499724e-02], [9.49792270e-02, -5.56561016e-02],
     [4.05741354e-02, -5.11056947e-02], [-1.24746680e-03, -4.58268936e-02],
     [-5.20302500e-02, -3.81131387e-02], [-1.01805114e-01, -3.16101258e-02],
     [-1.51874267e-01, -2.50855445e-02], [-2.01943420e-01, -2.02074944e-02],
     [-2.61607516e-01, -1.41653476e-02], [-3.02124016e-01, -9.83478430e-03],
     [-3.12840355e-01, -9.28491550e-03],]),
     eye=np.array([0.46, -0.03, 0.005]))
-""" Outline of an *Eigenmannia virescens* viewed from the side. """
+"""Outline of an *Eigenmannia virescens* viewed from the side."""
 
 fish_shapes = dict(Alepto_top=Alepto_top,
                    Alepto_male_side=Alepto_male_side,
                    Eigenmannia_top=Eigenmannia_top,
                    Eigenmannia_side=Eigenmannia_side)
-""" Dictionary holding all electric fish shapes. """
+"""Dictionary holding all electric fish shapes."""
 
 fish_top_shapes = dict(Alepto=Alepto_top,
                        Eigenmannia=Eigenmannia_top)
-""" Dictionary holding electric fish shapes viewed from top. """
+"""Dictionary holding electric fish shapes viewed from top."""
 
 fish_side_shapes = dict(Alepto_male=Alepto_male_side,
                    Eigenmannia=Eigenmannia_side)
-""" Dictionary holding electric fish shapes viewed from the side. """
+"""Dictionary holding electric fish shapes viewed from the side."""
+
+
+def fish_shape(fish):
+    """Get a dictinary containing shapes of a fish.
+
+    Parameters
+    ----------
+    fish: string or tuple or dict
+        Specifies a fish to show:
+        - any of the strings defining a shape contained in the `fish_shapes` dictionary,
+        - a tuple with the name of the fish as the first element and 'top' or 'side' as the second element,
+        - a dictionary with at least a 'body' key holding pathes to be drawn.
+
+    Returns
+    -------
+    fish: dict
+        Dictionary with at least a 'body' key holding pathes to be drawn.
+    """
+    if not isinstance(fish, dict):
+        if isinstance(fish, (tuple, list)):
+            if fish[1] == 'top':
+                fish = fish_top_shapes[fish[0]]
+            else:
+                fish = fish_side_shapes[fish[0]]
+        else:
+            fish = fish_shapes[fish]
+    return fish
     
 
 def plot_fish(ax, fish, pos=(0, 0), direction=(1, 0), size=20.0, bend=0, scaley=1,
               bodykwargs={}, finkwargs={}, eyekwargs=None):
-    """ Plot body and fin of an electric fish.
+    """Plot body, fins and eye of an electric fish.
 
     Parameters
     ----------
     ax: matplotlib axes
         Axes where to draw the fish.
     fish: string or tuple or dict
         Specifies a fish to show:
@@ -365,23 +404,15 @@
     fish = (('Eigenmannia', 'side'), (0, 0), (1, 0), 20.0, -25)
     plot_fish(ax, *fish, bodykwargs=bodykwargs, finkwargs=finkwargs)
     ax.set_xlim(-15, 15)
     ax.set_ylim(-10, 10)
     plt.show()
     ```
     """
-    # retrieve fish shape:
-    if not isinstance(fish, dict):
-        if isinstance(fish, (tuple, list)):
-            if fish[1] == 'top':
-                fish = fish_top_shapes[fish[0]]
-            else:
-                fish = fish_side_shapes[fish[0]]
-        else:
-            fish = fish_shapes[fish]
+    fish = fish_shape(fish)
     bpatch = None
     size_fac = 1.1
     bbox = bbox_pathes(*fish.values())
     trans = mpl.transforms.Affine2D()
     angle = np.arctan2(direction[1], direction[0])
     trans.rotate(angle)
     #trans.scale(dxu/dyu, dyu/dxu)   # what is the right scaling????
@@ -416,37 +447,140 @@
         if part == 'body':
             bpatch = patch
         ax.add_patch(patch)
     return bpatch
 
 
 def plot_object(ax, pos=(0, 0), radius=1.0, **kwargs):
-    """ Plot circular object.
+    """Plot circular object.
 
     Parameters
     ----------
     ax: matplotlib axes
-        Axes where to draw the fish.
+        Axes where to draw the object.
     pos: tuple of floats
         Coordinates of the objects's position (its center).
     radius: float
         Radius of the cirular object.
     kwargs: key word arguments
-        Arguments for PathPatch used to draw the fish.
+        Arguments for Circle used to draw the obkect.
     """
     ax.add_patch(Circle(pos, radius, **kwargs))
 
+    
+def plot_fishfinder(ax, pos, direction, length, handle=0.05,
+                    central_ground=False, wires=False,
+                    rodkwargs=dict(edgecolor='none', facecolor='gray'),
+                    poskwargs=dict(edgecolor='none', facecolor='red'),
+                    negkwargs=dict(edgecolor='none', facecolor='blue'),
+                    gndkwargs=dict(edgecolor='none', facecolor='black'),
+                    lw=1, zorder=50):
+    """Plot a fishfinder with electrodes and wires.
+
+    Parameters
+    ----------
+    ax: matplotlib axes
+        Axes where to draw the fishfinder.
+    pos: tuple of floats
+        Coordinates of the fishfinder's position (its center).
+    direction: tuple of floats
+        Coordinates defining the orientation of the fishfinder.
+    length: float
+        Length of the fishfinder (center of positive electrode
+        minus center of negative electrode).
+    handle: float
+        Length of handle (rod beyond the negative electrode)
+        as a fraction of the `length` of fishfinder.
+    central_ground: bool
+        Add a central ground electrode.
+    wires: bool, 'postop' or 'negtop'
+        Draw wires for each electrode.
+        - True or 'postop': draw wire of positive electrode on top.
+        - 'negtop': draw wire of negative electrode on top.
+        Return the coordinates of the endpoints of the wires.
+    rodkwargs: dict
+        Key-word arguments for Rectangle used to draw the rod.
+    poskwargs: dict
+        Key-word arguments for Rectangle used to draw the positive electrode.
+    negkwargs: dict
+        Key-word arguments for Rectangle used to draw the negative electrode.
+    gndkwargs: dict
+        Key-word arguments for Rectangle used to draw the ground electrode.
+    lw: float
+        Width of the lines used for drawing the wires.
+    zorder: int
+        zorder for the fishfinder.
+
+    Returns
+    -------
+    negpos: tuple of floats
+        Coordinates of center of negative electrode.
+    pospos: tuple of floats
+        Coordinates of center of positive electrode.
+    negwirepos: tuple of floats
+        If `wire`, the end of the wire of the negative electrode.
+    poswirepos: tuple of floats
+        If `wire`, the end of the wire of the positive electrode.
+    gndwirepos: tuple of floats
+        If `central_ground` and `wire`, the end of the wire of
+        the ground electrode.
+    """
+    width = 0.07*length
+    transform = mpt.Affine2D().rotate(np.arctan2(direction[1], direction[0])).translate(*pos)
+
+    ax.add_patch(Rectangle((-(0.5+handle)*length, -0.5*width),
+                           (1+handle+0.05)*length, width,
+                           transform=transform + ax.transData,
+                           zorder=zorder, **rodkwargs))
+    ax.add_patch(Rectangle((0.5*length-0.4*width, -0.6*width),
+                           0.8*width, 1.2*width,
+                           transform=transform + ax.transData,
+                           zorder=zorder+2, **poskwargs))
+    ax.add_patch(Rectangle((-0.5*length-0.4*width, -0.6*width),
+                           0.8*width, 1.2*width,
+                           transform=transform + ax.transData,
+                           zorder=zorder+2, **negkwargs))
+    nodes = [(-0.5*length, 0), (0.5*length, 0)]
+    if central_ground:
+        ax.add_patch(Rectangle((-0.4*width, -0.6*width),
+                               0.8*width, 1.2*width,
+                               transform=transform + ax.transData,
+                               zorder=zorder+2, **gndkwargs))
+    if wires:
+        offs = 0.03*width*lw
+        if wires == 'negtop':
+            offs *= -1
+        if central_ground:
+            offs *= 2
+        color = negkwargs.get('facecolor')
+        ax.plot((-0.5*length, -(0.5+handle)*length), (-offs, -offs),
+                color=color, lw=lw, solid_capstyle='butt',
+                transform=transform + ax.transData, zorder=zorder+1)
+        color = poskwargs.get('facecolor')
+        ax.plot((0.5*length, -(0.5+handle)*length), (offs, offs),
+                color=color, lw=lw, solid_capstyle='butt', transform=transform +
+                ax.transData, zorder=zorder+1)
+        nodes.extend(((-(0.5+handle)*length, -offs), (-(0.5+handle)*length, offs)))
+        if central_ground:
+            color = gndkwargs.get('facecolor')
+            ax.plot((0, -(0.5+handle)*length), (0, 0),
+                    color=color, lw=lw, solid_capstyle='butt',
+                    transform=transform + ax.transData, zorder=zorder+1)
+            nodes.append((-(0.5+handle)*length, 0))
+    nodes = transform.transform(nodes)
+    return nodes
+
 
 def plot_pathes(ax, *vertices, **kwargs):
-    """ Plot pathes.
+    """Plot pathes.
 
     Parameters
     ----------
     ax: matplotlib axes
-        Axes where to draw the fish.
+        Axes where to draw the path.
     vertices: one or more 2D arrays
         The coordinates of pathes to be plotted
         (first column x-coordinates, second colum y-coordinates).
     kwargs: key word arguments
         Arguments for PathPatch used to draw the path.
     """
     for verts in vertices:
@@ -463,15 +597,15 @@
     bbox += center
     ax.set_xlim(*bbox[:,0])
     ax.set_ylim(*bbox[:,1])
 
 
 def fish_surface(fish, pos=(0, 0), direction=(1, 0), size=20.0, bend=0,
                  gamma=1.0):
-    """ Generate meshgrid of one side of the fish from shape.
+    """Generate meshgrid of one side of the fish from shape.
     
     Parameters
     ----------
     fish: string or tuple or dict
         Specifies a fish to show:
         - any of the strings defining a shape contained in the `fish_shapes` dictionary,
         - a tuple with the name of the fish and 'top' or 'side',
@@ -496,23 +630,15 @@
     yy: 2D array of floats
         y-coordinates in direction upwards from body axis.
     zz: 2D array of floats
         z-coordinates of fish surface, outside of fish NaN.
     """
     if direction[1] != 0:
         raise ValueError('rotation not supported by fish_surface yet.')
-    # retrieve fish shape:
-    if not isinstance(fish, dict):
-        if isinstance(fish, (tuple, list)):
-            if fish[1] == 'top':
-                fish = fish_top_shapes[fish[0]]
-            else:
-                fish = fish_side_shapes[fish[0]]
-        else:
-            fish = fish_shapes[fish]
+    fish = fish_shape(fish)
     bbox = bbox_pathes(*fish.values())
     size_fac = -1.05*0.5/bbox[0,0]
     path = bend_path(fish['body'], bend, size, size_fac)
     # split in top and bottom half:
     minxi = np.argmin(path[:,0])
     maxxi = np.argmax(path[:,0])
     i0 = min(minxi, maxxi)
@@ -551,15 +677,15 @@
     y = np.linspace(np.min(midline[:,1]-diamy), np.max(midline[:,1]+diamy), n//2)
     xx, yy = np.meshgrid(x ,y)
     zz = diamz * (np.sqrt(1.0 - ((yy-midline[:,1])/diamy)**2))**gamma
     return xx, yy, zz
 
 
 def surface_normals(xx, yy, zz):
-    """ Normal vectors on a surface.
+    """Normal vectors on a surface.
 
     Compute surface normals on a surface as returned by `fish_surface()`.
 
     Parameters
     ----------
     xx: 2D array of floats
         Mesh grid of x coordinates.
@@ -585,15 +711,15 @@
     ny[:-1,:] = -np.diff(zz, axis=0)/dy
     nz = np.ones(xx.shape)
     norm = np.sqrt(nx*nx+ny*ny+1)
     return nx/norm, ny/norm, nz/norm
 
 
 def extract_path(data):
-    """ Convert SVG coordinates to numpy array with path coordinates.
+    """Convert SVG coordinates to numpy array with path coordinates.
 
     Draw a fish outline in inkscape. Open the XML Editor (shift+ctrl+x)
     and copy the value of the data field ('d') into a variable that you
     pass to this function.
     Alternatively, try the 'inkscape:original-d' variable.
 
     Parameters
@@ -629,15 +755,15 @@
             elif c in 'mlc':
                 relative = True
     vertices = np.array(vertices)
     return vertices
 
 
 def bbox_pathes(*vertices):
-    """ Common bounding box of pathes.
+    """Common bounding box of pathes.
 
     Parameters
     ----------
     vertices: one or more 2D arrays
         The coordinates of pathes
         (first column x-coordinates, second colum y-coordinates).
 
@@ -662,15 +788,15 @@
             bbox[0,1] = min(bbox[0,1], vbbox[0,1])
             bbox[1,0] = max(bbox[1,0], vbbox[1,0])
             bbox[1,1] = max(bbox[1,1], vbbox[1,1])
     return bbox
 
 
 def translate_pathes(dx, dy, *vertices):
-    """ Translate pathes in place.
+    """Translate pathes in place.
 
     Parameters
     ----------
     dx: float
         Shift in x direction.
     dy: float
         Shift in y direction.
@@ -680,15 +806,15 @@
     """
     for verts in vertices:
         verts[:,0] += dx
         verts[:,1] += dy
 
 
 def center_pathes(*vertices):
-    """ Translate pathes to their common origin in place.
+    """Translate pathes to their common origin in place.
 
     Parameters
     ----------
     vertices: one or more 2D arrays
         The coordinates of pathes to be centered
         (first column x-coordinates, second colum y-coordinates).
     """
@@ -696,15 +822,15 @@
     # shift:
     for verts in vertices:
         verts[:,0] -= center[0]
         verts[:,1] -= center[1]
 
 
 def rotate_pathes(theta, *vertices):
-    """ Rotate pathes in place.
+    """Rotate pathes in place.
 
     Parameters
     ----------
     theta: float
         Rotation angle in degrees.
     vertices: one or more 2D arrays
         The coordinates of pathes to be rotated
@@ -717,41 +843,41 @@
     rm = np.array(((c, -s), (s, c)))
     # rotation:
     for verts in vertices:
         verts[:,:] = np.dot(verts, rm)
 
 
 def flipx_pathes(*vertices):
-    """ Flip pathes in x-direction in place.
+    """Flip pathes in x-direction in place.
 
     Parameters
     ----------
     vertices: one or more 2D arrays
         The coordinates of pathes to be flipped
         (first column x-coordinates, second colum y-coordinates).
     """
     for verts in vertices:
         verts[:,0] = -verts[:,0]
 
 
 def flipy_pathes(*vertices):
-    """ Flip pathes in y-direction in place.
+    """Flip pathes in y-direction in place.
 
     Parameters
     ----------
     vertices: one or more 2D arrays
         The coordinates of pathes to be flipped
         (first column x-coordinates, second colum y-coordinates).
     """
     for verts in vertices:
         verts[:,1] = -verts[:,1]
 
 
 def mirror_path(vertices1):
-    """ Complete path of half a fish outline by appending the mirrored path.
+    """Complete path of half a fish outline by appending the mirrored path.
 
     It is sufficient to draw half of a top view of a fish. Import with
     extract_path() and use this function to add the missing half of the
     outline to the path. The outline is mirrored on the x-axis.
 
     Parameters
     ----------
@@ -767,15 +893,15 @@
     vertices2 = np.array(vertices1[::-1,:])
     vertices2[:,1] *= -1
     vertices = np.concatenate((vertices1, vertices2))
     return vertices
 
 
 def normalize_path(*vertices):
-    """ Normalize and shift path in place.
+    """Normalize and shift path in place.
 
     The path extent in x direction is normalized to one and its center
     is shifted to the origin.
 
     Parameters
     ----------
     vertices: one or more 2D arrays
@@ -787,15 +913,15 @@
         verts[:,1] -= np.mean(bbox[:,1])
         verts[:,0] -= bbox[0,0]
         verts /= bbox[1,0] - bbox[0,0]
         verts[:,0] -= 0.5
 
 
 def bend_path(path, bend, size, size_fac=1.0):
-    """ Bend and scale a path.
+    """Bend and scale a path.
 
     Parameters
     ----------
     path: 2D array
         The coordinates of a path.
     bend: float
         Angle for bending in degrees.
@@ -820,15 +946,15 @@
         R = r-yp                              # radius of point
         path[sel,0] = -np.abs(R*np.sin(beta)) # transformed x coordinates
         path[sel,1] = r-R*np.cos(beta)        # transformed y coordinates
     return path
         
 
 def export_path(vertices):
-    """ Print coordinates of path for import as numpy array.
+    """Print coordinates of path for import as numpy array.
 
     The variable name, a leading 'np.array([' and the closing '])'
     are not printed.
 
     Parameters
     ----------
     vertices: 2D array
@@ -841,15 +967,15 @@
             print('   ', end='')
         print(' [%.8e, %.8e],' % (v[0], v[1]), end='')
         if k%n == n-1 and k < len(vertices)-1:
             print('')
 
 
 def export_fish(name, body, *fins):
-    """ Serialize coordinates of fish outlines as a dictionary.
+    """Serialize coordinates of fish outlines as a dictionary.
 
     Writes a dictionary with name 'name' and keys 'body', 'fin0', 'fin1', ...
     holding the pathes.
 
     Copy these coordinates from the console and paste them into this module.
     Give it a proper name and don't forget to add it to the fish_shapes dictionary
     to make it know to plot_fish().
@@ -879,15 +1005,15 @@
         export_path(f)
         fish['fin%d' % k] = f
     print(']))')
     return fish
 
 
 def export_fish_demo():
-    """ Code demonstrating how to export a fish outline from SVG.
+    """Code demonstrating how to export a fish outline from SVG.
     """
     # copy the path specification from an SVG object:
     data = "m 84.013672,21.597656 0.0082,83.002434 0.113201,-0.0145 0.1238,-0.32544 0.06532,-0.80506 0.06836,-0.87696 0.0332,-4.298823 v -8.625 l 0.06836,-1.724609 0.06836,-1.722657 0.07032,-1.726562 0.06836,-1.726563 0.06641,-1.693359 0.03439,-1.293583 0.06912,-1.30798 0.10547,-1.724609 0.10156,-1.724609 0.10352,-1.726563 0.10352,-1.724609 0.13867,-1.72461 0.171876,-2.572265 0.13672,-1.72461 0.13672,-1.726562 0.10352,-1.724609 0.06836,-1.722657 0.103515,-2.574219 0.06836,-1.722656 0.10352,-1.728515 0.07032,-1.722657 0.06836,-1.724609 0.240234,-1.724609 0.34375,-1.72461 0.134766,-1.726562 0.10352,-1.69336 0.03516,-0.875 0.07031,-1.728515 v -0.847657 l -0.07273,-2.246267 -0.0172,-0.184338 0.15636,0.09441 0.384252,1.019739 0.748821,0.905562 1.028854,0.647532 1.356377,-0.03149 0.362644,-0.347764 -0.264138,-0.736289 -1.268298,-1.126614 -1.363988,-0.922373 -0.927443,-0.451153 -0.228986,-0.07018 -0.0015,-0.21624 0.03663,-0.660713 0.480469,-0.847657 -0.101563,-0.876953 -0.103515,-0.845703 -0.103516,-0.876953 -0.207031,-1.695313 -0.273438,-1.724609 -0.308594,-1.726562 -0.27539,-1.72461 -0.310547,-1.722656 -0.240234,-0.878906 -0.400196,-0.877344 -0.53927,-0.596268 -0.486573,-0.216683 z"
     verts = extract_path(data)
     # look at the path:
     fig, ax = plt.subplots()
     plot_pathes(ax, verts)
@@ -910,19 +1036,19 @@
               finkwargs=dict(lw=1, edgecolor='k', facecolor='b'))
     ax.set_xlim(-1.5, 1.5)
     ax.set_ylim(-1, 1)
     plt.show()
 
     
 def main():
-    """ Plot some fish shapes and surface normals.
+    """Plot some fish shapes and surface normals.
     """
-    bodykwargs=dict(lw=1, edgecolor='k', facecolor='none')
-    finkwargs=dict(lw=1, edgecolor='k', facecolor='grey')
-    eyekwargs=dict(lw=1, edgecolor='white', facecolor='grey')
+    bodykwargs = dict(lw=1, edgecolor='k', facecolor='none')
+    finkwargs = dict(lw=1, edgecolor='k', facecolor='grey')
+    eyekwargs = dict(lw=1, edgecolor='white', facecolor='grey')
     var = ['zz', 'nx', 'ny', 'nz']
     fig, ax = plt.subplots()
     for k in range(4):
         y = (1.5-k)*9
         fish = (('Alepto_male', 'side'), (0, y), (1, 0), 20.0, 0)
         xx, yy, zz = fish_surface(*fish, gamma=0.5)
         nx, ny, nz = surface_normals(xx, yy, zz)
@@ -937,23 +1063,27 @@
     ilumn = [-0.05, 0.1, 1.0]
     dv = np.zeros(nv[0].shape)
     for nc, ic in zip(nv, ilumn):
         dv += nc*ic
     #ax.contourf(xx[0,:], yy[:,0], dv, 20, cmap='gist_gray')
     ax.contourf(xx[0,:], yy[:,0], dv, levels=[np.nanmin(dv), np.nanmin(dv)+0.99*(np.nanmax(dv)-np.nanmin(dv)), np.nanmax(dv)], cmap='gist_gray')
     plot_fish(ax, *fish, bodykwargs=bodykwargs, finkwargs=finkwargs, eyekwargs=eyekwargs)
-    bodykwargs=dict(lw=1, edgecolor='k', facecolor='k')
-    fish = (('Alepto', 'top'), (23, 0), (2, 1), 16.0, -25)
+    bodykwargs = dict(lw=1, edgecolor='k', facecolor='k')
+    fish = (('Alepto', 'top'), (23, 0), (2, 1), 16.0, 25)
     plot_fish(ax, *fish, bodykwargs=bodykwargs, finkwargs=finkwargs)
     fish = (('Eigenmannia', 'top'), (23, 8), (1, 0.3), 16.0, -15)
     plot_fish(ax, *fish, bodykwargs=bodykwargs, finkwargs=finkwargs)
     fish = (('Eigenmannia', 'side'), (20, 18), (1, 0), 20.0, -25)
     plot_fish(ax, *fish, bodykwargs=bodykwargs, finkwargs=finkwargs, eyekwargs=eyekwargs)
-    ax.set_xlim(-15, 35)
+    plot_fishfinder(ax, (38, 13), (1, 2), 18, handle=0.2,
+                    central_ground=True, wires=True, lw=2)
+    plot_fishfinder(ax, (38, -8), (1, 2), 18, central_ground=False)
+    ax.set_xlim(-15, 45)
     ax.set_ylim(-20, 24)
+    ax.set_aspect('equal')
     plt.show()
 
 
 if __name__ == '__main__':
     #export_fish_demo()
     main()
```

### Comparing `thunderfish-1.9.9/thunderfish/harmonics.py` & `thunderfish-2.0.0/src/thunderfish/harmonics.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,30 +49,29 @@
                                in power spectra from configuration.
 - `add_harmonic_groups_config()`: add parameters for the detection of
                                   harmonic groups to configuration.
 - `harmonic_groups_args()`: retrieve parameters for the detection of
                             harmonic groups from configuration.
 """
 
-from __future__ import print_function
 import math as m
 import numpy as np
 import scipy.signal as sig
-from .eventdetection import detect_peaks, trim, hist_threshold
-from .powerspectrum import decibel, power, plot_decibel_psd
+from thunderlab.eventdetection import detect_peaks, trim, hist_threshold
+from thunderlab.powerspectrum import decibel, power, plot_decibel_psd
 try:
     import matplotlib.cm as cm
     import matplotlib.colors as mc
 except ImportError:
     pass
 
 
 def group_candidate(good_freqs, all_freqs, freq, divisor,
                     freq_tol, max_freq_tol, min_group_size, verbose):
-    """ Candidate harmonic frequencies belonging to a fundamental frequency.
+    """Candidate harmonic frequencies belonging to a fundamental frequency.
 
     Parameters
     ----------
     good_freqs: 2-D array
         Frequency, power, and use count (columns) of strong peaks detected
         in a power spectrum.
     all_freqs: 2-D array
@@ -115,14 +114,23 @@
         divisor = 1
         dvs = False
         
     # 1. find harmonics in good_freqs and adjust fzero accordingly:
     fzero = freq
     fzero_harmonics = 1
     if len(good_freqs[:,0]) > 0:
+        """
+        ff = good_freqs[:,0]
+        h = np.round(ff/fzero)
+        h_indices = np.unique(h, return_index=True)[1]
+        f_best = [hi+np.argmin(np.abs(fh/h - fzero)) for hi, fh in zip(h_indices, np.split(ff, h_indices))]
+        fe = np.abs(ff/h - fzero)
+        h = h[fe < freq_tol]
+        fe = fe[fe < freq_tol]
+        """
         prev_freq = divisor * freq
         for h in range(divisor+1, 2*min_group_size+1):
             idx = np.argmin(np.abs(good_freqs[:,0]/h - fzero))
             ff = good_freqs[idx,0]
             if m.fabs(ff/h - fzero) > freq_tol:
                 continue
             df = ff - prev_freq
@@ -148,15 +156,15 @@
     # freq might not be in our group anymore, because fzero was adjusted:
     if np.abs(freq - fzero) > freq_tol:
         if verbose > 0:
             print('  discarded: lost frequency')
         return [], -1.0, fzero_harmonics
 
     # 3. collect harmonics from all_freqs:
-    new_group = -np.ones(min_group_size, dtype=np.int)
+    new_group = -np.ones(min_group_size, dtype=int)
     new_penalties = np.ones(min_group_size)
     freqs = []
     prev_h = 0
     prev_fe = 0.0
     for h in range(1, min_group_size+1):
         penalty = 0
         i = np.argmin(np.abs(all_freqs[:,0]/h - fzero))
@@ -229,15 +237,15 @@
 
     # 5. return results:
     return new_group, fzero, fzero_harmonics
 
 
 def update_group(good_freqs, all_freqs, new_group, fzero,
                  freq_tol, verbose, group_str):
-    """ Update good frequencies and harmonic group.
+    """Update good frequencies and harmonic group.
 
     Remove frequencies from good_freqs, add missing fundamental to group.
 
     Parameters
     ----------
     good_freqs: 2-D array
         Frequency, power, and use count (columns) of strong peaks detected
@@ -274,15 +282,15 @@
     # indices of group in good_freqs:
     freq_tol *= 1.1
     indices = []
     for f in group[:,0]:
         idx = np.argmin(np.abs(good_freqs[:,0]-f))
         if np.abs(good_freqs[idx,0]-f) <= freq_tol:
             indices.append(idx)
-    indices = np.asarray(indices, dtype=np.int)
+    indices = np.asarray(indices, dtype=int)
 
     # harmonics in good_freqs:
     nharm = np.round(good_freqs[:,0]/fzero)
     idxs = np.where(np.abs(good_freqs[:,0] - nharm*fzero) <= freq_tol)[0]
     indices = np.unique(np.concatenate((indices, idxs)))
 
     # report:
@@ -505,15 +513,15 @@
                                      fzero, freq_tol, verbose, group_str)
 
     # good_freqs: removed all frequencies of bestgroup
     return good_freqs, group, new_group, fzero_harmonics
 
 
 def expand_group(group, indices, freqs, freq_tol, max_harmonics=0):
-    """ Add more harmonics to harmonic group.
+    """Add more harmonics to harmonic group.
     
     Parameters
     ----------
     group: 2-D array
         Group of fundamental frequency and harmonics
         as returned by build_harmonic_group.
     indices: 1-D array of indices
@@ -560,15 +568,15 @@
         group_freqs.append(f)
         indices.append(i)
     # assemble group:
     new_group = freqs[indices,:group.shape[1]]
     # keep filled in fundamental:
     if group[0,2] == -2:
         new_group = np.vstack((group[0,:], new_group))
-    return new_group, np.array(indices, dtype=np.int)
+    return new_group, np.array(indices, dtype=int)
             
 
 def extract_fundamentals(good_freqs, all_freqs, freq_tol, max_freq_tol,
                          verbose=0, check_freqs=[],
                          mains_freq=60.0, mains_freq_tol=1.0,
                          min_freq=0.0, max_freq=2000.0, max_db_diff=20.0,
                          max_divisor=4, min_group_size=3, max_harmonics_db=-5.0,
@@ -892,15 +900,15 @@
     max_harmonics: int
         Maximum number of harmonics to be returned for each group.
     max_groups: int
         If not zero the maximum number of most powerful harmonic groups.
 
     Returns
     -------
-    group_list: list of 2-D arrays
+    groups: list of 2-D arrays
         List of all extracted harmonic groups, sorted by fundamental frequency.
         Each harmonic group is a 2-D array with the first dimension the harmonics
         and the second dimension containing frequency and power of each harmonic.
         If the power is zero, there was no corresponding peak in the power spectrum.
     fzero_harmonics: list of ints
         The harmonics from which the fundamental frequencies were computed.
     mains: 2-d array
@@ -1015,16 +1023,16 @@
             f = fundamental_freqs(groups)
             fundamentals.append(f)
     return fundamentals
 
 
 def fundamental_freqs_and_power(group_list, power=False,
                                 ref_power=1.0, min_power=1e-20):
-    """
-    Extract fundamental frequencies and their power in dB from lists of harmonic groups.
+    """Extract fundamental frequencies and their power in dB from lists
+    of harmonic groups.
 
     The inner list of 2-D arrays of the input argument is transformed
     into a 2-D array containig for each fish (1st dimension) the
     fundamental frequencies and powers (summed over all harmonics)
     extracted from the 2-D arrays.
     
     Parameters
@@ -1032,29 +1040,28 @@
     group_list: (list of (list of ...)) list of 2-D arrays
         Arbitrarily nested lists of harmonic groups as returned by
         extract_fundamentals() and harmonic_groups() with the element
         [0, 0] being the fundamental frequency and the elements [:,1] being
         the powers of each harmonics.
     power: boolean
         If `False` convert the power into decibel using the
-        powerspectrum.decibel() function.
+        `thunderlab.powerspectrum.decibel()` function.
     ref_power: float
         Reference power for computing decibel.
         If set to `None` the maximum power is used.
     min_power: float
         Power values smaller than `min_power` are set to `-np.inf`.
 
     Returns
     -------
     fundamentals: (list of (list of ...)) 2-D array
         Nested list (corresponding to `group_list`) of 2-D arrays
         with fundamental frequencies in first column and
         corresponding power in second column.
     """
-
     if len(group_list) == 0:
         return np.array([])
 
     # check whether group_list is list of harmonic groups:
     list_of_groups = True
     for group in group_list:
         if not ( hasattr(group, 'shape') and len(group.shape) == 2 ):
@@ -1073,15 +1080,15 @@
             f = fundamental_freqs_and_power(groups, power,
                                             ref_power, min_power)
             fundamentals.append(f)
     return fundamentals
 
 
 def add_relative_power(freqs):
-    """ Add a column with relative power.
+    """Add a column with relative power.
 
     For each element in `freqs`, its maximum power is subtracted
     from all powers.
 
     Parameters
     ----------
     freqs: list of 2-D arrays
@@ -1095,15 +1102,15 @@
     power_freqs: list of 2-D arrays
         Same as freqs, but with an added column containing the relative power.
     """
     return [np.column_stack((f, f[:,1] - np.max(f[:,1]))) for f in freqs]
 
 
 def add_power_ranks(freqs):
-    """ Add a column with power ranks.
+    """Add a column with power ranks.
 
     Parameters
     ----------
     freqs: list of 2-D arrays
         First column in the arrays is fundamental frequency and
         second column the corresponding power.
         Further columns are optional and kept in the returned list.
@@ -1122,15 +1129,15 @@
         ranks = np.empty_like(i)
         ranks[i] = -np.arange(len(i))
         rank_freqs.append(np.column_stack((f, ranks)))
     return rank_freqs
 
 
 def similar_indices(freqs, df_thresh, nextfs=0):
-    """ Indices of similar frequencies.
+    """Indices of similar frequencies.
 
     If two frequencies from different elements in the inner lists of `freqs` are
     reciprocally the closest to each other and closer than `df_thresh`,
     then two indices (element, frequency) of the respective other frequency
     are appended.
 
     Parameters
@@ -1184,15 +1191,15 @@
         indices = []
         for groups in freqs:
             indices.append(similar_indices(groups, df_thresh, nextfs))
     return indices
 
 
 def unique_mask(freqs, df_thresh, nextfs=0):
-    """ Mark similar frequencies from different recordings as dublicate.
+    """Mark similar frequencies from different recordings as dublicate.
 
     If two frequencies from different elements in `freqs` are
     reciprocally the closest to each other and closer than `df_thresh`,
     then the one with the smaller power is marked for removal.
 
     Parameters
     ----------
@@ -1242,15 +1249,15 @@
                             mask[j][m] = False
                     else:
                         mask[j][m] = False
     return mask
 
 
 def unique(freqs, df_thresh, mode='power', nextfs=0):
-    """ Remove similar frequencies from different recordings.
+    """Remove similar frequencies from different recordings.
 
     If two frequencies from different elements in the inner lists of `freqs`
     are reciprocally the closest to each other and closer than `df_thresh`,
     then the one with the smaller power is removed. As power, either the
     absolute power as provided in the second column of the data elements
     in `freqs` is taken (mode=='power'), or the relative power
     (mode='relpower'), or the power rank (mode='rank').
@@ -1308,16 +1315,15 @@
         unique_freqs = []
         for groups in freqs:
             unique_freqs.append(unique(groups, df_thresh, mode, nextfs))
     return unique_freqs
 
 
 def colors_markers():
-    """
-    Generate a list of colors and markers for plotting.
+    """Generate a list of colors and markers for plotting.
 
     Returns
     -------
     colors: list
         list of colors
     markers: list
         list of markers
@@ -1354,66 +1360,68 @@
     markers.extend(len(cc2) * 'D')
     mr2.extend(len(cc2) * 'x')
     markers.extend(mr2)
     return colors, markers
 
 
 def plot_harmonic_groups(ax, group_list, indices=None, max_groups=0,
-                         sort_by_freq=True, label_power=False,
+                         skip_bad=False, sort_by_freq=True, label_power=False,
                          colors=None, markers=None, legend_rows=8, **kwargs):
-    """
-    Mark decibel power of fundamentals and their harmonics in a plot.
+    """Mark decibel power of fundamentals and their harmonics in a plot.
 
     Parameters
     ----------
     ax: axis for plot
         Axis used for plotting.
     group_list: list of 2-D arrays
         Lists of harmonic groups as returned by extract_fundamentals() and
         harmonic_groups() with the element [0, 0] of the harmonic groups being
         the fundamental frequency, and element[0, 1] being the corresponding power.
     indices: list of int or None
         If smaller than zero then set the legend label of the corresponding group in brackets.
     max_groups: int
-            If not zero plot only the max_groups most powerful groups.
+        If not zero plot only the max_groups most powerful groups.
+    skip_bad: bool
+        Skip harmonic groups without index (entry in indices is negative).
     sort_by_freq: boolean
-            If True sort legend by frequency, otherwise by power.
+        If True sort legend by frequency, otherwise by power.
     label_power: boolean
         If `True` put the power in decibel in addition to the frequency into the legend.
     colors: list of colors or None
-            If not None list of colors for plotting each group
+        If not None list of colors for plotting each group
     markers: list of markers or None
-            If not None list of markers for plotting each group
+        If not None list of markers for plotting each group
     legend_rows: int
-            Maximum number of rows to be used for the legend.
+        Maximum number of rows to be used for the legend.
     kwargs: 
-            Key word arguments for the legend of the plot.
+        Key word arguments for the legend of the plot.
     """
-
     if len(group_list) == 0:
         return
     
     # sort by power:
     powers = np.array([np.sum(group[:,1]) for group in group_list])
     max_power = np.max(powers)
-    power_idx = np.argsort(powers)
-    if max_groups > 0 and len(power_idx > max_groups):
-        power_idx = power_idx[-max_groups:]
-    idx = np.array(list(reversed(power_idx)))
+    idx = np.argsort(-powers)
+    if max_groups > 0 and len(idx > max_groups):
+        idx = idx[:max_groups]
 
     # sort by frequency:
     if sort_by_freq:
-        freqs = [group_list[group][0, 0] for group in idx]
+        freqs = np.array([group_list[group][0,0] for group in idx])
         if legend_rows > 0 and legend_rows < len(freqs):
-            idx[:legend_rows] = idx[np.argsort(freqs[:legend_rows])]
+            idx = idx[np.argsort(freqs[:legend_rows])]
         else:
             idx = idx[np.argsort(freqs)]
 
     # plot:
-    for k, i in enumerate(idx):
+    k = 0
+    for i in idx:
+        if indices is not None and skip_bad and indices[i] < 0:
+            continue
         group = group_list[i]
         x = group[:,0]
         y = decibel(group[:,1])
         msize = 7.0 + 10.0*(powers[i]/max_power)**0.25
         color_kwargs = {}
         if colors is not None:
             color_kwargs = {'color': colors[k%len(colors)]}
@@ -1430,14 +1438,15 @@
         if markers is None:
             ax.plot(x, y, 'o', ms=msize, label=label, **color_kwargs)
         else:
             if k >= len(markers):
                 break
             ax.plot(x, y, linestyle='None', marker=markers[k],
                     mec=None, mew=0.0, ms=msize, label=label, **color_kwargs)
+        k += 1
 
     # legend:
     if legend_rows > 0:
         if legend_rows > 5:
             ncol = 1
         else:
             ncol = (len(idx)-1) // legend_rows + 1
@@ -1445,16 +1454,16 @@
     else:
         ax.legend(numpoints=1, **kwargs)
 
 
 def plot_psd_harmonic_groups(ax, psd_freqs, psd, group_list,
                              mains=None, all_freqs=None, good_freqs=None,
                              log_freq=False, min_freq=0.0, max_freq=2000.0, ymarg=0.0):
-    """
-    Plot decibel power-spectrum with detected peaks, harmonic groups, and mains frequencies.
+    """Plot decibel power-spectrum with detected peaks, harmonic groups,
+    and mains frequencies.
     
     Parameters
     ----------
     psd_freqs: array
         Frequencies of the power spectrum.
     psd: array
         Power spectrum (linear, not decible).
@@ -1504,37 +1513,37 @@
     plot_decibel_psd(ax, psd_freqs, psd, log_freq=log_freq, min_freq=min_freq,
                      max_freq=max_freq, ymarg=ymarg, color='blue')
 
     
 def add_psd_peak_detection_config(cfg, low_threshold=0.0, high_threshold=0.0,
                                   thresh_bins=100,
                                   low_thresh_factor=6.0, high_thresh_factor=10.0):
-    """ Add parameter needed for detection of peaks in power spectrum used by
-    harmonic_groups() as a new section to a configuration.
+    """Add parameter needed for detection of peaks in power spectrum used
+    by harmonic_groups() as a new section to a configuration.
 
     Parameters
     ----------
     cfg: ConfigFile
         The configuration.
     """
-
     cfg.add_section('Thresholds for peak detection in power spectra:')
     cfg.add('lowThreshold', low_threshold, 'dB', 'Threshold for all peaks.\n If 0.0 estimate threshold from histogram.')
     cfg.add('highThreshold', high_threshold, 'dB', 'Threshold for good peaks. If 0.0 estimate threshold from histogram.')
     
     cfg.add_section('Threshold estimation:\nIf no thresholds are specified they are estimated from the histogram of the decibel power spectrum.')
     cfg.add('thresholdBins', thresh_bins, '', 'Number of bins used to compute the histogram used for threshold estimation.')
     cfg.add('lowThresholdFactor', low_thresh_factor, '', 'Factor for multiplying standard deviation of noise floor for lower threshold.')
     cfg.add('highThresholdFactor', high_thresh_factor, '', 'Factor for multiplying standard deviation of noise floor for higher threshold.')
 
 
 def psd_peak_detection_args(cfg):
-    """ Translates a configuration to the respective parameter names for the
-    detection of peaks in power spectrum used by harmonic_groups().
-    The return value can then be passed as key-word arguments to this function.
+    """Translates a configuration to the respective parameter names for
+    the detection of peaks in power spectrum used by
+    harmonic_groups().  The return value can then be passed as
+    key-word arguments to this function.
 
     Parameters
     ----------
     cfg: ConfigFile
         The configuration.
 
     Returns
@@ -1551,23 +1560,22 @@
 
 
 def add_harmonic_groups_config(cfg, mains_freq=60.0, mains_freq_tol=1.0,
                                max_divisor=4, freq_tol_fac=1.0,
                                max_freq_tol=1.0, min_group_size=3,
                                min_freq=20.0, max_freq=2000.0, max_db_diff=20.0,
                                max_harmonics_db=-5.0, max_harmonics=0, max_groups=0):
-    """ Add parameter needed for detection of harmonic groups as
-    a new section to a configuration.
+    """Add parameter needed for detection of harmonic groups as a new
+    section to a configuration.
 
     Parameters
     ----------
     cfg: ConfigFile
         The configuration.
     """
-    
     cfg.add_section('Harmonic groups:')
     cfg.add('mainsFreq', mains_freq, 'Hz', 'Mains frequency to be excluded.')
     cfg.add('mainsFreqTolerance', mains_freq_tol, 'Hz', 'Exclude peaks within this tolerance around multiples of the mains frequency.')
     cfg.add('minimumGroupSize', min_group_size, '',
 'Minimum number of harmonics (inclusively fundamental) that make up a harmonic group.')
     cfg.add('maxDivisor', max_divisor, '', 'Maximum ratio between the frequency of the largest peak and its fundamental.')
     cfg.add('freqTolerance', freq_tol_fac, '',
@@ -1581,17 +1589,17 @@
     cfg.add('maximumPowerDifference', max_db_diff, 'dB', 'If larger than zero, maximum standard deviation allowed for difference in logarithmic power between successive harmonics. Smaller values enforce smoother spectra.')
     cfg.add('maximumHarmonicsPower', max_harmonics_db, 'dB', 'Maximum allowed power of the minimumGroupSize-th and higher harmonics relative to peak power.')
     cfg.add('maximumHarmonics', max_harmonics, '', '0: keep all, >0 only keep the first # harmonics.')
     cfg.add('maximumGroups', max_groups, '', 'Maximum number of harmonic groups. If 0 process all.')
 
 
 def harmonic_groups_args(cfg):
-    """ Translates a configuration to the
-    respective parameter names of the harmonic-group detection functions.
-    The return value can then be passed as key-word arguments to this function.
+    """Translates a configuration to the respective parameter names of
+    the harmonic-group detection functions.  The return value can then
+    be passed as key-word arguments to this function.
 
     Parameters
     ----------
     cfg: ConfigFile
         The configuration.
 
     Returns
@@ -1610,46 +1618,51 @@
                     'max_freq': 'maximumFrequency',
                     'max_db_diff': 'maximumPowerDifference',
                     'max_harmonics_db': 'maximumHarmonicsPower',                     
                     'max_harmonics': 'maximumHarmonics',
                     'max_groups': 'maximumGroups'})
 
 
-if __name__ == "__main__":
-    import sys
+def main(data_file=None):
     import matplotlib.pyplot as plt
+    from thunderlab.powerspectrum import psd
     from .fakefish import wavefish_eods
-    from .powerspectrum import psd
 
-    if len(sys.argv) < 2:
+    if data_file is None:
         # generate data:
         title = 'simulation'
         samplerate = 44100.0
+        d = 20.0
+        noise = 0.01
         eodfs = [123.0, 333.0, 666.0, 666.5]
-        fish1 = 0.5*wavefish_eods('Eigenmannia', eodfs[0], samplerate, duration=8.0, noise_std=0.01)
-        fish2 = 1.0*wavefish_eods('Eigenmannia', eodfs[1], samplerate, duration=8.0, noise_std=0.01)
-        fish3 = 10.0*wavefish_eods('Alepto', eodfs[2], samplerate, duration=8.0, noise_std=0.01)
-        fish4 = 6.0*wavefish_eods('Alepto', eodfs[3], samplerate, duration=8.0, noise_std=0.01)
+        fish1 = 0.5*wavefish_eods('Eigenmannia', eodfs[0], samplerate,
+                                  duration=d, noise_std=noise)
+        fish2 = 1.0*wavefish_eods('Eigenmannia', eodfs[1], samplerate,
+                                  duration=d, noise_std=noise)
+        fish3 = 10.0*wavefish_eods('Alepto', eodfs[2], samplerate,
+                                   duration=d, noise_std=noise)
+        fish4 = 6.0*wavefish_eods('Alepto', eodfs[3], samplerate,
+                                  duration=d, noise_std=noise)
         data = fish1 + fish2 + fish3 + fish4
     else:
-        from .dataloader import load_data
-        print("load %s ..." % sys.argv[1])
-        data, samplerate, unit = load_data(sys.argv[1], 0)
-        title = sys.argv[1]
+        from thunderlab.dataloader import load_data
+        print("load %s ..." % data_file)
+        data, samplerate, unit, amax = load_data(data_file)
+        data = data[:,0]
+        title = data_file
 
     # retrieve fundamentals from power spectrum:
-    psd_data = psd(data, samplerate, freq_resolution=0.5)
-    groups, _, mains, all_freqs, good_freqs, _, _, _ = harmonic_groups(psd_data[0], psd_data[1], verbose=0, check_freqs=[123.0, 666.0])
-    fig = plt.figure()
-    ax = fig.add_subplot(1, 1, 1)
+    psd_data = psd(data, samplerate, freq_resolution=0.1)
+    groups, _, mains, all_freqs, good_freqs, _, _, _ = harmonic_groups(psd_data[0], psd_data[1], check_freqs=[123.0, 666.0], max_db_diff=30.0, verbose=0)
+    fig, ax = plt.subplots()
     plot_psd_harmonic_groups(ax, psd_data[0], psd_data[1], groups, mains,
                              all_freqs, good_freqs, max_freq=3000.0)
     ax.set_title(title)
     plt.show()
-    #exit()
+    
     # unify fundamental frequencies:
     fundamentals = fundamental_freqs(groups)
     np.set_printoptions(formatter={'float': lambda x: '%5.1f' % x})
     print('fundamental frequencies extracted from power spectrum:')
     print(fundamentals)
     print('')
     freqs = fundamental_freqs_and_power([groups])
@@ -1673,10 +1686,17 @@
     print('\n'.join(( str(f) for f in unique_freqs)))
     print('')
     unique_freqs = unique(freqs, 1.0, 'rank')
     print('unique rank:')
     print('\n'.join(( str(f) for f in unique_freqs)))
     print('')
     unique_freqs = unique(freqs, 1.0, 'rank', 1)
-    print('unique rank for next neighor only:')
+    print('unique rank for next neighour only:')
     print('\n'.join(( str(f) for f in unique_freqs)))
     print('')
+
+    
+if __name__ == "__main__":
+    import sys
+    data_file = sys.argv[1] if len(sys.argv) > 1 else None
+    main(data_file)
+
```

### Comparing `thunderfish-1.9.9/thunderfish/pulseplots.py` & `thunderfish-2.0.0/src/thunderfish/pulseplots.py`

 * *Files identical despite different names*

### Comparing `thunderfish-1.9.9/thunderfish/pulses.py` & `thunderfish-2.0.0/src/thunderfish/pulses.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from scipy import stats
 from scipy.interpolate import interp1d
 from sklearn.preprocessing import StandardScaler
 from sklearn.decomposition import PCA
 from sklearn.cluster import DBSCAN
 from sklearn.mixture import BayesianGaussianMixture
 from sklearn.metrics import pairwise_distances
-from .eventdetection import detect_peaks, median_std_threshold
+from thunderlab.eventdetection import detect_peaks, median_std_threshold
 from .pulseplots import *
 
 import warnings
 def warn(*args, **kwargs):
     """
     Ignore all warnings.
     """
@@ -58,26 +58,27 @@
         Number of instances for each unique value in ar.
     """
     try:
         return np.unique(ar, return_counts=True)
     except TypeError:
         ar = np.asanyarray(ar).flatten()
         ar.sort()
-        mask = np.empty(ar.shape, dtype=np.bool_)
+        mask = np.empty(ar.shape, dtype=bool_)
         mask[:1] = True
         mask[1:] = ar[1:] != ar[:-1]
         idx = np.concatenate(np.nonzero(mask) + ([mask.size],))
         return ar[mask], np.diff(idx)  
 
 
-###################################################################################
+###########################################################################
 
 
-def extract_pulsefish(data, samplerate, width_factor_shape=3, width_factor_wave=8,
-                      width_factor_display=4, verbose=0, plot_level=0, save_plots=False,
+def extract_pulsefish(data, samplerate, width_factor_shape=3,
+                      width_factor_wave=8, width_factor_display=4,
+                      verbose=0, plot_level=0, save_plots=False,
                       save_path='', ftype='png', return_data=[]):
     """ Extract and cluster pulse-type fish EODs from single channel data.
     
     Takes recording data containing an unknown number of pulsefish and extracts the mean 
     EOD and EOD timepoints for each fish present in the recording.
     
     Parameters
@@ -324,29 +325,48 @@
         i_data = data
     log_dict['data'] = i_data               # TODO: could be removed
     log_dict['samplerate'] = i_samplerate   # TODO: could be removed
     log_dict['i_data'] = i_data
     log_dict['i_samplerate'] = i_samplerate
     # log_dict["interp_fac"] = interp_fac  # TODO: is not set anymore
                                          
+    # standard deviation of data in small snippets:
+    threshold = median_std_threshold(data, samplerate)  # TODO make this a parameter
     
     # extract peaks:
-    x_peak, x_trough, eod_heights, eod_widths, pd_log_dict = \
-      detect_pulse_candidates(i_data, i_samplerate,
-                              np.max([width_factor_shape, width_factor_display, width_factor_wave]),
-                              verbose=verbose-1, return_data=return_data)
+    if 'peak_detection' in return_data:
+        x_peak, x_trough, eod_heights, eod_widths, pd_log_dict = \
+            detect_pulses(i_data, i_samplerate, threshold,
+                          width_fac=np.max([width_factor_shape,
+                                            width_factor_display,
+                                            width_factor_wave]),
+                          verbose=verbose-1, return_data=True)
+        log_dict.update(pd_log_dict)
+    else:
+        x_peak, x_trough, eod_heights, eod_widths = \
+            detect_pulses(i_data, i_samplerate, threshold,
+                          width_fac=np.max([width_factor_shape,
+                                            width_factor_display,
+                                            width_factor_wave]),
+                          verbose=verbose-1, return_data=False)
     
     if len(x_peak) > 0:
         # cluster
-        clusters, x_merge, c_log_dict = cluster(x_peak, x_trough, eod_heights, eod_widths,
-                                                i_data, i_samplerate,
-                                                width_factor_shape, width_factor_wave,
-                                                verbose=verbose-1, plot_level=plot_level-1,
-                                                save_plots=save_plots, save_path=save_path,
-                                                ftype=ftype, return_data=return_data) 
+        clusters, x_merge, c_log_dict = cluster(x_peak, x_trough,
+                                                eod_heights,
+                                                eod_widths, i_data,
+                                                i_samplerate,
+                                                width_factor_shape,
+                                                width_factor_wave,
+                                                verbose=verbose-1,
+                                                plot_level=plot_level-1,
+                                                save_plots=save_plots,
+                                                save_path=save_path,
+                                                ftype=ftype,
+                                                return_data=return_data) 
 
         # extract mean eods and times
         mean_eods, eod_times, eod_peaktimes, eod_troughtimes, cluster_labels = \
           extract_means(i_data, x_merge, x_peak, x_trough, eod_widths, clusters,
                         i_samplerate, width_factor_display, verbose=verbose-1)
 
         # determine clipped clusters (save them, but ignore in other steps)
@@ -385,143 +405,171 @@
         if save_plots:
             plt.close('all')
     
         if 'all_eod_times' in return_data:
             log_dict['all_times'] = [x_peak/i_samplerate, x_trough/i_samplerate]
             log_dict['eod_troughtimes'] = eod_troughtimes
         
-        log_dict.update(pd_log_dict)
         log_dict.update(c_log_dict)
 
     return mean_eods, eod_times, eod_peaktimes, zoom_window, log_dict
 
 
-def detect_pulse_candidates(data, samplerate, width_factor,
-                            min_peakwidth=0.00005, max_peakwidth=0.01,
-                            verbose=0, return_data=[]):
-    """ Detect potential pulse EODs in data.
-
-    Was `def extract_eod_times(data, samplerate, width_factor, interp_freq=500000,
-                      max_peakwidth=0.01, min_peakwidth=None, verbose=0,
-                      return_data=[], save_path='')` before.
+def detect_pulses(data, samplerate, thresh, min_rel_slope_diff=0.25,
+                  min_width=0.00005, max_width=0.01, width_fac=5.0,
+                  verbose=0, return_data=False):
+    """Detect pulses in data.
+
+    Was `def extract_eod_times(data, samplerate, width_factor,
+                      interp_freq=500000, max_peakwidth=0.01,
+                      min_peakwidth=None, verbose=0, return_data=[],
+                      save_path='')` before.
 
     Parameters
     ----------
     data: 1-D array of float
         The data to be analysed.
     samplerate: float
-        Sampling rate of the data
-    width_factor: float
-        Factor for extracting EOD shapes.
-        Only EODs are extracted that can fully be analysed with this width.
-
-    min_peakwidth: float (optional)
-        Minimum width for peak detection in seconds.
-    max_peakwidth: float (optional)
-        Maximum width for peak detection in seconds.
-
+        Sampling rate of the data.
+    thresh: float
+        Threshold for peak and trough detection via `detect_peaks()`.
+        Must be a positive number that sets the minimum difference
+        between a peak and a trough.
+    min_rel_slope_diff: float
+        Minimum required difference between left and right slope (between
+        peak and troughs) relative to mean slope for deciding which trough
+        to take besed on slope difference.
+    min_width: float
+        Minimum width (peak-trough distance) of pulses in seconds.
+    max_width: float
+        Maximum width (peak-trough distance) of pulses in seconds.
+    width_fac: float
+        Pulses extend plus or minus `width_fac` times their width
+        (distance between peak and assigned trough).
+        Only pulses are returned that can fully be analysed with this width.
     verbose : int (optional)
         Verbosity level.
-    return_data : list of strings (optional)
-        Keys that specify data to be logged. If 'peak_detection' is in `return_data`, 
-        data of this function is logged (see extract_pulsefish()).
+    return_data : bool
+        If `True` data of this function is logged and returned (see
+        extract_pulsefish()).
 
     Returns
     -------
-    x_peak: array of ints
+    peak_indices: array of ints
         Indices of EOD peaks in data.
-    x_trough: array of ints
+    trough_indices: array of ints
         Indices of EOD troughs in data. There is one x_trough for each x_peak.
-    eod_heights: array of floats
+    heights: array of floats
         EOD heights for each x_peak.
-    eod_widths: array of ints
+    widths: array of ints
         EOD widths for each x_peak (in samples).
     peak_detection_result : dictionary
-        Key value pairs of logged data. Data to be logged is specified by return_data.
+        Key value pairs of logged data.
+        This is only returned if `return_data` is `True`.
 
     """
     peak_detection_result = {}
-    
-    # standard deviation of data in small snippets:
-    threshold = median_std_threshold(data, samplerate)  # TODO make this a parameter
 
     # detect peaks and troughs in the data:
-    peak_indices, trough_indices = detect_peaks(data, threshold)
+    peak_indices, trough_indices = detect_peaks(data, thresh)
     if verbose > 0:
         print('Peaks/troughs detected in data:                      %5d %5d'
               % (len(peak_indices), len(trough_indices)))
-    if 'peak_detection' in return_data:
+    if return_data:
         peak_detection_result.update(peaks_1=np.array(peak_indices),
                                      troughs_1=np.array(trough_indices))
-    if len(peak_indices)<2 or \
-       len(trough_indices)<2 or \
+    if len(peak_indices) < 2 or \
+       len(trough_indices) < 2 or \
        len(peak_indices) > len(data)/20:
+        # TODO: if too many peaks increase threshold!
         if verbose > 0:
             print('No or too many peaks/troughs detected in data.')
-        return np.array([]), np.array([]), np.array([]), np.array([]), \
-            peak_detection_result
+        if return_data:
+            return np.array([], dtype=int), np.array([], dtype=int), \
+                np.array([]), np.array([], dtype=int), peak_detection_result
+        else:
+            return np.array([], dtype=int), np.array([], dtype=int), \
+                np.array([]), np.array([], dtype=int)
 
     # assign troughs to peaks:
-    peak_indices, trough_indices, heights, widths = \
-      assign_side_peaks(data, peak_indices, trough_indices, 0.25)
-    # TODO: make 0.25 a parameter
+    peak_indices, trough_indices, heights, widths, slopes = \
+      assign_side_peaks(data, peak_indices, trough_indices, min_rel_slope_diff)
     if verbose > 1:
         print('Number of peaks after assigning side-peaks:          %5d'
               % (len(peak_indices)))
-    if 'peak_detection' in return_data:
+    if return_data:
         peak_detection_result.update(peaks_2=np.array(peak_indices),
                                      troughs_2=np.array(trough_indices))
 
     # check widths:
-    keep_events = ((widths>min_peakwidth*samplerate) &
-                   (widths<max_peakwidth*samplerate))
-    peak_indices = peak_indices[keep_events]
-    trough_indices = trough_indices[keep_events]
-    heights = heights[keep_events]
-    widths = widths[keep_events]
+    keep = ((widths>min_width*samplerate) & (widths<max_width*samplerate))
+    peak_indices = peak_indices[keep]
+    trough_indices = trough_indices[keep]
+    heights = heights[keep]
+    widths = widths[keep]
+    slopes = slopes[keep]
     if verbose > 1:
         print('Number of peaks after checking pulse width:          %5d'
               % (len(peak_indices)))
-    if 'peak_detection' in return_data:
+    if return_data:
         peak_detection_result.update(peaks_3=np.array(peak_indices),
                                      troughs_3=np.array(trough_indices))
 
-    """"
-    # merge connected peaks:
-    peak_indices, trough_indices, heights, widths = \
-      discard_connecting_eods(peak_indices, trough_indices, heights, widths)
+    # discard connected peaks:
+    same = np.nonzero(trough_indices[:-1] == trough_indices[1:])[0]
+    keep = np.ones(len(trough_indices), dtype=bool)
+    for i in same:
+        # same troughs at trough_indices[i] and trough_indices[i+1]:
+        s = slopes[i:i+2]
+        rel_slopes = np.abs(np.diff(s))[0]/np.mean(s)
+        if rel_slopes > min_rel_slope_diff:
+            keep[i+(s[1]<s[0])] = False
+        else:
+            keep[i+(heights[i+1]<heights[i])] = False
+    peak_indices = peak_indices[keep]
+    trough_indices = trough_indices[keep]
+    heights = heights[keep]
+    widths = widths[keep]
     if verbose > 1:
         print('Number of peaks after merging pulses:                %5d'
               % (len(peak_indices)))
-    if 'peak_detection' in return_data:
+    if return_data:
         peak_detection_result.update(peaks_4=np.array(peak_indices),
                                      troughs_4=np.array(trough_indices))
     if len(peak_indices) == 0:
         if verbose > 0:
             print('No peaks remain as pulse candidates.')
-        return np.array([]), np.array([]), np.array([]), np.array([]), \
-            peak_detection_result
-    """
+        if return_data:
+            return np.array([], dtype=int), np.array([], dtype=int), \
+                np.array([]), np.array([], dtype=int), peak_detection_result
+        else:
+            return np.array([], dtype=int), np.array([], dtype=int), \
+                np.array([]), np.array([], dtype=int)
     
     # only take those where the maximum cutwidth does not cause issues -
-    # if the width_factor times the width + x is more than length.
-    max_width = np.max(widths)*width_factor
-    cut_idx = ((peak_indices - max_width > 0) &
-               (peak_indices + max_width < len(data)) &
-               (trough_indices - max_width > 0) &
-               (trough_indices + max_width < len(data)))
+    # if the width_fac times the width + x is more than length.
+    keep = ((peak_indices - widths > 0) &
+            (peak_indices + widths < len(data)) &
+            (trough_indices - widths > 0) &
+            (trough_indices + widths < len(data)))
 
     if verbose > 0:
         print('Remaining peaks after EOD extraction:                %5d'
-              % (p.sum(cut_idx)))
+              % (p.sum(keep)))
         print('')
 
-    return peak_indices[cut_idx], trough_indices[cut_idx], heights[cut_idx], widths[cut_idx], peak_detection_result
+    if return_data:
+        return peak_indices[keep], trough_indices[keep], \
+            heights[keep], widths[keep], peak_detection_result
+    else:
+        return peak_indices[keep], trough_indices[keep], \
+            heights[keep], widths[keep]
 
 
+@jit(nopython=True)
 def assign_side_peaks(data, peak_indices, trough_indices,
                       min_rel_slope_diff=0.25):
     """Assign to each peak the trough resulting in a pulse with the steepest slope or largest height.
 
     The slope between a peak and a trough is computed as the height
     difference divided by the distance between peak and trough. If the
     slopes between the left and the right trough differ by less than
@@ -551,21 +599,23 @@
     trough_indices: array of ints
         Corresponding trough indices of trough to the left or right
         of the peaks.
     heights: array of floats
         Peak heights (distance between peak and corresponding trough amplitude)
     widths: array of ints
         Peak widths (distance between peak and corresponding trough indices)
-
+    slopes: array of floats
+        Peak slope (height divided by width)
     """
     # is a main or side peak first?
     peak_first = int(peak_indices[0] < trough_indices[0])
     # is a main or side peak last?
     peak_last = int(peak_indices[-1] > trough_indices[-1])
-    # ensure main peaks to have side peaks at both sides:
+    # ensure all peaks to have side peaks (troughs) at both sides,
+    # i.e. troughs at same index and next index are before and after peak:
     peak_indices = peak_indices[peak_first:len(peak_indices)-peak_last]
     y = data[peak_indices]
     
     # indices of troughs on the left and right side of main peaks:
     l_indices = np.arange(len(peak_indices))
     r_indices = l_indices + 1
 
@@ -579,79 +629,30 @@
     r_side_indices = trough_indices[r_indices]
     r_distance = np.abs(r_side_indices - peak_indices)
     r_height = np.abs(y - data[r_side_indices])
     r_slope = np.abs(r_height/r_distance)
 
     # which trough to assign to the peak?
     # - either the one with the steepest slope, or
-    # - when slopes are similar on both sides (within 25% difference),
+    # - when slopes are similar on both sides
+    #   (within `min_rel_slope_diff` difference),
     #   the trough with the maximum height difference to the peak:
     rel_slopes = np.abs(l_slope-r_slope)/(0.5*(l_slope+r_slope))
     take_slopes = rel_slopes > min_rel_slope_diff
     take_left = l_height > r_height
     take_left[take_slopes] = l_slope[take_slopes] > r_slope[take_slopes]
 
-    # assign troughs, heights, and widths:
+    # assign troughs, heights, widths, and slopes:
     trough_indices = np.where(take_left,
                               trough_indices[:-1], trough_indices[1:])
     heights = np.where(take_left, l_height, r_height)
     widths = np.where(take_left, l_distance, r_distance)
     slopes = np.where(take_left, l_slope, r_slope)
 
-    ## TODO: check for width here?
-    
-    # discard connected peaks:
-    same = np.nonzero(trough_indices[:-1] == trough_indices[1:])[0]
-    keep = np.ones(len(trough_indices), dtype=np.bool)
-    for i in same:
-        # same troughs at trough_indices[i] and trough_indices[i+1]:
-        s = slopes[i:i+2]
-        rel_slopes = np.abs(np.diff(s))[0]/np.mean(s)
-        if rel_slopes > min_rel_slope_diff:
-            keep[i+(s[1]<s[0])] = False
-        else:
-            keep[i+(heights[i+1]<heights[i])] = False
-    
-    return peak_indices[keep], trough_indices[keep], heights[keep], widths[keep]
-
-
-@jit(nopython=True)
-def discard_connecting_eods(x_peak, x_trough, heights, widths):
-    """If two detected EODs share the same closest trough, keep only the
-highest peak.
-
-    Parameters
-    ----------
-    x_peak: list of ints
-        Indices of EOD peaks.
-    x_trough: list of ints
-        Indices of EOD troughs.
-    heights: list of floats
-        EOD heights.
-    widths: list of ints
-        EOD widths.
-
-    Returns
-    -------
-    x_peak, x_trough, heights, widths : lists of ints and floats
-        EOD location and features of the non-discarded EODs
-    """
-    keep_idxs = np.ones(len(x_peak))
-
-    for tr in np.unique(x_trough):
-        if len(x_trough[x_trough==tr]) > 1:
-            slopes = heights[x_trough==tr]/widths[x_trough==tr]
-
-            if (np.max(slopes)!=np.min(slopes)) and \
-              (np.abs(np.max(slopes)-np.min(slopes))/(0.5*np.max(slopes)+0.5*np.min(slopes)) > 0.25):
-                keep_idxs[np.where(x_trough==tr)[0][np.argmin(heights[x_trough==tr]/widths[x_trough==tr])]] = 0
-            else:
-                keep_idxs[np.where(x_trough==tr)[0][np.argmin(heights[x_trough==tr])]] = 0
-            
-    return x_peak[np.where(keep_idxs==1)[0]], x_trough[np.where(keep_idxs==1)[0]], heights[np.where(keep_idxs==1)[0]], widths[np.where(keep_idxs==1)[0]]
+    return peak_indices, trough_indices, heights, widths, slopes
 
 
 def cluster(eod_xp, eod_xt, eod_heights, eod_widths, data, samplerate,
             width_factor_shape, width_factor_wave,
             n_gaus_height=10, merge_threshold_height=0.1, n_gaus_width=3,
             merge_threshold_width=0.5, minp=10,
             verbose=0, plot_level=0, save_plots=False, save_path='', ftype='pdf',
@@ -729,20 +730,20 @@
         all_heightlabels = []
         all_shapelabels = []
         all_snippets = []
         all_features = []
         all_heights = []
         all_unique_heightlabels = []
 
-    all_p_clusters = np.ones(len(eod_xp))*-1
-    all_t_clusters = np.ones(len(eod_xp))*-1
+    all_p_clusters = -1 * np.ones(len(eod_xp))
+    all_t_clusters = -1 * np.ones(len(eod_xp))
     artefact_masks_p = np.ones(len(eod_xp), dtype=bool)
     artefact_masks_t = np.ones(len(eod_xp), dtype=bool)
 
-    x_merge = np.ones(len(eod_xp))*-1
+    x_merge = -1 * np.ones(len(eod_xp))
 
     max_label_p = 0   # keep track of the labels so that no labels are overwritten
     max_label_t = 0
 
     # loop only over height clusters that are bigger than minp
     # first cluster on width
     width_labels, bgm_log_dict = BGM(1000*eod_widths/samplerate, merge_threshold_width,
@@ -763,25 +764,33 @@
     for wi, width_label in enumerate(unique_width_labels):
 
         # select only features in one width cluster at a time
         w_eod_widths = eod_widths[width_labels==width_label]
         w_eod_heights = eod_heights[width_labels==width_label]
         w_eod_xp = eod_xp[width_labels==width_label]
         w_eod_xt = eod_xt[width_labels==width_label]
-        wp_clusters = np.ones(len(w_eod_xp))*-1
-        wt_clusters = np.ones(len(w_eod_xp))*-1
+        width = int(width_factor_shape*np.median(w_eod_widths))
+        if width > w_eod_xp[0]:
+            width = w_eod_xp[0]
+        if width > w_eod_xt[0]:
+            width = w_eod_xt[0]
+        if width > len(data) - w_eod_xp[-1]:
+            width = len(data) - w_eod_xp[-1]
+        if width > len(data) - w_eod_xt[-1]:
+            width = len(data) - w_eod_xt[-1]
+        
+        wp_clusters = -1 * np.ones(len(w_eod_xp))
+        wt_clusters = -1 * np.ones(len(w_eod_xp))
         wartefact_mask = np.ones(len(w_eod_xp))
 
         # determine height labels
         raw_p_snippets, p_snippets, p_features, p_bg_ratio = \
-          extract_snippet_features(data, w_eod_xp, w_eod_widths, w_eod_heights,
-                                   width_factor_shape)
+          extract_snippet_features(data, w_eod_xp, w_eod_heights, width)
         raw_t_snippets, t_snippets, t_features, t_bg_ratio = \
-          extract_snippet_features(data, w_eod_xt, w_eod_widths, w_eod_heights,
-                                   width_factor_shape)
+          extract_snippet_features(data, w_eod_xt, w_eod_heights, width)
 
         height_labels, bgm_log_dict = \
           BGM(w_eod_heights,
               min(merge_threshold_height, np.median(np.min(np.vstack([p_bg_ratio, t_bg_ratio]), axis=0))),
               n_gaus_height, use_log=True, verbose=verbose-1, plot_level=plot_level-1,
               xlabel = 'height [a.u.]', save_plot=save_plots, save_path=save_path,
               save_name = 'height_%d' % wi, ftype=ftype, return_data=return_data)
@@ -1022,15 +1031,15 @@
     bgm_dict : dictionary
         Key value pairs of logged data. Data to be logged is specified by return_data.
     """
 
     bgm_dict = {}
 
     if len(np.unique(x)) > n_gaus:
-        BGM_model = BayesianGaussianMixture(n_gaus, max_iter=max_iter, n_init=n_init)
+        BGM_model = BayesianGaussianMixture(n_components=n_gaus, max_iter=max_iter, n_init=n_init)
         if use_log:
             labels = BGM_model.fit_predict(stats.zscore(np.log(x)).reshape(-1, 1))
         else:
             labels = BGM_model.fit_predict(stats.zscore(x).reshape(-1, 1))
     else:
         return np.zeros(len(x)), bgm_dict
     
@@ -1117,29 +1126,27 @@
     # apply mapping
     for map_key, map_value in mapping.items():
         labels[labels==map_key] = map_value
 
     return labels
 
 
-def extract_snippet_features(data, eod_x, eod_widths, eod_heights, width_factor, n_pc=5):
+def extract_snippet_features(data, eod_x, eod_heights, width, n_pc=5):
     """ Extract snippets from recording data, normalize them, and perform PCA.
 
     Parameters
     ----------
     data : 1D numpy array of floats
         Recording data.
     eod_x : 1D array of ints
         Locations of EODs as indices.
-    eod_widths : 1D array of ints
-        EOD widths in samples.
     eod_heights: 1D array of floats
         EOD heights.
-    width_factor: float
-        Multiplier for extracting EOD snippets        
+    width : int
+        Width to cut out to each side in samples.
 
     n_pc : int (optional)
         Number of PCs to use for PCA.
 
     Returns
     -------
     raw_snippets : 2D numpy array (N, EOD_width)
@@ -1147,18 +1154,16 @@
     snippets : 2D numpy array (N, EOD_width)
         Normalized EOD snippets
     features : 2D numpy array (N,n_pc)
         PC values of EOD snippets
     bg_ratio : 1D numpy array (N)
         Ratio of the background activity slopes compared to EOD height.
     """
-
     # extract snippets with corresponding width
-    width = width_factor*np.median(eod_widths)
-    raw_snippets = np.vstack([data[int(x-width):int(x+width)] for x in eod_x])
+    raw_snippets = np.vstack([data[x-width:x+width] for x in eod_x])
 
     # subtract the slope and normalize the snippets
     snippets, bg_ratio = subtract_slope(np.copy(raw_snippets), eod_heights)
     snippets = StandardScaler().fit_transform(snippets.T).T
 
     # scale so that the absolute integral = 1.
     snippets = (snippets.T/np.sum(np.abs(snippets), axis=1)).T
```

### Comparing `thunderfish-1.9.9/thunderfish/pulsetracker.py` & `thunderfish-2.0.0/src/thunderfish/pulsetracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 """
 by Dexter Frueh
 """
 
+import os
 import sys
-import numpy as np
+import ntpath
+import time
 import copy
+from shutil import copy2
+from collections import deque
+import numpy as np
 from scipy import stats
 from scipy import signal
 from scipy import optimize
 import matplotlib
 #from fish import ProgressFish
 import matplotlib.pyplot as plt
-from thunderfish.dataloader import open_data
-from thunderfish.eventdetection import detect_peaks
 from scipy.interpolate import interp1d
 from sklearn.preprocessing import StandardScaler
 from sklearn.decomposition import PCA
 from sklearn.cluster import DBSCAN
 from sklearn.cluster import AgglomerativeClustering
-from collections import deque
-import ntpath
-import time
-import os
-from shutil import copy2
-
-from collections import OrderedDict
+from thunderlab.dataloader import DataLoader
+from thunderlab.eventdetection import detect_peaks
 
 def makeeventlist(main_event_positions,side_event_positions,data,event_width=20):
     """
     Generate array of events that might be EODs of a pulse-type fish, using the location of peaks and troughs,
     the data and an optional width of an supposed EOD-event.
     The generated event-array contains location and height of such events.
     The height of the events is calculated by its height-difference to nearby troughs and main events that have no side events in a range closer than event_width are discarded and not considered as EOD event.
@@ -42,15 +40,15 @@
     data: array of float
         The given data.
     event_width: int or float, optional
 
     Returns
     -------
     EOD_events: ndarray
-        2D array containing data with 'np.float' type, size (number_of_properties = 3, number_of_events).
+        2D array containing data with 'float' type, size (number_of_properties = 3, number_of_events).
         Generated and combined data of the detected events in an array with arrays of x, y and height along the first axis.
 
     """
     mainfirst = int((min(main_event_positions[0],side_event_positions[0])<side_event_positions[0]))  # determines if there is a peak or through first. Evaluates to 1 if there is a peak first.
     main_x = main_event_positions
     main_y = data[main_event_positions]
     # empty placeholders, filled in the next step while iterating over the properties of single main
@@ -91,15 +89,15 @@
                 h[...] = y-r_side_y
         elif r_side_ind == len(side_event_positions):
             if l_distance> event_width:
                 r[...] = False
             else:
                 h[...] = y-l_side_y
     # generate return array and discard all events that are not marked as real
-    EOD_events = np.array([main_x, main_y, main_h], dtype = np.float)[:,main_real==1]
+    EOD_events = np.array([main_x, main_y, main_h], dtype = float)[:,main_real==1]
     return EOD_events
 
 def discardnearbyevents(event_locations, event_heights, min_distance):
     """
     Given a number of events with given location and heights, returns a selection
     of these events where  no event is closer than eventwidth to the next event.
     Among neighboring events closer than eventwidth the event with smaller height
@@ -638,15 +636,15 @@
      """
      deleteclasses = []
      for cl in np.unique(peaks[3]):
          peaksofclass = peaks[:,peaks[3] == cl]
          isi = np.diff(peaksofclass[0])
          isi_mean = np.mean(isi)
          widepeaks = 0
-         isi_tenth_area = lambda x, isi : np.arange(np.floor(x-0.1*isi),np.ceil(x+0.1*isi),1, dtype = np.int)
+         isi_tenth_area = lambda x, isi : np.arange(np.floor(x-0.1*isi),np.ceil(x+0.1*isi),1, dtype=int)
          for p in peaksofclass.T:
              data = np.array(data)
              try:
                  for dp_around in data[isi_tenth_area(p[0],isi_mean)]:
                     if dp_around <= p[1]-p[2]:
                        break
              except (IndexError,ValueError) as e:
@@ -661,17 +659,17 @@
 
 def plot_events_on_data(peaks, data, colors):
     """
         plots the detected events onto the data timeseries. If the events are classified, the classes are plotted in different colors and the class -1 (not belonging to a cluster) is plotted in black
     """
     plt.plot(range(len(data)),data, color = 'black')
     if len(peaks)>3:
-        classlist =  np.array(peaks[3],dtype=np.int)
+        classlist =  np.array(peaks[3],dtype=int)
         if len(peaks) > 4:
-            classlist = np.array(peaks[4],dtype=np.int)
+            classlist = np.array(peaks[4],dtype=int)
         #classlist=labels
         cmap = plt.get_cmap('jet')
 
         for cl in np.unique(classlist):
 
             if cl == -1:
                 color = 'black'
@@ -802,15 +800,15 @@
     eods: numpy array
         2D numpy array. first axis: attributes of an EOD (x (datapoints), y (recorded voltage), height (difference from maximum to minimum), class), second axis: EODs in chronological order.
     """
     
     # parameters for the analysis
     thresh = 0.04 # minimal threshold for peakdetection
     peakwidth = 20 # width of a peak and minimal distance between two EODs
-    # basic parameters for thunderfish.dataloader.open_data
+    # basic parameters for thunderfish.dataloader.DataLoader
     verbose = 0
     channel = 0
     ultimate_threshold = thresh+0.01
     startblock = 0
     starttime = int(starttime)
     endtime = int(endtime)
     timegiven = False
@@ -831,23 +829,23 @@
         quit()
     if npmmp:
         #proceed = input('With the option npmmp enabled, a numpy memmap will be saved to ' + datasavepath + '. continue? [y/n] ').lower()
         proceed = 'y'
         if proceed != 'y':
              quit()
     # starting analysis
-    with open_data(filepath, channel, deltat, 0.0, verbose) as data:
+    with DataLoader(filepath, deltat, 0.0, verbose) as data:
 
         samplerate = data.samplerate
 
         # selected time interval
         if timegiven == True:
             parttime1 = starttime*samplerate
             parttime2 = endtime*samplerate
-            data = data[parttime1:parttime2]
+            data = data[parttime1:parttime2,channel]
 
         #split data into blocks
         nblock = int(deltat*samplerate)
         if len(data)%nblock != 0:
             blockamount = len(data)//nblock + 1
         else:
             blockamount = len(data)//nblock
@@ -855,15 +853,15 @@
 
         pca_cur = 0
         progress = 0
 
         for idx in range(0, blockamount):
             print('BLOCK %i/%i'%(idx+1,blockamount))
 
-            blockdata = data[idx*nblock:(idx+1)*nblock]
+            blockdata = data[idx*nblock:(idx+1)*nblock,channel]
             if progress < (idx*100 //blockamount):
                 progress = (idx*100)//blockamount
             progressstr = ' Filestatus: '
 
             # fish.animate(amount = idx, dexextra = progressstr)
              # delete peaks under absolute threshold
             
@@ -940,15 +938,15 @@
                     
                     if plot_eods==True:
                         plt.title('Detected and classified EODs')
                         plt.xlabel('time [ms]')
                         plt.ylabel('signal (normalized)')
                     
                         phandles, plabels = plt.gca().get_legend_handles_labels()
-                        by_label = OrderedDict(zip(plabels, phandles))
+                        by_label = dict(zip(plabels, phandles))
                         plt.legend(by_label.values(), by_label.keys())
                         plt.show()
 
                     for lab in np.unique(labels):
                         
                         if lab == -1:
                             c = 'k'
@@ -962,15 +960,15 @@
                 
                     if plot_features==True:
                         plt.title('EOD Features')
                         plt.xlabel('feature [#]')
                         plt.ylabel('value [a.u.]')
                     
                         phandles, plabels = plt.gca().get_legend_handles_labels()
-                        by_label = OrderedDict(zip(plabels, phandles))
+                        by_label = dict(zip(plabels, phandles))
                         plt.legend(by_label.values(), by_label.keys())
                         plt.show()
 
                     #peaklist.len = nblock
                     worldpeaks = np.copy(peaks)
                     worldpeaks[0] = worldpeaks[0] + (idx*nblock)
                     # delete the classification that only considers wave shape.
@@ -993,15 +991,15 @@
                     else:
                         if idx > 0:
                             all_eods = np.concatenate((all_eods,thisblock_eods),axis = 1)
                         else:
                             all_eods = thisblock_eods
         if plot_steps == True:
             print('FINAL RESULTS')
-            plot_events_on_data(all_eods, data, colors)
+            plot_events_on_data(all_eods, data[:,channel], colors)
     #plot_events_on_data(all_eods,data)
     print('returnes analyzed EODS. Calculate frequencies using all of these but discard the data from the EODS within the lowest few percent of amplitude')
 
     if npmmp:
         all_eods = np.memmap(datasavepath+'/'+mmpname, dtype='float64', mode='r+', shape=(4,eods_len), order = 'F')
     if save == 1:
        path = filename[:-4]+"/"
```

### Comparing `thunderfish-1.9.9/thunderfish/thunderfish.py` & `thunderfish-2.0.0/src/thunderfish/thunderfish.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,53 @@
-"""
-# thunderfish
+"""# thunderfish
 
 Automatically detect and analyze all EOD waveforms in short recordings
 and generated summary plots and data tables.
 
 Run it from the thunderfish development directory as:
-```
-python3 -m thunderfish.thunderfish audiofile.wav
+```sh
+> python3 -m thunderfish.thunderfish audiofile.wav
 ```
 Or install thunderfish
-```
-sudo pip3 install .
+```sh
+> sudo pip3 install .
 ```
 Then you can run it directly from every directory:
-```
-thunderfish audiofile.wav
+```sh
+> thunderfish audiofile.wav
 ```
 """
 
 import sys
 import os
 import glob
+import io
+import zipfile
 import argparse
 import traceback
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.gridspec as gridspec
 import matplotlib.ticker as ticker
 import matplotlib.lines as ml
 from matplotlib.transforms import Bbox
 from matplotlib.backends.backend_pdf import PdfPages
 from multiprocessing import Pool, freeze_support, cpu_count
-from audioio.playaudio import play, fade
+from audioio import play, fade, load_audio
+from thunderlab.configfile import ConfigFile
+from thunderlab.dataloader import load_data
+from thunderlab.powerspectrum import decibel, plot_decibel_psd, multi_psd
+from thunderlab.powerspectrum import add_multi_psd_config, multi_psd_args
+from thunderlab.tabledata import TableData, add_write_table_config, write_table_args
 from .version import __version__, __year__
-from .configfile import ConfigFile
-from .dataloader import load_data
 from .bestwindow import add_clip_config, add_best_window_config
 from .bestwindow import clip_args, best_window_args
 from .bestwindow import analysis_window, plot_data_window
 from .checkpulse import check_pulse, add_check_pulse_config, check_pulse_args
 from .pulses import extract_pulsefish
-from .powerspectrum import decibel, plot_decibel_psd, multi_psd
-from .powerspectrum import add_multi_psd_config, multi_psd_args
 from .harmonics import add_psd_peak_detection_config, add_harmonic_groups_config
 from .harmonics import harmonic_groups, harmonic_groups_args, psd_peak_detection_args
 from .harmonics import colors_markers, plot_harmonic_groups
 from .consistentfishes import consistent_fishes
 from .eodanalysis import eod_waveform, analyze_wave, analyze_pulse
 from .eodanalysis import clipped_fraction
 from .eodanalysis import plot_eod_recording, plot_pulse_eods
@@ -53,22 +55,24 @@
 from .eodanalysis import plot_pulse_spectrum, plot_wave_spectrum
 from .eodanalysis import add_eod_analysis_config, eod_waveform_args
 from .eodanalysis import analyze_wave_args, analyze_pulse_args
 from .eodanalysis import add_species_config
 from .eodanalysis import wave_quality, wave_quality_args, add_eod_quality_config
 from .eodanalysis import pulse_quality, pulse_quality_args
 from .eodanalysis import save_eod_waveform, save_wave_eodfs, save_wave_fish, save_pulse_fish
-from .eodanalysis import save_wave_spectrum, save_pulse_spectrum, save_pulse_peaks
+from .eodanalysis import save_wave_spectrum, save_pulse_spectrum, save_pulse_peaks, save_pulse_times
+from .eodanalysis import load_eod_waveform, load_wave_eodfs, load_wave_fish, load_pulse_fish
+from .eodanalysis import load_wave_spectrum, load_pulse_spectrum, load_pulse_peaks
+from .eodanalysis import save_analysis, load_analysis, load_recording
+from .eodanalysis import parse_filename, file_types
 from .fakefish import normalize_wavefish, export_wavefish
-from .tabledata import TableData, add_write_table_config, write_table_args
 
 
 def configuration():
-    """
-    Assemble configuration parameter for thunderfish.
+    """Assemble configuration parameter for thunderfish.
 
     Returns
     -------
     cfg: ConfigFile
         Configuration parameters.
     """
     cfg = ConfigFile()
@@ -91,16 +95,15 @@
     add_species_config(cfg)
     add_write_table_config(cfg, table_format='csv', unit_style='row',
                            align_columns=True, shrink_width=False)
     return cfg
 
 
 def save_configuration(cfg, config_file):
-    """
-    Save configuration parameter for thunderfish to a file.
+    """Save configuration parameter for thunderfish to a file.
 
     Parameters
     ----------
     cfg: ConfigFile
         Configuration parameters and their values.
     config_file: string
         Name of the configuration file to be loaded.
@@ -116,15 +119,15 @@
         del cfg['fileLaTeXLabelCommand']
         del cfg['fileLaTeXMergeStd']
         cfg.dump(config_file)
 
 
 def detect_eods(data, samplerate, min_clip, max_clip, name, mode,
                 verbose, plot_level, cfg):
-    """ Detect EODs of all fish present in the data.
+    """Detect EODs of all fish present in the data.
 
     Parameters
     ----------
     data: array of floats
         The recording in which to detect EODs.
     samplerate: float
         Sampling rate of the dataset.
@@ -170,20 +173,24 @@
     power_thresh:  2 D array or None
         Frequency (first column) and power (second column) of threshold
         derived from single pulse spectra to discard false wave fish.
         None if no pulse fish was detected.
     skip_reason: list of string
         Reasons, why an EOD was discarded.
     """
+    dfreq = np.nan
+    nfft = 0
     psd_data = [[]]
     wave_eodfs = []
     wave_indices = []
     if 'w' in mode:
         # detect wave fish:
         psd_data = multi_psd(data, samplerate, **multi_psd_args(cfg))
+        dfreq = np.mean(np.diff(psd_data[0][:,0]))
+        nfft = int(samplerate/dfreq)
         h_kwargs = psd_peak_detection_args(cfg)
         h_kwargs.update(harmonic_groups_args(cfg))
         wave_eodfs_list = []
         for i, psd in enumerate(psd_data):
             wave_eodfs = harmonic_groups(psd[:,0], psd[:,1], verbose-1, **h_kwargs)[0]
             if verbose > 0 and len(psd_data) > 1:
                 numpsdresolutions = cfg.value('numberPSDResolutions')
@@ -211,15 +218,15 @@
     power_thresh = None
     skip_reason = []
     max_pulse_amplitude = 0.0
     zoom_window = []
 
     if 'p' in mode:
         # detect pulse fish:
-        _, eod_times, eod_peaktimes, zoom_window, _ = extract_pulsefish(data, samplerate, verbose=verbose, plot_level=plot_level, save_path=os.path.splitext(os.path.basename(name))[0])
+        _, eod_times, eod_peaktimes, zoom_window, _ = extract_pulsefish(data, samplerate, verbose=verbose-1, plot_level=plot_level, save_path=os.path.splitext(os.path.basename(name))[0])
 
         #eod_times = []
         #eod_peaktimes = []
         if verbose > 0:
             if len(eod_times) > 0:
                 print('found %2d pulsefish EODs' % len(eod_times))
             else:
@@ -236,17 +243,20 @@
                                                           freq_resolution=min_freq_res,
                                                           **analyze_pulse_args(cfg))
             if len(peaks) == 0:
                 print('error: no peaks in pulse EOD detected')
                 continue
             clipped_frac = clipped_fraction(data, samplerate, eod_times0,
                                             mean_eod, min_clip, max_clip)
-            props['peaktimes'] = eod_pts      # XXX that should go into analyze pulse
+            props['peaktimes'] = eod_pts  # XXX that should go into analyze pulse
             props['index'] = len(eod_props)
             props['clipped'] = clipped_frac
+            props['samplerate'] = samplerate
+            props['nfft'] = nfft
+            props['dfreq'] = dfreq
 
             # add good waveforms only:
             skips, msg, skipped_clipped = pulse_quality(props, **pulse_quality_args(cfg))
 
             if len(skips) == 0:
                 eod_props.append(props)
                 mean_eods.append(mean_eod)
@@ -295,17 +305,17 @@
                         wave_eodfs.pop(n-1-k)
                         if verbose > 0:
                             print('skip %6.1fHz wave  fish: %2d harmonics are below pulsefish threshold' % (fish[0,0], nbelow))
                         break
 
     if 'w' in mode:
         # analyse EOD waveform of all wavefish:
-        powers = np.array([np.sum(fish[:, 1]**2) for fish in wave_eodfs])
+        powers = np.array([np.sum(fish[:,1]) for fish in wave_eodfs])
         power_indices = np.argsort(-powers)
-        wave_indices = np.zeros(len(wave_eodfs), dtype=np.int) - 3
+        wave_indices = np.zeros(len(wave_eodfs), dtype=int) - 3
         for k, idx in enumerate(power_indices):
             fish = wave_eodfs[idx]
             eod_times = np.arange(0.0, len(data)/samplerate, 1.0/fish[0,0])
             mean_eod, eod_times = \
                 eod_waveform(data, samplerate, eod_times, win_fac=3.0, min_win=0.0,
                              min_sem=(k==0), **eod_waveform_args(cfg))
             mean_eod, props, sdata, error_str = \
@@ -313,28 +323,31 @@
             if error_str:
                 print(name + ': ' + error_str)
             clipped_frac = clipped_fraction(data, samplerate, eod_times,
                                             mean_eod, min_clip, max_clip)
             props['n'] = len(eod_times)
             props['index'] = len(eod_props)
             props['clipped'] = clipped_frac
+            props['samplerate'] = samplerate
+            props['nfft'] = nfft
+            props['dfreq'] = dfreq
             # remove wave fish that are smaller than the largest pulse fish:
             if props['p-p-amplitude'] < 0.01*max_pulse_amplitude:
                 rm_indices = power_indices[k:]
                 if verbose > 0:
                     print('skip %6.1fHz wave  fish: power=%5.1fdB, p-p amplitude=%5.1fdB smaller than pulse fish=%5.1dB - 20dB' %
                           (props['EODf'], decibel(powers[idx]),
                            decibel(props['p-p-amplitude']), decibel(max_pulse_amplitude)))
                     for idx in rm_indices[1:]:
                         print('skip %6.1fHz wave  fish: power=%5.1fdB even smaller' %
                               (wave_eodfs[idx][0,0], decibel(powers[idx])))
                 wave_eodfs = [eodfs for idx, eodfs in enumerate(wave_eodfs)
                               if idx not in rm_indices]
                 wave_indices = np.array([idcs for idx, idcs in enumerate(wave_indices)
-                                        if idx not in rm_indices], dtype=np.int)
+                                        if idx not in rm_indices], dtype=int)
                 break
             # add good waveforms only:
             remove, skips, msg = wave_quality(props, sdata[1:,3], **wave_quality_args(cfg))
             if len(skips) == 0:
                 wave_indices[idx] = props['index']
                 eod_props.append(props)
                 mean_eods.append(mean_eod)
@@ -345,125 +358,77 @@
             else:
                 wave_indices[idx] = -2 if remove else -1
                 skip_reason += ['%.1fHz wave fish %s' % (props['EODf'], skips)]
                 if verbose > 0:
                     print('%-6s %6.1fHz wave  fish: %s (%s)' %
                           ('remove' if remove else 'skip', props['EODf'], skips, msg))
         wave_eodfs = [eodfs for idx, eodfs in zip(wave_indices, wave_eodfs) if idx > -2]
-        wave_indices = np.array([idx for idx in wave_indices if idx > -2], dtype=np.int)
+        wave_indices = np.array([idx for idx in wave_indices if idx > -2], dtype=int)
     return (psd_data, wave_eodfs, wave_indices, eod_props, mean_eods,
             spec_data, peak_data, power_thresh, skip_reason, zoom_window)
 
 
 def remove_eod_files(output_basename, verbose, cfg):
-    """ Remove all files from previous runs of thunderfish
+    """Remove all files from previous runs of thunderfish
     """
     ff = cfg.value('fileFormat')
     if ff == 'py':
         fext = 'py'
     else:
-        fext = TableData.extensions[cfg.value('fileFormat')]
+        fext = TableData.extensions[ff]
     # remove all files from previous runs of thunderfish:
     for fn in glob.glob('%s*.%s' % (output_basename, fext)):
         os.remove(fn)
         if verbose > 0:
             print('removed file %s' % fn)
 
-            
-def save_eods(output_basename, eod_props, mean_eods, spec_data, peak_data,
-              wave_eodfs, wave_indices, unit, verbose, cfg):
-    """ Save analysis results of all EODs to files.
-    """
-    if write_table_args(cfg)['table_format'] == 'py':
-        with open(output_basename+'.py', 'w') as f:
-            name = os.path.basename(output_basename)
-            for k, sdata in enumerate(spec_data):
-                # save wave fish only:
-                if len(sdata)>0 and sdata.shape[1] > 2:
-                    fish = dict(amplitudes=sdata[:,3], phases=sdata[:,5])
-                    fish = normalize_wavefish(fish)
-                    export_wavefish(fish, name+'-%d_harmonics' % k, f)
-    else:
-        # all wave fish in wave_eodfs:
-        if len(wave_eodfs) > 0:
-            fp = save_wave_eodfs(wave_eodfs, wave_indices, output_basename,
-                                 **write_table_args(cfg))
-            if verbose > 0:
-                print('wrote file %s' % fp)
-        # all wave and pulse fish:
-        for i, (mean_eod, sdata, pdata) in enumerate(zip(mean_eods, spec_data, peak_data)):
-            fp = save_eod_waveform(mean_eod, unit, i, output_basename,
-                                   **write_table_args(cfg))
-            if verbose > 0:
-                print('wrote file %s' % fp)
-            # power spectrum:
-            if len(sdata)>0:
-                if sdata.shape[1] == 2:
-                    fp = save_pulse_spectrum(sdata, unit, i, output_basename,
-                                             **write_table_args(cfg))
-                else:
-                    fp = save_wave_spectrum(sdata, unit, i, output_basename,
-                                            **write_table_args(cfg))
-                if verbose > 0:
-                    print('wrote file %s' % fp)
-            # peaks:
-            fp = save_pulse_peaks(pdata, unit, i, output_basename,
-                                  **write_table_args(cfg))
-            if verbose > 0 and fp is not None:
-                print('wrote file %s' % fp)
-        # wave fish properties:
-        fp = save_wave_fish(eod_props, unit, output_basename,
-                            **write_table_args(cfg))
-        if verbose > 0 and fp:
-            print('wrote file %s' % fp)
-        # pulse fish properties:
-        fp = save_pulse_fish(eod_props, unit, output_basename,
-                             **write_table_args(cfg))
-        if verbose > 0 and fp:
-            print('wrote file %s' % fp)
-
 
 def plot_style():
-    """ Set style of plots.
+    """Set style of plots.
     """
     plt.rcParams['figure.facecolor'] = 'white'
     plt.rcParams['axes.facecolor'] = 'none'
     plt.rcParams['xtick.direction'] = 'out'
     plt.rcParams['ytick.direction'] = 'out'
 
 
 def axes_style(ax):
-    """ Fix style of axes.
+    """Fix style of axes.
 
     Parameters
     ----------
     ax: matplotlib axes
     """
     ax.spines['top'].set_visible(False)
     ax.spines['right'].set_visible(False)
     ax.get_xaxis().tick_bottom()
     ax.get_yaxis().tick_left()
 
                                 
-def plot_eods(base_name, raw_data, samplerate, channel, idx0, idx1, clipped,
-              psd_data, wave_eodfs, wave_indices, mean_eods, eod_props, peak_data, spec_data,
-              indices, unit, zoom_window, n_snippets=10, power_thresh=None, label_power=True,
-              all_eods=False, spec_plots='auto', log_freq=False, min_freq=0.0, max_freq=3000.0,
+def plot_eods(base_name, message_filename,
+              raw_data, samplerate, channel, idx0, idx1, clipped,
+              psd_data, wave_eodfs, wave_indices, mean_eods, eod_props,
+              peak_data, spec_data, indices, unit, zoom_window,
+              n_snippets=10, power_thresh=None, label_power=True,
+              all_eods=False, spec_plots='auto', skip_bad=True,
+              log_freq=False, min_freq=0.0, max_freq=3000.0,
               interactive=True, verbose=0):
     """Creates an output plot for the thunderfish program.
 
     This output contains the raw trace where the analysis window is
     marked, the power-spectrum of this analysis window where the
     detected fish are marked, plots of averaged EOD plots, and
     spectra of the EOD waveforms.
 
     Parameters
     ----------
     base_name: string
         Basename of audio_file.
+    message_filename: string or None
+        Path to meta-data message.
     raw_data: array
         Dataset.
     samplerate: float
         Sampling rate of the dataset.
     channel: int or None
         Channel of the recording to be put into the plot title.
         If None, do not write the channel into the title.
@@ -504,14 +469,16 @@
         If `True` put the power in decibel in addition to the frequency
         into the legend.
     all_eods: bool
         Plot all EOD waveforms.
     spec_plots: bool or 'auto'
         Plot amplitude spectra of EOD waveforms.
         If 'auto', plot them if there is a singel waveform only.
+    skip_bad: bool
+        Skip harmonic groups without index (entry in indices is negative).
     log_freq: boolean
         Logarithmic (True) or linear (False) frequency axis of power spectrum of recording.
     min_freq: float
         Limits of frequency axis of power spectrum of recording
         are set to `(min_freq, max_freq)` if `max_freq` is greater than zero
     max_freq: float
         Limits of frequency axis of power spectrum of recording
@@ -532,14 +499,18 @@
         if event.key in 'pP':
             if idx1 > idx0:
                 playdata = 1.0 * raw_data[idx0:idx1]
             else:
                 playdata = 1.0 * raw_data[:]
             fade(playdata, samplerate, 0.1)
             play(playdata, samplerate, blocking=False)
+        if event.key in 'mM' and message_filename:
+            # play voice message:
+            msg, msg_rate = load_audio(message_filename)
+            play(msg, msg_rate, blocking=False)
 
     def recording_format_coord(x, y):
         return 'full recording: x=%.3f s, y=%.3f' % (x, y)
 
     def recordingzoom_format_coord(x, y):
         return 'recording zoom-in: x=%.3f s, y=%.3f' % (x, y)
             
@@ -556,16 +527,17 @@
         return u'phase spectrum: x=%.0f, y=%.2f \u03c0' % (x, y/np.pi)
             
     def pulsepsd_format_coord(x, y):
         return 'single pulse power spectrum: x=%.1f Hz, y=%.1f dB' % (x, y)
 
     # count number of fish types to be plotted:
     if indices is None:
-        indices = list(range(len(eod_props)))
-    indices = np.array(indices, dtype=np.int)
+        indices = np.arange(len(eod_props))
+    else:
+        indices = np.array(indices, dtype=int)
     nwave = 0
     npulse = 0
     for idx in indices:
         if eod_props[idx]['type'] == 'pulse':
             npulse += 1
         elif eod_props[idx]['type'] == 'wave':
             nwave += 1
@@ -608,30 +580,32 @@
     ax.text(1.0, 1.0, 'thunderfish by Benda-Lab', fontsize=16, ha='right', va='top')
     ax.text(1.0, 0.0, 'version %s' % __version__, fontsize=16, ha='right', va='bottom')
     ax.set_frame_on(False)
     ax.set_axis_off()
     ax.set_navigate(False)
 
     # layout of recording and psd plots:
-    #force_both = True                    # set to True for debugging pulse and wave detection
+    #force_both = True  # set to True for debugging pulse and wave detection
     force_both = False
     posy = 1.0 - 4.0/height
     axr = None
     axp = None
     legend_inside = True
-    legendwidth = 3.2/width if label_power else 2.2/width
+    legendwidth = 2.2/width if label_power else 1.7/width
     if neods == 0:
         axr = fig.add_axes([leftx, posy, fullwidth, pheight])                    # top, wide
         if len(psd_data) > 0:
             axp = fig.add_axes([leftx, 2.0/height, fullwidth, pheight])              # bottom, wide
     else:
-        if npulse == 0 and nwave > 2 and len(psd_data) > 0 and not force_both:
+        if npulse == 0 and nwave > 2 and psd_data is not None and \
+           len(psd_data) > 0 and not force_both:
             axp = fig.add_axes([leftx, posy, fullwidth-legendwidth, pheight])    # top, wide
             legend_inside = False
-        elif (npulse > 0 or len(psd_data) == 0) and len(wave_eodfs) == 0 and not force_both:
+        elif (npulse > 0 or psd_data is None or len(psd_data) == 0) \
+             and len(wave_eodfs) == 0 and not force_both:
             axr = fig.add_axes([leftx, posy, fullwidth, pheight])                # top, wide
         else:
             axr = fig.add_axes([leftx, posy, halfwidth, pheight])                # top left
             label_power = False
             legendwidth = 2.2/width
             axp = fig.add_axes([midx, posy, halfwidth, pheight])                 # top, right
         
@@ -650,17 +624,22 @@
                 twidth = 5.0/eod_props[indices[0]]['EODf']
             else:
                 if len(wave_eodfs) > 0:
                     twidth = 3.0/eod_props[indices[0]]['EODf']
                 else:
                     twidth = 10.0/eod_props[indices[0]]['EODf']
             twidth = (1+twidth//0.005)*0.005
-        plot_eod_recording(axr, data, samplerate, twidth, unit, idx0/samplerate)
-        plot_pulse_eods(axr, data, samplerate, zoom_window, twidth, eod_props, idx0/samplerate,
-                        colors=pulse_colors, markers=pulse_markers, frameon=True, loc='upper right')
+        if data is not None and len(data) > 0:
+            plot_eod_recording(axr, data, samplerate, unit, twidth,
+                               idx0/samplerate)
+            plot_pulse_eods(axr, data, samplerate,
+                            zoom_window, twidth, eod_props,
+                            idx0/samplerate, colors=pulse_colors,
+                            markers=pulse_markers, frameon=True,
+                            loc='upper right')
         if axr.get_legend() is not None:
             axr.get_legend().get_frame().set_color('white')
         axr.set_title('Recording', fontsize=14, y=1.05)
         axr.format_coord = recordingzoom_format_coord
     
     # plot psd
     wave_colors, wave_markers = colors_markers()
@@ -674,24 +653,27 @@
                 title = '%d EOD frequencies' % len(wave_eodfs)
                 kwargs = {'title': title if len(wave_eodfs) > 2 else None }
                 if legend_inside:
                     kwargs.update({'bbox_to_anchor': (1.05, 1.1),
                                    'loc': 'upper right', 'legend_rows': 10,
                                    'frameon': True})
                 else:
-                    kwargs.update({'bbox_to_anchor': (1.0, 1.1), 'frameon': False,
-                                   'loc': 'upper left', 'legend_rows': 12})
+                    kwargs.update({'bbox_to_anchor': (1.02, 1.1),
+                                   'loc': 'upper left', 'legend_rows': 14,
+                                   'labelspacing': 0.6, 'frameon': False})
             plot_harmonic_groups(axp, wave_eodfs, wave_indices, max_groups=0,
+                                 skip_bad=skip_bad,
                                  sort_by_freq=True, label_power=label_power,
                                  colors=wave_colors, markers=wave_markers,
                                  **kwargs)
             if legend_inside:
                 axp.get_legend().get_frame().set_color('white')
-        plot_decibel_psd(axp, psd_data[:,0], psd_data[:,1], log_freq=log_freq,
-                         min_freq=min_freq, max_freq=max_freq, ymarg=5.0, color='blue')
+        if psd_data is not None and len(psd_data) > 0:
+            plot_decibel_psd(axp, psd_data[:,0], psd_data[:,1], log_freq=log_freq,
+                             min_freq=min_freq, max_freq=max_freq, ymarg=5.0, color='blue')
         axp.yaxis.set_major_locator(ticker.MaxNLocator(6))
         if len(wave_eodfs) == 1:
             axp.get_legend().set_visible(False)
             label = '%6.1f Hz' % wave_eodfs[0][0, 0]
             axp.set_title('Powerspectrum: %s' % label, y=1.05, fontsize=14)
         else:
             axp.set_title('Powerspectrum', y=1.05, fontsize=14)
@@ -744,39 +726,39 @@
         peaks = peak_data[idx]
         lx = leftx if spec_plots or k%2 == 0 else midx
         ax = fig.add_axes([lx, posy, halfwidth, pheight])
         axes_style(ax)
         ax.yaxis.set_major_locator(ticker.MaxNLocator(ny))
         if len(indices) > 1:
             ax.text(0.3, ty, '{EODf:.1f} Hz {type} fish'.format(**props),
-                       transform=ax.transAxes, fontsize=14)
+                       transform=ax.transAxes, fontsize=14, zorder=20)
             mx = 0.25
         else:
             ax.text(-0.1, ty, '{EODf:.1f} Hz {type} fish'.format(**props),
-                       transform=ax.transAxes, fontsize=14)
-            ax.text(0.5, ty, 'Averaged EOD',
-                       transform=ax.transAxes, fontsize=14, ha='center')
+                       transform=ax.transAxes, fontsize=14, zorder=20)
+            ax.text(0.5, ty, 'Averaged EOD', ha='center',
+                       transform=ax.transAxes, fontsize=14, zorder=20)
             mx = -0.14
         eodf = props['EODf']
         if props['type'] == 'wave':
             if axp is not None:
                 wk = np.nanargmin(np.abs(legend_wave_eodfs - eodf))
                 ma = ml.Line2D([mx], [my], color=w[wk].get_color(), marker=w[wk].get_marker(),
                                markersize=w[wk].get_markersize(), mec='none', clip_on=False,
                                label=w[wk].get_label(), transform=ax.transAxes)
                 ax.add_line(ma)
         else:
-            if axr is not None:
+            if axr is not None and len(legend_pulse_eodfs) > 0:
                 pk = np.argmin(np.abs(legend_pulse_eodfs - eodf))
                 ma = ml.Line2D([mx], [my], color=p[pk].get_color(), marker=p[pk].get_marker(),
                                markersize=p[pk].get_markersize(), mec='none', clip_on=False,
                                label=p[pk].get_label(), transform=ax.transAxes)
                 ax.add_line(ma)
         plot_eod_waveform(ax, mean_eod, props, peaks, unit)
-        if props['type'] == 'pulse':
+        if props['type'] == 'pulse' and 'times' in props:
             plot_eod_snippets(ax, data, samplerate, mean_eod[0,0], mean_eod[-1,0],
                               props['times'], n_snippets, props['flipped'])
         if not large_plots and k < max_plots-2:
             ax.set_xlabel('')
         ax.format_coord = meaneod_format_coord
 
         # plot spectra:
@@ -802,37 +784,39 @@
 
         if spec_plots or k%2 == 1:
             posy -= pstep
 
     # whole trace:
     ax = fig.add_axes([leftx, 0.6/height, fullwidth, 0.9/height])
     axes_style(ax)
-    plot_data_window(ax, raw_data, samplerate, unit, idx0, idx1, clipped)
+    if raw_data is not None and len(raw_data) > 0:
+        plot_data_window(ax, raw_data, samplerate, unit, idx0, idx1, clipped)
     ax.format_coord = recording_format_coord
 
     return fig
 
                             
-def plot_eod_subplots(base_name, subplots, raw_data, samplerate, idx0, idx1, clipped,
-                      psd_data, wave_eodfs, wave_indices, mean_eods, eod_props, peak_data,
-                      spec_data, unit, zoom_window, n_snippets=10, power_thresh=None,
-                      label_power=True, log_freq=False, min_freq=0.0, max_freq=3000.0):
-    """
-    Plot time traces and spectra into separate files.
+def plot_eod_subplots(base_name, subplots, raw_data, samplerate, idx0, idx1,
+                      clipped, psd_data, wave_eodfs, wave_indices, mean_eods,
+                      eod_props, peak_data, spec_data, unit, zoom_window,
+                      n_snippets=10, power_thresh=None, label_power=True,
+                      skip_bad=True, log_freq=False,
+                      min_freq=0.0, max_freq=3000.0, save=True):
+    """Plot time traces and spectra into separate windows or files.
 
     Parameters
     ----------
     base_name: string
         Basename of audio_file.
     subplots: string
         Specifies which subplots to plot:
         r) recording with best window, t) data trace with detected pulse fish,
         p) power spectrum with detected wave fish, w/W) mean EOD waveform,
         s/S) EOD spectrum, e/E) EOD waveform and spectra. With capital letters
-        all fish are saved into a single pdf filem with small letters each fish
+        all fish are saved into a single pdf file, with small letters each fish
         is saved into a separate file.
     raw_data: array
         Dataset.
     samplerate: float
         Sampling rate of the dataset.
     idx0: float
         Index of the beginning of the analysis window in the dataset.
@@ -863,164 +847,353 @@
         Number of EOD waveform snippets to be plotted. If zero do not plot any.
     power_thresh:  2 D array or None
         Frequency (first column) and power (second column) of threshold
         derived from single pulse spectra to discard false wave fish.
     label_power: boolean
         If `True` put the power in decibel in addition to the frequency
         into the legend.
+    skip_bad: bool
+        Skip harmonic groups without index (entry in indices is negative).
     log_freq: boolean
         Logarithmic (True) or linear (False) frequency axis of power spectrum of recording.
     min_freq: float
         Limits of frequency axis of power spectrum of recording
         are set to `(min_freq, max_freq)` if `max_freq` is greater than zero
     max_freq: float
         Limits of frequency axis of power spectrum of recording
         are set to `(min_freq, max_freq)` and limits of power axis are computed
         from powers below max_freq if `max_freq` is greater than zero
+    save: bool
+        If True save plots to files instead of showing them.
     """
     plot_style()
     if 'r' in subplots:
         fig, ax = plt.subplots(figsize=(10, 2))
         fig.subplots_adjust(left=0.07, right=0.99, bottom=0.22, top=0.95)
         plot_data_window(ax, raw_data, samplerate, unit, idx0, idx1, clipped)
         ax.yaxis.set_major_locator(ticker.MaxNLocator(5))
         axes_style(ax)
-        fig.savefig(base_name + '-recording.pdf')
+        if save:
+            fig.savefig(base_name + '-recording.pdf')
     if 't' in subplots:
         fig, ax = plt.subplots(figsize=(10, 6))
-        ax.text(0.5, 0.5, 'not implemented yet',
-                transform=ax.transAxes, ha='center', va='center')
+        twidth = 0.1
+        if len(eod_props) > 0:
+            if eod_props[0]['type'] == 'wave':
+                twidth = 5.0/eod_props[0]['EODf']
+            else:
+                if len(wave_eodfs) > 0:
+                    twidth = 3.0/eod_props[0]['EODf']
+                else:
+                    twidth = 10.0/eod_props[0]['EODf']
+        twidth = (1+twidth//0.005)*0.005
+        pulse_colors, pulse_markers = colors_markers()
+        pulse_colors = pulse_colors[3:]
+        pulse_markers = pulse_markers[3:]
+        plot_eod_recording(ax, raw_data[idx0:idx1], samplerate, unit,
+                           twidth, idx0/samplerate)
+        plot_pulse_eods(ax, raw_data[idx0:idx1], samplerate,
+                        zoom_window, twidth, eod_props,
+                        idx0/samplerate, colors=pulse_colors,
+                        markers=pulse_markers, frameon=True,
+                        loc='upper right')
+        if ax.get_legend() is not None:
+            ax.get_legend().get_frame().set_color('white')
         axes_style(ax)
-        fig.savefig(base_name + '-trace.pdf')
+        if save:
+            fig.savefig(base_name + '-trace.pdf')
     if 'p' in subplots:
         fig, ax = plt.subplots(figsize=(10, 5))
         fig.subplots_adjust(left=0.08, right=0.975, bottom=0.11, top=0.9)
         axes_style(ax)
         if power_thresh is not None:
             ax.plot(power_thresh[:,0], decibel(power_thresh[:,1]), '#CCCCCC', lw=1)
         if len(wave_eodfs) > 0:
             kwargs = {}
             if len(wave_eodfs) > 1:
                 title = '%d EOD frequencies' % len(wave_eodfs)
                 kwargs = {'title': title if len(wave_eodfs) > 2 else None }
                 if len(wave_eodfs) > 2:
-                    fig.subplots_adjust(left=0.08, right=0.72, bottom=0.11, top=0.9)
-                    kwargs.update({'bbox_to_anchor': (1.0, 1.1),
-                                   'loc': 'upper left', 'legend_rows': 12})
+                    fig.subplots_adjust(left=0.08, right=0.78, bottom=0.11, top=0.9)
+                    kwargs.update({'bbox_to_anchor': (1.01, 1.1),
+                                   'loc': 'upper left', 'legend_rows': 14,
+                                   'labelspacing': 0.6})
                 else:
                     kwargs.update({'bbox_to_anchor': (1.05, 1.1),
                                    'loc': 'upper right', 'legend_rows': 10})
             wave_colors, wave_markers = colors_markers()
             plot_harmonic_groups(ax, wave_eodfs, wave_indices, max_groups=0,
+                                 skip_bad=skip_bad,
                                  sort_by_freq=True, label_power=label_power,
                                  colors=wave_colors, markers=wave_markers,
                                  frameon=False, **kwargs)
         plot_decibel_psd(ax, psd_data[:,0], psd_data[:,1], log_freq=log_freq,
                          min_freq=min_freq, max_freq=max_freq, ymarg=5.0, color='blue')
         ax.yaxis.set_major_locator(ticker.MaxNLocator(6))
         if len(wave_eodfs) == 1:
             ax.get_legend().set_visible(False)
             label = '%6.1f Hz' % wave_eodfs[0][0, 0]
             ax.set_title('Powerspectrum: %s' % label, y=1.05)
         else:
             ax.set_title('Powerspectrum', y=1.05)
-        fig.savefig(base_name + '-psd.pdf')
+        if save:
+            fig.savefig(base_name + '-psd.pdf')
     if 'w' in subplots or 'W' in subplots:
         mpdf = None
         if 'W' in subplots:
             mpdf = PdfPages(base_name + '-waveforms.pdf')
         for meod, props, peaks in zip(mean_eods, eod_props, peak_data):
+            if meod is None:
+                continue
             fig, ax = plt.subplots(figsize=(5, 3))
             fig.subplots_adjust(left=0.18, right=0.98, bottom=0.15, top=0.9)
-            ax.set_title('{index:d}: {EODf:.1f} Hz {type} fish'.format(**props))
+            if not props is None:
+                ax.set_title('{index:d}: {EODf:.1f} Hz {type} fish'.format(**props))
             plot_eod_waveform(ax, meod, props, peaks, unit)
             data = raw_data[idx0:idx1] if idx1 > idx0 else raw_data
-            if props['type'] == 'pulse':
+            if not props is None and props['type'] == 'pulse' and \
+               'times' in props:
                 plot_eod_snippets(ax, data, samplerate, meod[0,0], meod[-1,0],
                                   props['times'], n_snippets)
             ax.yaxis.set_major_locator(ticker.MaxNLocator(6))
             axes_style(ax)
             if mpdf is None:
-                fig.savefig(base_name + '-waveform-%d.pdf' % props['index'])
+                if save:
+                    fig.savefig(base_name + '-waveform-%d.pdf' % props['index'])
             else:
                 mpdf.savefig(fig)
         if mpdf is not None:
             mpdf.close()
     if 's' in subplots or 'S' in subplots:
         mpdf = None
         if 'S' in subplots:
             mpdf = PdfPages(base_name + '-spectrum.pdf')
         for props, peaks, spec in zip(eod_props, peak_data, spec_data):
-            if props['type'] == 'pulse':
+            if spec is None:
+                continue
+            if props is not None and props['type'] == 'pulse':
                 fig, ax = plt.subplots(figsize=(5, 3.5))
                 fig.subplots_adjust(left=0.15, right=0.967, bottom=0.16, top=0.88)
                 axes_style(ax)
                 ax.set_title('{index:d}: {EODf:.1f} Hz {type} fish'.format(**props), y=1.07)
                 plot_pulse_spectrum(ax, spec, props)
             else:
                 fig, (ax1, ax2) = plt.subplots(2, 1, figsize=(5, 3.5))
                 fig.subplots_adjust(left=0.15, right=0.97, bottom=0.16, top=0.88, hspace=0.4)
                 axes_style(ax1)
                 axes_style(ax2)
-                ax1.set_title('{index:d}: {EODf:.1f} Hz {type} fish'.format(**props), y=1.15)
+                if not props is None:
+                    ax1.set_title('{index:d}: {EODf:.1f} Hz {type} fish'.format(**props), y=1.15)
                 plot_wave_spectrum(ax1, ax2, spec, props, unit)
                 ax1.set_xticklabels([])
                 ax1.yaxis.set_major_locator(ticker.MaxNLocator(4))
             if mpdf is None:
-                fig.savefig(base_name + '-spectrum-%d.pdf' % props['index'])
+                if save:
+                    fig.savefig(base_name + '-spectrum-%d.pdf' % props['index'])
             else:
                 mpdf.savefig(fig)
         if mpdf is not None:
             mpdf.close()
     if 'e' in subplots or 'E' in subplots:
         mpdf = None
         if 'E' in subplots:
             mpdf = PdfPages(base_name + '-eods.pdf')
         for meod, props, peaks, spec in zip(mean_eods, eod_props, peak_data, spec_data):
+            if meod is None or spec is None:
+                continue
             fig = plt.figure(figsize=(10, 3.5))
             gs = gridspec.GridSpec(nrows=2, ncols=2, left=0.09, right=0.98,
                                    bottom=0.16, top=0.88, wspace=0.4, hspace=0.4)
             ax1 = fig.add_subplot(gs[:,0])
-            ax1.set_title('{index:d}: {EODf:.1f} Hz {type} fish'.format(**props), y=1.07)
+            if not props is None:
+                ax1.set_title('{index:d}: {EODf:.1f} Hz {type} fish'.format(**props), y=1.07)
             plot_eod_waveform(ax1, meod, props, peaks, unit)
             data = raw_data[idx0:idx1] if idx1 > idx0 else raw_data
-            if props['type'] == 'pulse':
+            if not props is None and props['type'] == 'pulse' and 'times' in props:
                 plot_eod_snippets(ax1, data, samplerate, meod[0,0], meod[-1,0],
                                   props['times'], n_snippets)
             ax1.yaxis.set_major_locator(ticker.MaxNLocator(6))
             axes_style(ax1)
-            if props['type'] == 'pulse':
+            if not props is None and props['type'] == 'pulse':
                 ax2 = fig.add_subplot(gs[:,1])
                 axes_style(ax2)
                 plot_pulse_spectrum(ax2, spec, props)
                 ax2.set_title('Single pulse spectrum', y=1.07)
             else:
                 ax2 = fig.add_subplot(gs[0,1])
                 ax3 = fig.add_subplot(gs[1,1])
                 axes_style(ax2)
                 axes_style(ax3)
                 plot_wave_spectrum(ax2, ax3, spec, props, unit)
                 ax2.set_title('Amplitude and phase spectrum', y=1.15)
                 ax2.set_xticklabels([])
                 ax2.yaxis.set_major_locator(ticker.MaxNLocator(4))
             if mpdf is None:
-                fig.savefig(base_name + '-eod-%d.pdf' % props['index'])
+                if save:
+                    fig.savefig(base_name + '-eod-%d.pdf' % props['index'])
             else:
                 mpdf.savefig(fig)
         if mpdf is not None:
             mpdf.close()
-    plt.close()
+    if not save:
+        plt.show()
+    plt.close('all')
+
 
+def thunderfish_plot(files, data_path=None, load_kwargs={},
+                     all_eods=False, spec_plots='auto', skip_bad=True,
+                     save_plot=False, multi_pdf=None,
+                     save_subplots='', log_freq=False, min_freq=0.0,
+                     max_freq=3000.0, output_folder='.',
+                     keep_path=False, verbose=0):
+    """Generate plots from saved analysis results.
 
+    Parameters
+    ----------
+    files: list of str
+        Analysis files from a single recording.
+    data_path: str
+        Path where to find the raw data.
+    load_kwargs: dict
+        Key-word arguments for the `load_data()` function.
+    all_eods: bool
+        If True, plot all EOD waveforms.
+    spec_plots: bool or 'auto'
+        Plot amplitude spectra of EOD waveforms.
+        If 'auto', plot them if there is a singel waveform only.
+    skip_bad: bool
+        Skip harmonic groups without index in the spectrum plot.
+    save_plot: bool
+        If True, save plots as pdf file.
+    multi_pdf: matplotlib.PdfPages or None
+        PdfPages instance in which to save plots.
+    save_subplots: string
+        If not empty, specifies subplots to be saved as separate pdf
+        files: r) recording with best window, t) data trace with
+        detected pulse fish, p) power spectrum with detected wave
+        fish, w/W) mean EOD waveform, s/S) EOD spectrum, e/E) EOD
+        waveform and spectra. Capital letters produce a single
+        multipage pdf containing plots of all detected fish.
+    log_freq: boolean
+        Logarithmic (True) or linear (False) frequency axis of
+        power spectrum of recording.
+    min_freq: float
+        Limits of frequency axis of power spectrum of recording
+        are set to `(min_freq, max_freq)`, if `max_freq` is greater than zero
+    max_freq: float
+        Limits of frequency axis of power spectrum of recording
+        are set to `(min_freq, max_freq)` and limits of power axis are computed
+        from powers below max_freq, if `max_freq` is greater than zero
+    output_folder: string
+        Folder where to save results.
+    keep_path: bool
+        Add relative path of data files to output path.
+    verbose: int
+       Verbosity level (for debugging).
+    """
+    if len(save_subplots) == 0:
+        save_subplots = 'rtpwsed'  # plot everything
+    # load analysis results:
+    mean_eods, wave_eodfs, wave_indices, eod_props, spec_data, \
+        peak_data, base_name, channel, unit = load_analysis(files)
+    if len(mean_eods) == 0 or all(me is None for me in mean_eods):
+        save_subplots = save_subplots.replace('w', '')
+        save_subplots = save_subplots.replace('W', '')
+        save_subplots = save_subplots.replace('e', '')
+        save_subplots = save_subplots.replace('E', '')
+        save_subplots = save_subplots.replace('d', '')
+    if len(spec_data) == 0 or all(sd is None for sd in spec_data):
+        save_subplots = save_subplots.replace('s', '')
+        save_subplots = save_subplots.replace('S', '')
+        save_subplots = save_subplots.replace('e', '')
+        save_subplots = save_subplots.replace('E', '')
+        save_subplots = save_subplots.replace('d', '')
+    clipped = 0.0
+    if len(eod_props) > 0 and not eod_props[0] is None and \
+       'winclipped' in eod_props[0]:
+        clipped = eod_props[0]['winclipped']
+    zoom_window = [1.2, 1.3]
+    # load recording:
+    psd_data = None
+    if base_name:
+        name = os.path.basename(base_name) if data_path and data_path != '.' else base_name
+        data_path = os.path.join(data_path, name)
+    data, samplerate, idx0, idx1, data_path = \
+        load_recording(data_path, channel, load_kwargs,
+                       eod_props, verbose-1)
+    if data is None:
+        save_subplots = save_subplots.replace('r', '')
+        save_subplots = save_subplots.replace('t', '')
+        save_subplots = save_subplots.replace('d', '')
+    if verbose > 0:
+        print('loaded', data_path)
+    if len(eod_props) > 0 and not eod_props[0] is None and \
+       'dfreq' in eod_props[0] and data is not None and len(data) > 0:
+        psd_data = multi_psd(data[idx0:idx1],
+                             samplerate,
+                             1.1*eod_props[0]['dfreq'])[0]
+    if psd_data is not None and len(psd_data) > 0:
+        for idx, fish in zip(wave_indices, wave_eodfs):
+            if idx < 0:
+                for k in range(len(fish)):
+                    fish[k,1] = psd_data[np.argmin(np.abs(psd_data[:,0] - fish[k,0])),1]
+    if psd_data is None:
+        save_subplots = save_subplots.replace('p', '')
+        save_subplots = save_subplots.replace('d', '')
+    # file name for output files:
+    fn = base_name if keep_path else os.path.basename(base_name)
+    output_basename = os.path.join(output_folder, fn)
+    if channel >= 0:
+        output_basename += f'-c{channel}'
+    # make directory if necessary:
+    if keep_path:
+        outpath = os.path.dirname(output_basename)
+        if not os.path.exists(outpath):
+            if verbose > 0:
+                print('mkdir %s' % outpath)
+            os.makedirs(outpath)
+    # plot:
+    if len(save_subplots) == 0 or 'd' in save_subplots:
+        fig = plot_eods(os.path.basename(base_name), None,
+                        data, samplerate,
+                        channel, idx0, idx1, clipped, psd_data,
+                        wave_eodfs, wave_indices, mean_eods,
+                        eod_props, peak_data, spec_data, None, unit,
+                        zoom_window, 10, None, True, all_eods,
+                        spec_plots, skip_bad, log_freq, min_freq,
+                        max_freq, interactive=not save_plot,
+                        verbose=verbose-1)
+        if save_plot:
+            if multi_pdf is not None:
+                multi_pdf.savefig(fig)
+            else:
+                fig.savefig(output_basename + '.pdf')
+        else:
+            fig.canvas.manager.set_window_title('thunderfish')
+            plt.show()
+        plt.close()
+        save_subplots = save_subplots.replace('d', '')
+    if len(save_subplots) > 0:
+        plot_eod_subplots(output_basename, save_subplots, data,
+                          samplerate, idx0, idx1, clipped,
+                          psd_data, wave_eodfs, wave_indices,
+                          mean_eods, eod_props, peak_data,
+                          spec_data, unit, zoom_window, 10, None,
+                          True, skip_bad, log_freq, min_freq,
+                          max_freq, save_plot)
+    return None
+
+                
 def thunderfish(filename, load_kwargs, cfg, channel=0,
                 time=None, time_file=False,
-                mode='wp', log_freq=0.0, save_data=False,
-                all_eods=False, spec_plots='auto', save_plot=False,
-                multi_pdf=None, save_subplots='',
-                output_folder='.', keep_path=False, show_bestwindow=False,
+                mode='wp', log_freq=False, min_freq=0.0, max_freq=3000,
+                save_data=False, zip_file=False,
+                all_eods=False, spec_plots='auto', skip_bad=True,
+                save_plot=False, multi_pdf=None, save_subplots='',
+                output_folder='.', keep_path=False,
                 verbose=0, plot_level=0):
     """Automatically detect and analyze all EOD waveforms in a short recording.
 
     Parameters
     ----------
     filename: string
         Path of the data file to be analyzed.
@@ -1034,24 +1207,35 @@
         "best", or time in seconds (as float or string). If not None
         overwrites "windowPosition" in cofiguration file.
     time_file: bool
         If `True` add time of analysis window to output file names.
     mode: 'w', 'p', 'P', 'wp', or 'wP'
         Analyze wavefish ('w'), all pulse fish ('p'), or largest pulse
         fish only ('P').
-    log_freq: float
-        If not 0 plot spectra with logarithmic frequency axis.
-        Minimum frequency for the logarithmic spectra.
+    log_freq: boolean
+        Logarithmic (True) or linear (False) frequency axis of
+        power spectrum of recording.
+    min_freq: float
+        Limits of frequency axis of power spectrum of recording
+        are set to `(min_freq, max_freq)`, if `max_freq` is greater than zero
+    max_freq: float
+        Limits of frequency axis of power spectrum of recording
+        are set to `(min_freq, max_freq)` and limits of power axis are computed
+        from powers below max_freq, if `max_freq` is greater than zero
     save_data: bool
         If True save analysis results in files. If False, just plot the data.
+    zip_data: bool
+        If True, store all analysis results in a single zip file.
     all_eods: bool
         If True, plot all EOD waveforms.
     spec_plots: bool or 'auto'
         Plot amplitude spectra of EOD waveforms.
         If 'auto', plot them if there is a singel waveform only.
+    skip_bad: bool
+        Skip harmonic groups without index in the spectrum plot.
     save_plot: bool
         If True, save plots as pdf file.
     multi_pdf: matplotlib.PdfPages or None
         PdfPages instance in which to save plots.
     save_subplots: string
         If not empty, specifies subplots to be saved as separate pdf
         files: r) recording with best window, t) data trace with
@@ -1059,16 +1243,14 @@
         fish, w/W) mean EOD waveform, s/S) EOD spectrum, e/E) EOD
         waveform and spectra. Capital letters produce a single
         multipage pdf containing plots of all detected fish.
     output_folder: string
         Folder where to save results.
     keep_path: bool
         Add relative path of data files to output path.
-    show_bestwindow: bool
-        Just show how the best window is determined and exit.
     verbose: int
        Verbosity level (for debugging).
     plot_level: int
        Plot intermediate results.
 
     Returns
     -------
@@ -1078,19 +1260,23 @@
     # check data file:
     if len(filename) == 0:
         return 'you need to specify a file containing some data'
 
     # file names:
     fn = filename if keep_path else os.path.basename(filename)
     outfilename = os.path.splitext(fn)[0]
+    messagefilename = os.path.splitext(fn)[0] + '-message.wav'
+    if not os.path.isfile(messagefilename):
+        messagefilename = None
 
     # load data:
     try:
-        all_data, samplerate, unit = load_data(filename, -1,
-                                               verbose=verbose, **load_kwargs)
+        all_data, samplerate, unit, ampl_max = load_data(filename,
+                                                         verbose=verbose,
+                                                         **load_kwargs)
     except IOError as e:
         return '%s: failed to open file: %s' % (filename, str(e))
     # select channel:
     channels = all_data.shape[1]
     chan_list = [channel]
     if channel < 0:
         chan_list = range(channels)
@@ -1104,18 +1290,17 @@
         if verbose >= 0 and len(chan_list) > 1:
             print('  channel %d' % chan)
 
         # analysis window:
         win_pos = cfg.value('windowPosition')
         if time is not None:
             win_pos = time
-        data, idx0, idx1, clipped, min_clip, max_clip = analysis_window(raw_data, samplerate, win_pos,
-                                                                        cfg, show_bestwindow)
-        if show_bestwindow:
-            return None
+        data, idx0, idx1, clipped, min_clip, max_clip = \
+            analysis_window(raw_data, samplerate, ampl_max, win_pos,
+                            cfg, plot_level>0)
         found_bestwindow = idx1 > 0
         if not found_bestwindow:
             return '%s: not enough data for requested window length. You may want to adjust the windowSize parameter in the configuration file.' % filename
 
         # detect EODs in the data:
         psd_data, wave_eodfs, wave_indices, eod_props, \
         mean_eods, spec_data, peak_data, power_thresh, skip_reason, zoom_window = \
@@ -1125,98 +1310,106 @@
             wave_eodfs = []
             wave_indices = []
             eod_props = []
             mean_eods = []
 
         # add analysis window to EOD properties:
         for props in eod_props:
-            props['tstart'] = idx0/samplerate
-            props['twindow'] = (idx1 - idx0)/samplerate
+            props['twin'] = idx0/samplerate
+            props['window'] = (idx1 - idx0)/samplerate
+            props['winclipped'] = clipped
 
         # warning message in case no fish has been found:
         if found_bestwindow and not eod_props :
             msg = ', '.join(skip_reason)
             if msg:
                 print(filename + ': no fish found: %s' % msg)
             else:
                 print(filename + ': no fish found.')
 
-        # save results to files:
+        # file name for output files:
         output_basename = os.path.join(output_folder, outfilename)
         if channels > 1:
             if channels > 100:
                 output_basename += '-c%03d' % chan
             elif channels > 10:
                 output_basename += '-c%02d' % chan
             else:
                 output_basename += '-c%d' % chan
         if time_file:
             output_basename += '-t%.0fs' % (idx0/samplerate)
+        # make directory if necessary:
+        if keep_path and found_bestwindow:
+            outpath = os.path.dirname(output_basename)
+            if not os.path.exists(outpath):
+                if verbose > 0:
+                    print('mkdir %s' % outpath)
+                os.makedirs(outpath)
+        # save results to files:
         if save_data:
             remove_eod_files(output_basename, verbose, cfg)
             if found_bestwindow:
-                if keep_path:
-                    outpath = os.path.dirname(output_basename)
-                    if not os.path.exists(outpath):
-                        if verbose > 0:
-                            print('mkdir %s' % outpath)
-                        os.makedirs(outpath)
-                save_eods(output_basename, eod_props, mean_eods, spec_data, peak_data,
-                          wave_eodfs, wave_indices, unit, verbose, cfg)
-
+                save_analysis(output_basename, zip_file, eod_props,
+                              mean_eods, spec_data, peak_data,
+                              wave_eodfs, wave_indices, unit, verbose,
+                              **write_table_args(cfg))
+        # summary plots:
         if save_plot or not save_data:
-            min_freq = 0.0
-            max_freq = 3000.0
-            if log_freq > 0.0:
-                min_freq = log_freq
-                max_freq = min_freq*20
-                if max_freq < 2000:
-                    max_freq = 2000
-                log_freq = True
-            else:
-                log_freq = False
             n_snippets = 10
-            chl = chan if channels > 1 else None
-            fig = plot_eods(outfilename, raw_data, samplerate, chl, idx0, idx1, clipped,
-                            psd_data[0], wave_eodfs, wave_indices, mean_eods, eod_props,
-                            peak_data, spec_data, None, unit, zoom_window, n_snippets,
-                            power_thresh, True, all_eods, spec_plots, log_freq, min_freq, max_freq,
-                            interactive=not save_data, verbose=verbose)
-            if save_plot:
-                if multi_pdf is not None:
-                    multi_pdf.savefig(fig)
+            if len(save_subplots) == 0 or 'd' in save_subplots:
+                chl = chan if channels > 1 else None
+                fig = plot_eods(outfilename, messagefilename,
+                                raw_data, samplerate,
+                                chl, idx0, idx1, clipped, psd_data[0],
+                                wave_eodfs, wave_indices, mean_eods,
+                                eod_props, peak_data, spec_data, None,
+                                unit, zoom_window, n_snippets,
+                                power_thresh, True, all_eods,
+                                spec_plots, skip_bad, log_freq,
+                                min_freq, max_freq, interactive=not
+                                save_plot, verbose=verbose)
+                if save_plot:
+                    if multi_pdf is not None:
+                        multi_pdf.savefig(fig)
+                    else:
+                        fig.savefig(output_basename + '.pdf')
                 else:
-                    # save figure as pdf:
-                    fig.savefig(output_basename + '.pdf')
-                    plt.close('all')
-                if len(save_subplots) > 0:
-                    plot_eod_subplots(output_basename, save_subplots,
-                                      raw_data, samplerate, idx0, idx1, clipped, psd_data[0],
-                                      wave_eodfs, wave_indices, mean_eods, eod_props,
-                                      peak_data, spec_data, unit, zoom_window, n_snippets,
-                                      power_thresh, True, log_freq, min_freq, max_freq)
-            elif not save_data:
-                fig.canvas.set_window_title('thunderfish')
-                plt.show()
+                    fig.canvas.manager.set_window_title('thunderfish')
+                    plt.show()
+                plt.close()
+                save_subplots = save_subplots.replace('d', '')
+            if len(save_subplots) > 0:
+                plot_eod_subplots(output_basename, save_subplots,
+                                  raw_data, samplerate, idx0, idx1,
+                                  clipped, psd_data[0], wave_eodfs,
+                                  wave_indices, mean_eods, eod_props,
+                                  peak_data, spec_data, unit,
+                                  zoom_window, n_snippets,
+                                  power_thresh, True, skip_bad,
+                                  log_freq, min_freq, max_freq,
+                                  save_plot)
     return None
 
 
 def run_thunderfish(file_args):
+    """Helper function for mutlithreading Pool().map().
     """
-    Helper function for mutlithreading Pool().map().
-    """
-    verbose = file_args[1][-2]+1
-    if verbose > 0:
-        if verbose > 1:
-            print('='*70)
-        print('analyze recording %s ...' % file_args[0])
+    results = file_args[1][0]
+    verbose = file_args[1][-1] if results else file_args[1][-2]+1
+    if verbose > 1:
+        print('='*70)
     try:
-        msg = thunderfish(file_args[0], *file_args[1])
-        if msg:
-            print(msg)
+        if results:
+            thunderfish_plot(file_args[0], *file_args[1][1:])
+        else:
+            if verbose > 0:
+                print('analyze recording %s ...' % file_args[0])
+            msg = thunderfish(file_args[0], *file_args[1][1:])
+            if msg:
+                print(msg)
     except (KeyboardInterrupt, SystemExit):
         print('\nthunderfish interrupted by user... exit now.')
         sys.exit(0)
     except:
         print(traceback.format_exc())
 
 
@@ -1239,48 +1432,54 @@
                         help='level for debugging plots. Increase by specifying -V multiple times, or like -VVV')
     parser.add_argument('-c', dest='save_config', action='store_true',
                         help='save configuration to file {0} after reading all configuration files'.format(cfgfile))
     parser.add_argument('--channel', default=0, type=int,
                         help='channel to be analyzed (defaults to first channel, negative channel selects all channels)')
     parser.add_argument('-t', dest='time', default=None, type=str, metavar='TIME',
                         help='start time of analysis window in recording: "beginning", "center", "end", "best", or time in seconds (overwrites "windowPosition" in cofiguration file)')
+    parser.add_argument('-u', dest='unwrap', action='store_true',
+                        help='unwrap clipped files, toggles unwrap setting of config file.')
     parser.add_argument('-T', dest='time_file', action='store_true',
                         help='add start time of analysis file to output file names')
     parser.add_argument('-m', dest='mode', default='wp', type=str,
                         choices=['w', 'p', 'wp'],
                         help='extract wave "w" and/or pulse "p" fish EODs')
     parser.add_argument('-a', dest='all_eods', action='store_true',
-                        help='plot all EOD waveforms')
+                        help='show all EOD waveforms in the summary plot')
     parser.add_argument('-S', dest='spec_plots', action='store_true',
-                        help='plot spectra for all EOD waveforms')
+                        help='plot spectra for all EOD waveforms in the summary plot')
+    parser.add_argument('-b', dest='skip_bad', action='store_false',
+                        help='indicate bad EODs in legend of power spectrum')
+    parser.add_argument('-l', dest='log_freq', type=float, metavar='MINFREQ',
+                        nargs='?', const=100.0, default=0.0,
+                        help='logarithmic frequency axis in  power spectrum with optional minimum frequency (defaults to 100 Hz)')
+    parser.add_argument('-p', dest='save_plot', action='store_true',
+                        help='save output plots as pdf files')
+    parser.add_argument('-M', dest='multi_pdf', default='', type=str, metavar='PDFFILE',
+                        help='save all summary plots of all recordings in a multi page pdf file. Disables parallel jobs.')
+    parser.add_argument('-P', dest='save_subplots', default='', type=str, metavar='rtpwsed',
+                        help='save subplots as separate pdf files: r) recording with analysis window, t) data trace with detected pulse fish, p) power spectrum with detected wave fish, w/W) mean EOD waveform, s/S) EOD spectrum, e/E) EOD waveform and spectra, d) the default summary plot. Capital letters produce a single multipage pdf containing plots of all detected fish')
+    parser.add_argument('-d', dest='rawdata_path', default='.', type=str, metavar='PATH',
+                        help='path to raw EOD recordings needed for plotting based on analysis results')
     parser.add_argument('-j', dest='jobs', nargs='?', type=int, default=None, const=0,
                         help='number of jobs run in parallel. Without argument use all CPU cores.')
     parser.add_argument('-s', dest='save_data', action='store_true',
                         help='save analysis results to files')
+    parser.add_argument('-z', dest='zip_file', action='store_true',
+                        help='save analysis results in a single zip file')
     parser.add_argument('-f', dest='format', default='auto', type=str,
                         choices=TableData.formats + ['py'],
                         help='file format used for saving analysis results, defaults to the format specified in the configuration file or "csv"')
-    parser.add_argument('-p', dest='save_plot', action='store_true',
-                        help='save output plot of each recording as pdf file')
-    parser.add_argument('-P', dest='save_subplots', default='', type=str, metavar='rtpwse',
-                        help='save subplots as separate pdf files: r) recording with best window, t) data trace with detected pulse fish, p) power spectrum with detected wave fish, w/W) mean EOD waveform, s/S) EOD spectrum, e/E) EOD waveform and spectra. Capital letters produce a single multipage pdf containing plots of all detected fish')
-    parser.add_argument('-M', dest='multi_pdf', default='', type=str, metavar='PDFFILE',
-                        help='save all plots of all recordings in a multi pages pdf file. Disables parallel jobs.')
-    parser.add_argument('-l', dest='log_freq', type=float, metavar='MINFREQ',
-                        nargs='?', const=100.0, default=0.0,
-                        help='logarithmic frequency axis in  power spectrum with optional minimum frequency (defaults to 100 Hz)')
     parser.add_argument('-o', dest='outpath', default='.', type=str,
                         help='path where to store results and figures (defaults to current working directory)')
     parser.add_argument('-k', dest='keep_path', action='store_true',
                         help='keep path of input file when saving analysis files, i.e. append path of input file to OUTPATH')
     parser.add_argument('-i', dest='load_kwargs', default=[],
                         action='append', metavar='KWARGS',
                         help='key-word arguments for the data loader function')
-    parser.add_argument('-b', dest='show_bestwindow', action='store_true',
-                        help='show the cost function of the best window algorithm')
     parser.add_argument('file', nargs='*', default='', type=str,
                         help='name of a file with time series data of an EOD recording, may include wildcards')
     args = parser.parse_args(cargs)
 
     # help:
     if args.help:
         parser.print_help()
@@ -1299,51 +1498,53 @@
         print('- write configuration file:')
         print('  > thunderfish -c')
         parser.exit()
 
     # set verbosity level from command line:
     verbose = args.verbose
     plot_level = args.plot_level
-    if verbose < plot_level+1:
-        verbose = plot_level+1
+    if verbose < plot_level:
+        verbose = plot_level
 
     # interactive plot:
     plt.rcParams['keymap.quit'] = 'ctrl+w, alt+q, q'
     plt.ioff()
 
     # expand wildcard patterns:
     files = []
     if os.name == 'nt':
         for fn in args.file:
             files.extend(glob.glob(fn))
     else:
-        files = args.file
+        files = [f for f in args.file if '-message' not in f]
 
+    # save configuration:
     if args.save_config:
-        # save configuration:
         file_name = files[0] if len(files) else ''
         cfg = configuration()
         cfg.load_files(cfgfile, file_name, 4, verbose)
         save_configuration(cfg, cfgfile)
         exit()
     elif len(files) == 0:
         parser.error('you need to specify at least one file for the analysis')
 
     # configure:
     cfg = configuration()
     cfg.load_files(cfgfile, files[0], 4, verbose)
     if args.format != 'auto':
         cfg.set('fileFormat', args.format)
+    if args.unwrap:
+        cfg.set('unwrapData', not cfg.value('unwrapData'))
         
-    # save plots:
+    # plot parameter:
     spec_plots = 'auto'
     if args.spec_plots:
         spec_plots = True
-    if len(args.save_subplots) > 0:
-        args.save_plot = True
+
+    # multi-page pdfs:
     multi_pdf = None
     if len(args.multi_pdf) > 0:
         args.save_plot = True
         args.jobs = None  # PdfPages does not work yet with mutliprocessing
         ext = os.path.splitext(args.multi_pdf)[1]
         if ext != os.extsep + 'pdf':
             args.multi_pdf += os.extsep + 'pdf'
@@ -1352,28 +1553,72 @@
     # create output folder:
     if args.save_data or args.save_plot:
         if not os.path.exists(args.outpath):
             if verbose > 1:
                 print('mkdir %s' % args.outpath)
             os.makedirs(args.outpath)
 
-    # kwargs fro data loader:
+    # kwargs for data loader:
     load_kwargs = {}
     for s in args.load_kwargs:
         for kw in s.split(','):
             kws = kw.split(':')
             if len(kws) == 2:
                 load_kwargs[kws[0].strip()] = kws[1].strip()
-            
+
+    # frequency limits for power spectrum:
+    min_freq = 0.0
+    max_freq = 3000.0
+    log_freq = args.log_freq
+    if log_freq > 0.0:
+        min_freq = log_freq
+        max_freq = min_freq*20
+        if max_freq < 2000:
+            max_freq = 2000
+        log_freq = True
+    else:
+        log_freq = False
+
+    # check if all input files are results:
+    exts = TableData.ext_formats.values()
+    results = True
+    # check and group by recording:
+    result_files = []
+    for f in sorted(files):
+        _, base_name, _, _, ftype, _, ext = parse_filename(f)
+        if ext == 'zip' or (ext in exts and ftype in file_types):
+            if len(result_files) == 0 or \
+               not result_files[-1][-1].startswith(base_name):
+                result_files.append([f])
+            else:
+                result_files[-1].append(f)
+        else:
+            results = False
+            break
+    if results:
+        files = result_files
+
+    # adjust verbosity:
+    v = verbose
+    if len(files) > 1:
+        v += 1
+    
     # run on pool:
-    pool_args = (load_kwargs, cfg, args.channel, args.time, args.time_file,
-                 args.mode, args.log_freq, args.save_data,
-                 args.all_eods, spec_plots, args.save_plot, multi_pdf,
-                 args.save_subplots, args.outpath, args.keep_path,
-                 args.show_bestwindow, verbose-1, plot_level)
+    pool_args = (results, load_kwargs, cfg, args.channel, args.time,
+                 args.time_file, args.mode, log_freq, min_freq,
+                 max_freq, args.save_data, args.zip_file,
+                 args.all_eods, spec_plots, args.skip_bad,
+                 args.save_plot, multi_pdf, args.save_subplots,
+                 args.outpath, args.keep_path, v-1, plot_level)
+    if results:
+        pool_args = (results, args.rawdata_path, load_kwargs,
+                     args.all_eods, spec_plots, args.skip_bad,
+                     args.save_plot, multi_pdf, args.save_subplots,
+                     log_freq, min_freq, max_freq, args.outpath,
+                     args.keep_path, v)
     if args.jobs is not None and (args.save_data or args.save_plot) and len(files) > 1:
         cpus = cpu_count() if args.jobs == 0 else args.jobs
         if verbose > 1:
             print('run on %d cpus' % cpus)
         p = Pool(cpus)
         p.map(run_thunderfish, zip(files, [pool_args]*len(files)))
     else:
```

### Comparing `thunderfish-1.9.9/thunderfish/thunderlogger.py` & `thunderfish-2.0.0/src/thunderfish/thunderlogger.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 import datetime as dt
 import numpy as np
 import pandas as pd
 from scipy.signal import butter, lfilter
 from types import SimpleNamespace
 import matplotlib.pyplot as plt
 import matplotlib.dates as mdates
+from thunderlab.configfile import ConfigFile
+from thunderlab.dataloader import DataLoader
+from thunderlab.tabledata import TableData, write_table_args
+from thunderlab.eventdetection import hist_threshold
 from .version import __version__, __year__
-from .configfile import ConfigFile
-from .dataloader import DataLoader
-from .tabledata import TableData, write_table_args
-from .eventdetection import hist_threshold
 from .eodanalysis import save_eod_waveform, save_wave_fish, save_pulse_fish
 from .eodanalysis import save_wave_spectrum, save_pulse_spectrum, save_pulse_peaks
 from .eodanalysis import load_eod_waveform, load_wave_fish, load_pulse_fish
 from .eodanalysis import load_wave_spectrum, load_pulse_spectrum, load_pulse_peaks
 from .eodanalysis import wave_similarity, pulse_similarity
 from .thunderfish import configuration, save_configuration
 from .thunderfish import detect_eods, remove_eod_files
@@ -139,16 +139,16 @@
                                             fish = wfish
                                     if fish_deltaf > max_deltaf:
                                         fish = None
                                     peaks = None
                                 else:
                                     fish_dist = 10000.0
                                     for pfish in pulse_fishes[channel]:
-                                        ddist = np.abs(pfish.props['dist'] -
-                                                       props['dist'])
+                                        ddist = np.abs(pfish.props['P1-P1-dist'] -
+                                                       props['P1-P1-dist'])
                                         if ddist < fish_dist:
                                             fish_dist = ddist
                                             fish_deltaf = np.abs(pfish.props['EODf'] -
                                                                  props['EODf'])
                                             fish = pfish
                                     if fish_dist > max_dist or \
                                        fish_deltaf > max_deltaf:
@@ -219,21 +219,21 @@
     if idx is not None:
         fp += '-%d' % idx
     td.write(fp, **kwargs)
     
 
 def load_times(file_path):
     data = TableData(file_path).data_frame()
-    data['index'] = data['index'].astype(np.int)
+    data['index'] = data['index'].astype(int)
     data['tstart'] = pd.to_datetime(data['tstart'])
     data['tstart'] = pd.Series(data['tstart'].dt.to_pydatetime(), dtype=object)
     data['tend'] = pd.to_datetime(data['tend'])
     data['tend'] = pd.Series(data['tend'].dt.to_pydatetime(), dtype=object)
     if 'channel' in data:
-        data['channel'] = data['channel'].astype(np.int)
+        data['channel'] = data['channel'].astype(int)
     return data
 
 
 def save_power(times, stds, supra_thresh, unit, output_basename, **kwargs):
     td = TableData()
     td.append('index', '', '%d', list(range(len(times))))
     td.append('time', '', '%s',
@@ -255,15 +255,15 @@
                                           '%Y-%m-%dT%H:%M:%S'))
     if start_time is not None:
         deltat = start_time - times[0]
         for k in range(len(times)):
             times[k] += deltat
     channels = (data.columns()-2)//2
     stds = np.zeros((len(times), channels))
-    supra_thresh = np.zeros((len(times), channels), dtype=np.int)
+    supra_thresh = np.zeros((len(times), channels), dtype=int)
     for c in range(channels):
         stds[:,c] = data[:,'channel%d'%c]
         supra_thresh[:,c] = data[:,'thresh%d'%c]
     return np.array(times), stds, supra_thresh, device
 
 
 def save_data(output_folder, name, pulse_fishes, wave_fishes,
```

