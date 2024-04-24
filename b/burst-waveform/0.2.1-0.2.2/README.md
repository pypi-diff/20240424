# Comparing `tmp/burst-waveform-0.2.1.tar.gz` & `tmp/burst_waveform-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burst-waveform-0.2.1.tar", last modified: Mon Feb  5 10:18:16 2024, max compression
+gzip compressed data, was "burst_waveform-0.2.2.tar", last modified: Wed Apr 24 12:11:06 2024, max compression
```

## Comparing `burst-waveform-0.2.1.tar` & `burst_waveform-0.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 10:18:16.387163 burst-waveform-0.2.1/
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-02-05 10:18:00.000000 burst-waveform-0.2.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1830 2024-02-05 10:18:00.000000 burst-waveform-0.2.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)    35065 2024-02-05 10:18:00.000000 burst-waveform-0.2.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      100 2024-02-05 10:18:00.000000 burst-waveform-0.2.1/Makefile
--rw-r--r--   0 root         (0) root         (0)     1589 2024-02-05 10:18:16.386163 burst-waveform-0.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1132 2024-02-05 10:18:00.000000 burst-waveform-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 10:18:16.384163 burst-waveform-0.2.1/burst_waveform/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-05 10:18:00.000000 burst-waveform-0.2.1/burst_waveform/__init__.py
--rw-r--r--   0 root         (0) root         (0)      411 2024-02-05 10:18:16.000000 burst-waveform-0.2.1/burst_waveform/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2904 2024-02-05 10:18:00.000000 burst-waveform-0.2.1/burst_waveform/generate_waveform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 10:18:16.385163 burst-waveform-0.2.1/burst_waveform/models/
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-02-05 10:18:00.000000 burst-waveform-0.2.1/burst_waveform/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3176 2024-02-05 10:18:00.000000 burst-waveform-0.2.1/burst_waveform/models/sine_gaussian.py
--rw-rw-rw-   0 root         (0) root         (0)     3698 2024-02-05 10:18:00.000000 burst-waveform-0.2.1/burst_waveform/models/white_noise_burst.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 10:18:16.386163 burst-waveform-0.2.1/burst_waveform.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1589 2024-02-05 10:18:16.000000 burst-waveform-0.2.1/burst_waveform.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      597 2024-02-05 10:18:16.000000 burst-waveform-0.2.1/burst_waveform.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-05 10:18:16.000000 burst-waveform-0.2.1/burst_waveform.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-02-05 10:18:16.000000 burst-waveform-0.2.1/burst_waveform.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-02-05 10:18:16.000000 burst-waveform-0.2.1/burst_waveform.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 10:18:16.386163 burst-waveform-0.2.1/notebook/
--rw-rw-rw-   0 root         (0) root         (0)    41872 2024-02-05 10:18:00.000000 burst-waveform-0.2.1/notebook/SGQ_test.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    23999 2024-02-05 10:18:00.000000 burst-waveform-0.2.1/notebook/WNB_test.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     1490 2024-02-05 10:18:00.000000 burst-waveform-0.2.1/notebook/cWB_check.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    64207 2024-02-05 10:18:00.000000 burst-waveform-0.2.1/notebook/test.ipynb
--rw-rw-rw-   0 root         (0) root         (0)      542 2024-02-05 10:18:00.000000 burst-waveform-0.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-05 10:18:16.387163 burst-waveform-0.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1590 2024-02-05 10:18:00.000000 burst-waveform-0.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 10:18:16.386163 burst-waveform-0.2.1/test/
--rw-rw-rw-   0 root         (0) root         (0)      812 2024-02-05 10:18:00.000000 burst-waveform-0.2.1/test/test_waveform_generation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:11:06.930463 burst_waveform-0.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1830 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)    35065 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/Makefile
+-rw-r--r--   0 root         (0) root         (0)     1589 2024-04-24 12:11:06.929463 burst_waveform-0.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:11:06.928463 burst_waveform-0.2.2/burst_waveform/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/burst_waveform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2024-04-24 12:11:06.000000 burst_waveform-0.2.2/burst_waveform/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     3057 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/burst_waveform/generate_waveform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:11:06.928463 burst_waveform-0.2.2/burst_waveform/models/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/burst_waveform/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3176 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/burst_waveform/models/sine_gaussian.py
+-rw-rw-rw-   0 root         (0) root         (0)     3698 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/burst_waveform/models/white_noise_burst.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:11:06.929463 burst_waveform-0.2.2/burst_waveform.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1589 2024-04-24 12:11:06.000000 burst_waveform-0.2.2/burst_waveform.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      597 2024-04-24 12:11:06.000000 burst_waveform-0.2.2/burst_waveform.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 12:11:06.000000 burst_waveform-0.2.2/burst_waveform.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-24 12:11:06.000000 burst_waveform-0.2.2/burst_waveform.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-24 12:11:06.000000 burst_waveform-0.2.2/burst_waveform.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:11:06.929463 burst_waveform-0.2.2/notebook/
+-rw-rw-rw-   0 root         (0) root         (0)    41872 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/notebook/SGQ_test.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    23999 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/notebook/WNB_test.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     1490 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/notebook/cWB_check.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    63532 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/notebook/test.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      542 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 12:11:06.930463 burst_waveform-0.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:11:06.929463 burst_waveform-0.2.2/test/
+-rw-rw-rw-   0 root         (0) root         (0)      812 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/test/test_waveform_generation.py
```

### Comparing `burst-waveform-0.2.1/.gitlab-ci.yml` & `burst_waveform-0.2.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `burst-waveform-0.2.1/LICENSE` & `burst_waveform-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `burst-waveform-0.2.1/PKG-INFO` & `burst_waveform-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burst-waveform
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python package for gravitational wave burst waveform
 Home-page: https://git.ligo.org/yumeng.xu/setup.py
 Author: Yumeng Xu
 Author-email: The PycWB team <yumeng.xu@ligo.org>
 Keywords: ligo,sine-gaussian,white noise burst,gravitational waves,burst,waveform model
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `burst-waveform-0.2.1/README.md` & `burst_waveform-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `burst-waveform-0.2.1/burst_waveform/generate_waveform.py` & `burst_waveform-0.2.2/burst_waveform/generate_waveform.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,16 @@
     #     for key in waveform_dict.keys():
     #         new_dc[key] = waveform_dict[key].value
     #     return new_dc
     def generate_td_modes(self, **parameters):
         return 0
 
     def generate_td_waveform(self, **parameters):
