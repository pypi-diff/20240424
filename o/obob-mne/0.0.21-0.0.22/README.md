# Comparing `tmp/obob_mne-0.0.21.tar.gz` & `tmp/obob_mne-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obob_mne-0.0.21.tar", last modified: Wed Jan 10 12:56:26 2024, max compression
+gzip compressed data, was "obob_mne-0.0.22.tar", last modified: Wed Apr 24 13:58:19 2024, max compression
```

## Comparing `obob_mne-0.0.21.tar` & `obob_mne-0.0.22.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-01-10 12:56:26.519334 obob_mne-0.0.21/
--rw-r--r--   0 th        (1011) th        (1011)    35097 2022-06-23 07:45:12.000000 obob_mne-0.0.21/LICENSE
--rw-r--r--   0 th        (1011) th        (1011)       49 2022-06-23 07:45:12.000000 obob_mne-0.0.21/MANIFEST.in
--rw-r--r--   0 th        (1011) th        (1011)      412 2024-01-10 12:56:26.519334 obob_mne-0.0.21/PKG-INFO
--rw-r--r--   0 th        (1011) th        (1011)       81 2022-06-23 07:45:12.000000 obob_mne-0.0.21/README.md
--rw-r--r--   0 th        (1011) th        (1011)        6 2024-01-10 12:56:17.000000 obob_mne-0.0.21/VERSION
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-01-10 12:56:26.516334 obob_mne-0.0.21/obob_mne/
--rw-r--r--   0 th        (1011) th        (1011)      870 2022-06-23 07:45:12.000000 obob_mne-0.0.21/obob_mne/__init__.py
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-01-10 12:56:26.517334 obob_mne-0.0.21/obob_mne/decoding/
--rw-r--r--   0 th        (1011) th        (1011)     1048 2022-06-23 07:45:12.000000 obob_mne-0.0.21/obob_mne/decoding/__init__.py
--rw-r--r--   0 th        (1011) th        (1011)    25330 2024-01-10 12:55:44.000000 obob_mne-0.0.21/obob_mne/decoding/gentemporal.py
--rw-r--r--   0 th        (1011) th        (1011)     1180 2022-06-23 07:45:12.000000 obob_mne-0.0.21/obob_mne/decoding/helpers.py
--rw-r--r--   0 th        (1011) th        (1011)     9036 2022-06-23 07:45:12.000000 obob_mne-0.0.21/obob_mne/decoding/temporal.py
--rw-r--r--   0 th        (1011) th        (1011)     4065 2022-06-23 08:42:16.000000 obob_mne-0.0.21/obob_mne/epochs.py
--rw-r--r--   0 th        (1011) th        (1011)     2367 2022-06-23 08:42:16.000000 obob_mne-0.0.21/obob_mne/events.py
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-01-10 12:56:26.518334 obob_mne-0.0.21/obob_mne/mixins/
--rw-r--r--   0 th        (1011) th        (1011)      807 2022-06-23 07:45:12.000000 obob_mne-0.0.21/obob_mne/mixins/__init__.py
--rw-r--r--   0 th        (1011) th        (1011)    13392 2024-01-10 08:50:00.000000 obob_mne-0.0.21/obob_mne/mixins/raw.py
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-01-10 12:56:26.518334 obob_mne-0.0.21/obob_mne/mri/
--rw-r--r--   0 th        (1011) th        (1011)      807 2022-06-23 07:45:12.000000 obob_mne-0.0.21/obob_mne/mri/__init__.py
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-01-10 12:56:26.518334 obob_mne-0.0.21/obob_mne/mri/cmd/
--rw-r--r--   0 th        (1011) th        (1011)      807 2022-06-23 07:45:12.000000 obob_mne-0.0.21/obob_mne/mri/cmd/__init__.py
--rw-r--r--   0 th        (1011) th        (1011)     1444 2022-06-23 07:45:12.000000 obob_mne-0.0.21/obob_mne/mri/cmd/import_subject.py
--rw-r--r--   0 th        (1011) th        (1011)     3516 2022-06-23 07:45:12.000000 obob_mne-0.0.21/obob_mne/mri/cmd/make_freesurfer_bem.py
--rw-r--r--   0 th        (1011) th        (1011)     2960 2022-06-23 07:45:12.000000 obob_mne-0.0.21/obob_mne/mri/cmd/make_source_space.py
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-01-10 12:56:26.519334 obob_mne-0.0.21/obob_mne/mri/cmd/utils/
--rw-r--r--   0 th        (1011) th        (1011)      807 2022-06-23 07:45:12.000000 obob_mne-0.0.21/obob_mne/mri/cmd/utils/__init__.py
--rw-r--r--   0 th        (1011) th        (1011)     1632 2022-06-23 07:45:12.000000 obob_mne-0.0.21/obob_mne/mri/cmd/utils/jobs.py
--rw-r--r--   0 th        (1011) th        (1011)      958 2022-06-23 07:45:12.000000 obob_mne-0.0.21/obob_mne/raw.py
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-01-10 12:56:26.519334 obob_mne-0.0.21/obob_mne.egg-info/
--rw-r--r--   0 th        (1011) th        (1011)      412 2024-01-10 12:56:26.000000 obob_mne-0.0.21/obob_mne.egg-info/PKG-INFO
--rw-r--r--   0 th        (1011) th        (1011)      771 2024-01-10 12:56:26.000000 obob_mne-0.0.21/obob_mne.egg-info/SOURCES.txt
--rw-r--r--   0 th        (1011) th        (1011)        1 2024-01-10 12:56:26.000000 obob_mne-0.0.21/obob_mne.egg-info/dependency_links.txt
--rw-r--r--   0 th        (1011) th        (1011)      278 2024-01-10 12:56:26.000000 obob_mne-0.0.21/obob_mne.egg-info/entry_points.txt
--rw-r--r--   0 th        (1011) th        (1011)       35 2024-01-10 12:56:26.000000 obob_mne-0.0.21/obob_mne.egg-info/requires.txt
--rw-r--r--   0 th        (1011) th        (1011)       15 2024-01-10 12:56:26.000000 obob_mne-0.0.21/obob_mne.egg-info/top_level.txt
--rw-r--r--   0 th        (1011) th        (1011)      444 2024-01-10 12:56:26.520334 obob_mne-0.0.21/setup.cfg
--rw-r--r--   0 th        (1011) th        (1011)     2138 2022-06-23 08:42:16.000000 obob_mne-0.0.21/setup.py
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-01-10 12:56:26.519334 obob_mne-0.0.21/tests/
--rw-r--r--   0 th        (1011) th        (1011)      809 2022-06-23 07:45:12.000000 obob_mne-0.0.21/tests/__init__.py
--rw-r--r--   0 th        (1011) th        (1011)      844 2022-06-23 07:45:12.000000 obob_mne-0.0.21/tests/test_example.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-24 13:58:19.269445 obob_mne-0.0.22/
+-rw-r--r--   0 th        (1011) th        (1011)    35097 2022-06-23 07:45:12.000000 obob_mne-0.0.22/LICENSE
+-rw-r--r--   0 th        (1011) th        (1011)       49 2022-06-23 07:45:12.000000 obob_mne-0.0.22/MANIFEST.in
+-rw-r--r--   0 th        (1011) th        (1011)      412 2024-04-24 13:58:19.269445 obob_mne-0.0.22/PKG-INFO
+-rw-r--r--   0 th        (1011) th        (1011)       81 2022-06-23 07:45:12.000000 obob_mne-0.0.22/README.md
+-rw-r--r--   0 th        (1011) th        (1011)        6 2024-04-24 13:58:15.000000 obob_mne-0.0.22/VERSION
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-24 13:58:19.258445 obob_mne-0.0.22/obob_mne/
+-rw-r--r--   0 th        (1011) th        (1011)      870 2022-06-23 07:45:12.000000 obob_mne-0.0.22/obob_mne/__init__.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-24 13:58:19.264445 obob_mne-0.0.22/obob_mne/decoding/
+-rw-r--r--   0 th        (1011) th        (1011)     1048 2022-06-23 07:45:12.000000 obob_mne-0.0.22/obob_mne/decoding/__init__.py
+-rw-r--r--   0 th        (1011) th        (1011)    25297 2024-04-24 13:54:40.000000 obob_mne-0.0.22/obob_mne/decoding/gentemporal.py
+-rw-r--r--   0 th        (1011) th        (1011)     1180 2022-06-23 07:45:12.000000 obob_mne-0.0.22/obob_mne/decoding/helpers.py
+-rw-r--r--   0 th        (1011) th        (1011)     9036 2022-06-23 07:45:12.000000 obob_mne-0.0.22/obob_mne/decoding/temporal.py
+-rw-r--r--   0 th        (1011) th        (1011)     4066 2024-04-24 13:54:55.000000 obob_mne-0.0.22/obob_mne/epochs.py
+-rw-r--r--   0 th        (1011) th        (1011)     2403 2024-04-24 13:55:33.000000 obob_mne-0.0.22/obob_mne/events.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-24 13:58:19.264445 obob_mne-0.0.22/obob_mne/mixins/
+-rw-r--r--   0 th        (1011) th        (1011)      807 2022-06-23 07:45:12.000000 obob_mne-0.0.22/obob_mne/mixins/__init__.py
+-rw-r--r--   0 th        (1011) th        (1011)    14590 2024-04-24 13:57:20.000000 obob_mne-0.0.22/obob_mne/mixins/raw.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-24 13:58:19.265445 obob_mne-0.0.22/obob_mne/mri/
+-rw-r--r--   0 th        (1011) th        (1011)      807 2022-06-23 07:45:12.000000 obob_mne-0.0.22/obob_mne/mri/__init__.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-24 13:58:19.266445 obob_mne-0.0.22/obob_mne/mri/cmd/
+-rw-r--r--   0 th        (1011) th        (1011)      807 2022-06-23 07:45:12.000000 obob_mne-0.0.22/obob_mne/mri/cmd/__init__.py
+-rw-r--r--   0 th        (1011) th        (1011)     1444 2022-06-23 07:45:12.000000 obob_mne-0.0.22/obob_mne/mri/cmd/import_subject.py
+-rw-r--r--   0 th        (1011) th        (1011)     3516 2022-06-23 07:45:12.000000 obob_mne-0.0.22/obob_mne/mri/cmd/make_freesurfer_bem.py
+-rw-r--r--   0 th        (1011) th        (1011)     2960 2022-06-23 07:45:12.000000 obob_mne-0.0.22/obob_mne/mri/cmd/make_source_space.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-24 13:58:19.267445 obob_mne-0.0.22/obob_mne/mri/cmd/utils/
+-rw-r--r--   0 th        (1011) th        (1011)      807 2022-06-23 07:45:12.000000 obob_mne-0.0.22/obob_mne/mri/cmd/utils/__init__.py
+-rw-r--r--   0 th        (1011) th        (1011)     1632 2022-06-23 07:45:12.000000 obob_mne-0.0.22/obob_mne/mri/cmd/utils/jobs.py
+-rw-r--r--   0 th        (1011) th        (1011)      958 2022-06-23 07:45:12.000000 obob_mne-0.0.22/obob_mne/raw.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-24 13:58:19.267445 obob_mne-0.0.22/obob_mne.egg-info/
+-rw-r--r--   0 th        (1011) th        (1011)      412 2024-04-24 13:58:19.000000 obob_mne-0.0.22/obob_mne.egg-info/PKG-INFO
+-rw-r--r--   0 th        (1011) th        (1011)      771 2024-04-24 13:58:19.000000 obob_mne-0.0.22/obob_mne.egg-info/SOURCES.txt
+-rw-r--r--   0 th        (1011) th        (1011)        1 2024-04-24 13:58:19.000000 obob_mne-0.0.22/obob_mne.egg-info/dependency_links.txt
+-rw-r--r--   0 th        (1011) th        (1011)      278 2024-04-24 13:58:19.000000 obob_mne-0.0.22/obob_mne.egg-info/entry_points.txt
+-rw-r--r--   0 th        (1011) th        (1011)       35 2024-04-24 13:58:19.000000 obob_mne-0.0.22/obob_mne.egg-info/requires.txt
+-rw-r--r--   0 th        (1011) th        (1011)       15 2024-04-24 13:58:19.000000 obob_mne-0.0.22/obob_mne.egg-info/top_level.txt
+-rw-r--r--   0 th        (1011) th        (1011)      444 2024-04-24 13:58:19.271445 obob_mne-0.0.22/setup.cfg
+-rw-r--r--   0 th        (1011) th        (1011)     2138 2022-06-23 08:42:16.000000 obob_mne-0.0.22/setup.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-24 13:58:19.267445 obob_mne-0.0.22/tests/
+-rw-r--r--   0 th        (1011) th        (1011)      809 2022-06-23 07:45:12.000000 obob_mne-0.0.22/tests/__init__.py
+-rw-r--r--   0 th        (1011) th        (1011)      844 2022-06-23 07:45:12.000000 obob_mne-0.0.22/tests/test_example.py
```

### Comparing `obob_mne-0.0.21/LICENSE` & `obob_mne-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.21/obob_mne/__init__.py` & `obob_mne-0.0.22/obob_mne/__init__.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.21/obob_mne/decoding/__init__.py` & `obob_mne-0.0.22/obob_mne/decoding/__init__.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.21/obob_mne/decoding/gentemporal.py` & `obob_mne-0.0.22/obob_mne/decoding/gentemporal.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import numpy
 import copy
 import logging
 import collections
 import scipy.stats
 
 from .temporal import TemporalArray