-
+        for key in parameters.keys():
+            parameters[key] = parameters[key].value if hasattr(parameters[key], 'value') else parameters[key]
         gen_wf = self.model(parameters)
 
         hp = gen_wf()
 
-        hp = TimeSeries(hp, t0=0, sample_rate=parameters['sample_rate'], name='hp')
-        hc = TimeSeries(np.zeros(len(hp)), t0=0, sample_rate=parameters['sample_rate'], name='hc')
+        hp = TimeSeries(hp, t0=0, sample_rate=gen_wf.params['sample_rate'], name='hp')
+        hc = TimeSeries(np.zeros(len(hp)), t0=0, sample_rate=gen_wf.params['sample_rate'], name='hc')
         return gw.GravitationalWavePolarizations(hp=hp, hc=hc)
```

### Comparing `burst-waveform-0.2.1/burst_waveform/models/sine_gaussian.py` & `burst_waveform-0.2.2/burst_waveform/models/sine_gaussian.py`

 * *Files identical despite different names*

### Comparing `burst-waveform-0.2.1/burst_waveform/models/white_noise_burst.py` & `burst_waveform-0.2.2/burst_waveform/models/white_noise_burst.py`

 * *Files identical despite different names*

### Comparing `burst-waveform-0.2.1/burst_waveform.egg-info/PKG-INFO` & `burst_waveform-0.2.2/burst_waveform.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burst-waveform
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python package for gravitational wave burst waveform
 Home-page: https://git.ligo.org/yumeng.xu/setup.py
 Author: Yumeng Xu
 Author-email: The PycWB team <yumeng.xu@ligo.org>
 Keywords: ligo,sine-gaussian,white noise burst,gravitational waves,burst,waveform model
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `burst-waveform-0.2.1/burst_waveform.egg-info/SOURCES.txt` & `burst_waveform-0.2.2/burst_waveform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `burst-waveform-0.2.1/notebook/SGQ_test.ipynb` & `burst_waveform-0.2.2/notebook/SGQ_test.ipynb`

 * *Files identical despite different names*

### Comparing `burst-waveform-0.2.1/notebook/WNB_test.ipynb` & `burst_waveform-0.2.2/notebook/WNB_test.ipynb`

 * *Files identical despite different names*

### Comparing `burst-waveform-0.2.1/notebook/cWB_check.ipynb` & `burst_waveform-0.2.2/notebook/cWB_check.ipynb`

 * *Files identical despite different names*

### Comparing `burst-waveform-0.2.1/notebook/test.ipynb` & `burst_waveform-0.2.2/notebook/test.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9813722511574074%*

 * *Differences: {"'cells'": "{0: {'outputs': {0: {'text': {insert: [(10, "*

 * *            "'lal.swig_redirect_standard_output_error(False)\\n')], delete: [10]}}}, 'metadata': "*

 * *            "{'ExecuteTime': {'end_time': '2024-04-24T11:41:16.101622Z', 'start_time': "*

 * *            "'2024-04-24T11:40:59.675492Z'}}}, 1: {'outputs': {0: {'data': {'text/plain': "*

 * *            "'[<matplotlib.lines.Line2D at 0x17b7097d0>]'}}}, 'metadata': {'ExecuteTime': "*

 * *            "{'end_time': '2024-04-24T11:41:17.099340Z', 'start_time': "*

 * *         […]*

```diff
@@ -2,16 +2,16 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "e814bd746ec878c7",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2024-01-25T14:33:35.587145Z",
-                    "start_time": "2024-01-25T14:33:20.654963Z"
+                    "end_time": "2024-04-24T11:41:16.101622Z",
+                    "start_time": "2024-04-24T11:40:59.675492Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
@@ -22,15 +22,15 @@
                         "This may lead to performance penalties. To disable locally, use:\n",
                         "\n",
                         "with lal.no_swig_redirect_standard_output_error():\n",
                         "    ...\n",
                         "\n",
                         "To disable globally, use:\n",
                         "\n",
-                        "lal.swig_redirect_standard_output_error(True)\n",
+                        "lal.swig_redirect_standard_output_error(False)\n",
                         "\n",
                         "Note however that this will likely lead to error messages from\n",
                         "LAL functions being either misdirected or lost when called from\n",
                         "Jupyter notebooks.\n",
                         "\n",
                         "To suppress this warning, use:\n",
                         "\n",
@@ -197,23 +197,23 @@
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "cbd27e73f8d804bb",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2024-01-25T14:33:35.599605Z",
-                    "start_time": "2024-01-25T14:33:35.588595Z"
+                    "end_time": "2024-04-24T11:41:17.099340Z",
+                    "start_time": "2024-04-24T11:41:17.061955Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "[<matplotlib.lines.Line2D at 0x179e24810>]"
+                        "text/plain": "[<matplotlib.lines.Line2D at 0x17b7097d0>]"
                     },
                     "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
@@ -228,78 +228,84 @@
                 "wave = model()\n",
                 "\n",
                 "plt.plot(wave)\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
-            "id": "d5f7d5599bbb8798",
-            "metadata": {
-                "collapsed": false
-            },
-            "outputs": [],
-            "source": []
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 1,
             "id": "385d47a199a1ca56",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2024-01-25T14:33:40.640783Z",
-                    "start_time": "2024-01-25T14:33:40.375976Z"
+                    "end_time": "2024-04-24T11:59:55.968851Z",
+                    "start_time": "2024-04-24T11:59:52.998945Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "XLAL Error - initialize (LALSimInspiralGeneratorPython.c:18): Python generator not implemented\n",
-                        "XLAL Error - initialize (LALSimInspiralGeneratorPython.c:18): Invalid argument\n",
-                        "XLAL Error - XLALCreateSimInspiralGenerator (LALSimInspiral.c:426): Internal function call failed: Invalid argument\n"
+                        "/Users/yumengxu/miniforge3/envs/waveform/lib/python3.11/site-packages/lalsimulation/lalsimulation.py:8: UserWarning: Wswiglal-redir-stdio:\n",
+                        "\n",
+                        "SWIGLAL standard output/error redirection is enabled in IPython.\n",
+                        "This may lead to performance penalties. To disable locally, use:\n",
+                        "\n",
+                        "with lal.no_swig_redirect_standard_output_error():\n",
+                        "    ...\n",
+                        "\n",
+                        "To disable globally, use:\n",
+                        "\n",
+                        "lal.swig_redirect_standard_output_error(False)\n",
+                        "\n",
+                        "Note however that this will likely lead to error messages from\n",
+                        "LAL functions being either misdirected or lost when called from\n",
+                        "Jupyter notebooks.\n",
+                        "\n",
+                        "To suppress this warning, use:\n",
+                        "\n",
+                        "import warnings\n",
+                        "warnings.filterwarnings(\"ignore\", \"Wswiglal-redir-stdio\")\n",
+                        "import lal\n",
+                        "\n",
+                        "  import lal\n"
                     ]
                 },
                 {
-                    "ename": "RuntimeError",
-                    "evalue": "Internal function call failed: Invalid argument",
-                    "output_type": "error",
-                    "traceback": [
-                        "\u001b[0;31m---------------------------------------------------------------------------\u001b[0m",
-                        "\u001b[0;31mRuntimeError\u001b[0m                              Traceback (most recent call last)",
-                        "Cell \u001b[0;32mIn[3], line 20\u001b[0m\n\u001b[1;32m     17\u001b[0m lal\u001b[38;5;241m.\u001b[39mDictInsertStringValue(lal_dict, \u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mmodule\u001b[39m\u001b[38;5;124m\"\u001b[39m, \u001b[38;5;124m'\u001b[39m\u001b[38;5;124mburst_for.generate_waveform\u001b[39m\u001b[38;5;124m'\u001b[39m)\n\u001b[1;32m     18\u001b[0m lal\u001b[38;5;241m.\u001b[39mDictInsertStringValue(lal_dict, \u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mobject\u001b[39m\u001b[38;5;124m\"\u001b[39m, \u001b[38;5;124m'\u001b[39m\u001b[38;5;124mSineGaussianQ\u001b[39m\u001b[38;5;124m'\u001b[39m)\n\u001b[0;32m---> 20\u001b[0m generator \u001b[38;5;241m=\u001b[39m \u001b[43mlalsim\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mSimInspiralChooseGenerator\u001b[49m\u001b[43m(\u001b[49m\u001b[43mlal_approximant\u001b[49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[43mlal_dict\u001b[49m\u001b[43m)\u001b[49m\n\u001b[1;32m     22\u001b[0m hp, hc \u001b[38;5;241m=\u001b[39m lalsim\u001b[38;5;241m.\u001b[39mSimInspiralGenerateFDWaveform(lal_dict, generator)\n",
-                        "\u001b[0;31mRuntimeError\u001b[0m: Internal function call failed: Invalid argument"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "The pyseobnr package has failed to load, you will not be able to employ SEOBNRv5 approximants.\n",
+                        "{'amplitude': 1.0, 'object': 'SineGaussianQ', 'module': 'burst_waveform.generate_waveform', 'Q': 9, 'frequency': 300.0}\n",
+                        "{'amplitude': 1.0, 'object': 'SineGaussianQ', 'module': 'burst_waveform.generate_waveform', 'Q': 9, 'frequency': 300.0, 'duration': 0.004774648292756861}\n"
                     ]
                 }
             ],
             "source": [
                 "import lalsimulation.gwsignal.core.waveform as wfm\n",
                 "import lalsimulation as lalsim\n",
                 "import lal\n",
                 "\n",
                 "python_dict_nrsur = {\n",
                 "    \"amplitude\": 1.0,\n",
                 "    \"frequency\": 300.0,\n",
                 "    \"Q\": 9\n",
                 "}\n",
                 "\n",
-                "python_dict_nrsur = {\n",
-                "    \"mass1\": 10,\n",
-                "}\n",
+                "\n",
                 "lal_dict = lalsim.gwsignal.core.utils.to_lal_dict(python_dict_nrsur)\n",
                 "lal_approximant = lalsim.ExternalPython\n",
                 "\n",
-                "lal.DictInsertStringValue(lal_dict, \"module\", 'burst_for.generate_waveform')\n",
+                "lal.DictInsertStringValue(lal_dict, \"module\", 'burst_waveform.generate_waveform')\n",
                 "lal.DictInsertStringValue(lal_dict, \"object\", 'SineGaussianQ')\n",
                 "\n",
                 "generator = lalsim.SimInspiralChooseGenerator(lal_approximant, lal_dict)\n",
                 "\n",
-                "hp, hc = lalsim.SimInspiralGenerateFDWaveform(lal_dict, generator)"
+                "hp, hc = lalsim.SimInspiralGenerateTDWaveform(lal_dict, generator)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "f5dd1367c98c8006",
             "metadata": {
```

### Comparing `burst-waveform-0.2.1/pyproject.toml` & `burst_waveform-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `burst-waveform-0.2.1/setup.py` & `burst_waveform-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `burst-waveform-0.2.1/test/test_waveform_generation.py` & `burst_waveform-0.2.2/test/test_waveform_generation.py`

 * *Files identical despite different names*