-from.helpers import _get_Y_from_metadata
+from .helpers import _get_Y_from_metadata
 
 
 class GeneralizedTemporalArray(mne.utils.SizeMixin):
     """Base class for Temporal Generalization Decoding.
 
     Parameters
     ----------
@@ -217,15 +217,16 @@
         axes.set_xlabel(xlabel)
         axes.set_ylabel(ylabel)
         axes.set_title('Temporal Generalization')
         axes.axvline(0, color='k')
         axes.axhline(0, color='k')
         old_xlim = axes.get_xlim()
         old_ylim = axes.get_ylim()
-        diag = (min(self._times_testing[0], self._times_training[0]), max(self._times_testing[-1], self._times_training[-1]))
+        diag = (min(self._times_testing[0], self._times_training[0]),
+                max(self._times_testing[-1], self._times_training[-1]))
         axes.plot(diag, diag, color='k')
         axes.set_xlim(old_xlim)
         axes.set_ylim(old_ylim)
         if colorbar:
             plt.colorbar(im, ax=axes)
 
         if show:
@@ -253,15 +254,15 @@
             If True, values below chance level get masked.
         interpolation : str, optional
             The interpolation method used.
         """
         scores = self.scores
 
         alpha = numpy.ones_like(scores)
-        
+
         if mask_below_chance:
             mask = scores < self.chance_level
             alpha[mask] = insignificant_alpha
 
         return self._plot_image(values=scores, axes=axes, show=show, cmap=cmap,
                                 colorbar=colorbar, interpolation=interpolation,
                                 alpha=alpha)
@@ -280,38 +281,36 @@
 
         self._info = mne.pick_info(self.info, good_channels_idx)
         self._weights = self._weights[good_channels_idx, :]
 
     def crop(self, tmin_training=None, tmax_training=None,
              tmin_testing=None, tmax_testing=None):
         """Crop to times
-        
+
         """
         if tmin_training is None:
             tmin_training = self._times_training[0]
         if tmax_training is None:
             tmax_training = self._times_training[-1]
 
         if tmin_testing is None:
             tmin_testing = self._times_testing[0]
         if tmax_testing is None:
             tmax_testing = self._times_testing[-1]
 
-        
         time_idx_training = numpy.where(
             numpy.logical_and(
                 self._times_training >= tmin_training,
                 self._times_training <= tmax_training))[0]
-        
+
         time_idx_testing = numpy.where(
             numpy.logical_and(
                 self._times_testing >= tmin_testing,
                 self._times_testing <= tmax_testing))[0]
-        
-        
+
         if self._scores_raw.ndim == 2:
             self._scores_raw = self._scores_raw[time_idx_training, :]
             self._scores_raw = self._scores_raw[:, time_idx_testing]
             if self._weights is not None:
                 self._weights = self._weights[time_idx_training, :]
                 self._weights = self._weights[:, time_idx_testing]
         else:
@@ -416,15 +415,15 @@
 
     """
 
     def __init__(self, data_list):
         self._equalize_channels(data_list)
 
         if None not in [x._weights for x in data_list]:
-            weights = numpy.average(numpy.stack([x._weights for x in data_list]),
+            weights = numpy.average(numpy.stack([x._weights for x in data_list]),  # noqa
                                     axis=0)
         else:
             weights = None
 
         scores_raw = numpy.average(
             numpy.stack([x._scores_raw for x in data_list]), axis=0)
 
@@ -476,15 +475,15 @@
             The interpolation method used.
         mask_p : float or None, optional
             If set, the plot is masked for the given p-value.
         """
         scores = self.scores
 
         alpha = numpy.ones_like(scores)
-        
+
         if mask_below_chance:
             mask = scores < self.chance_level
             alpha[mask] = insignificant_alpha
 
         if mask_p is not None:
             mask = self.p > mask_p
             alpha[mask] = insignificant_alpha
```

### Comparing `obob_mne-0.0.21/obob_mne/decoding/helpers.py` & `obob_mne-0.0.22/obob_mne/decoding/helpers.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.21/obob_mne/decoding/temporal.py` & `obob_mne-0.0.22/obob_mne/decoding/temporal.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.21/obob_mne/epochs.py` & `obob_mne-0.0.22/obob_mne/epochs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -123,8 +123,8 @@
     data = scipy.stats.zscore(data, 1)
 
     data = data.reshape(original_shape)
     data = data.swapaxes(0, 1)
 
     epoch._data = data
 
-    return epoch
+    return epoch
```

### Comparing `obob_mne-0.0.21/obob_mne/events.py` & `obob_mne-0.0.22/obob_mne/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,18 @@
     new_event_id = {key: value for key, value in event_id.items() if
                     key in good_event_keys}
     return new_event_id
 
 
 def read_events_from_analogue(raw, tolerance=1, trigger_channels=None):
     if trigger_channels is None:
-        trigger_channels = ['STI001', 'STI002', 'STI003', 'STI004', 'STI005', 'STI006', 'STI007', 'STI008']
+        trigger_channels = ['STI001', 'STI002', 'STI003',
+                            'STI004', 'STI005', 'STI006', 'STI007', 'STI008']
 
-    trigger_data = raw[mne.pick_channels(raw.ch_names, trigger_channels)][0] / 5
+    trigger_data = raw[mne.pick_channels(raw.ch_names, trigger_channels)][0] / 5  # noqa
 
     bit_mult = 2 ** np.arange(0, trigger_data.shape[0])
 
     trigger_values = np.sum((trigger_data.T * bit_mult).T, axis=0).astype(int)
 
     trigger_idx = np.where(np.diff(trigger_values) > 0)[0] + 1
     tmp_events = np.zeros((trigger_idx.shape[0], 3))
```

### Comparing `obob_mne-0.0.21/obob_mne/mixins/__init__.py` & `obob_mne-0.0.22/obob_mne/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.21/obob_mne/mixins/raw.py` & `obob_mne-0.0.22/obob_mne/mixins/raw.py`

 * *Files 6% similar despite different names*

```diff
@@ -175,31 +175,32 @@
                     raise ValueError(
                         'Subject %s is excluded!' % (cur_subject_id,))
 
             for cur_glob_pattern in cls.file_glob_patterns:
                 tmp_result = glob.glob(
                     os.path.join(
                         study_folder, '*', '*',
-                        cls.get_glob_pattern(cur_glob_pattern, cur_subject_id, run_nr)
+                        cls.get_glob_pattern(
+                            cur_glob_pattern, cur_subject_id, run_nr
                         )
+                    )
                 )
                 if tmp_result:
                     fname = tmp_result[-1]
 
         return fname
 
     @classmethod
     def get_glob_pattern(cls, cur_glob_pattern, cur_subject_id, run_nr):
         if run_nr is not None:
             return cur_glob_pattern % (cur_subject_id, run_nr)
         else:
             return cur_glob_pattern % (cur_subject_id, )
 
 
-
 class AdvancedEvents(mne.io.fiff.Raw):
     """Integrate event loading and handling into :class:`mne.io.Raw`.
 
     Including this mixin in your study specific ``Raw`` class provides event
     handling features directly in that class.
 
     More specifically, it provides three extra properties:
@@ -413,10 +414,43 @@
             cur_metadata = deepcopy(conditions_metadata)
             for stim_group_name, stim_group_choices in \
                     self.stimulus_triggers.items():
                 cur_metadata[stim_group_name] = self._decode_bin_trigger(
                     cur_evt_code, stim_group_choices
                 )
 
+            all_raw_metadata.append(cur_metadata)
+
+        self._evt_metadata = pd.DataFrame(all_raw_metadata)
+
+
+class AutomaticBinaryEventsWithMetadata(AutomaticBinaryEvents):
+    """Mixin for binary events with metadata.
+
+    """
+    def _process_events(self):
+        super(AutomaticBinaryEvents, self)._process_events()
+
+        conditions_metadata = {}
+        all_raw_metadata = []
+
+        if self.condition_triggers:
+            condition_trigger = self._events[0, 2]
+            self._events = np.delete(self._events, (0), axis=0)
+
+            for allcond_key, allcond_value in self.condition_triggers.items():
+                conditions_metadata[allcond_key] = self._decode_bin_trigger(
+                    condition_trigger,
+                    allcond_value
+                )
+
+        for cur_evt_code in self._events[:, 2]:
+            cur_metadata = deepcopy(conditions_metadata)
+            for stim_group_name, stim_group_choices in \
+                    self.stimulus_triggers.items():
+                cur_metadata[stim_group_name] = self._decode_bin_trigger(
+                    cur_evt_code, stim_group_choices
+                )
+
             all_raw_metadata.append(cur_metadata)
 
         self._evt_metadata = pd.DataFrame(all_raw_metadata)
```

### Comparing `obob_mne-0.0.21/obob_mne/mri/__init__.py` & `obob_mne-0.0.22/obob_mne/mri/__init__.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.21/obob_mne/mri/cmd/__init__.py` & `obob_mne-0.0.22/obob_mne/mri/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.21/obob_mne/mri/cmd/import_subject.py` & `obob_mne-0.0.22/obob_mne/mri/cmd/import_subject.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.21/obob_mne/mri/cmd/make_freesurfer_bem.py` & `obob_mne-0.0.22/obob_mne/mri/cmd/make_freesurfer_bem.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.21/obob_mne/mri/cmd/make_source_space.py` & `obob_mne-0.0.22/obob_mne/mri/cmd/make_source_space.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.21/obob_mne/mri/cmd/utils/__init__.py` & `obob_mne-0.0.22/obob_mne/mri/cmd/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.21/obob_mne/mri/cmd/utils/jobs.py` & `obob_mne-0.0.22/obob_mne/mri/cmd/utils/jobs.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.21/obob_mne/raw.py` & `obob_mne-0.0.22/obob_mne/raw.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.21/obob_mne.egg-info/SOURCES.txt` & `obob_mne-0.0.22/obob_mne.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.21/setup.py` & `obob_mne-0.0.22/setup.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.21/tests/__init__.py` & `obob_mne-0.0.22/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.21/tests/test_example.py` & `obob_mne-0.0.22/tests/test_example.py`

 * *Files identical despite different names*

