# Comparing `tmp/signaturizer-1.1.7.tar.gz` & `tmp/signaturizer-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/signaturizer-1.1.7.tar", last modified: Tue Nov 17 09:13:28 2020, max compression
+gzip compressed data, was "dist/signaturizer-1.1.9.tar", last modified: Mon Jan 25 10:44:14 2021, max compression
```

## Comparing `signaturizer-1.1.7.tar` & `signaturizer-1.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-17 09:13:28.000000 signaturizer-1.1.7/
--rw-r--r--   0 root         (0) root         (0)     8713 2020-11-17 09:13:28.000000 signaturizer-1.1.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7048 2020-11-17 09:00:37.000000 signaturizer-1.1.7/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2020-11-17 09:13:28.000000 signaturizer-1.1.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1054 2020-11-17 09:10:24.000000 signaturizer-1.1.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-17 09:13:28.000000 signaturizer-1.1.7/signaturizer/
--rw-rw-rw-   0 root         (0) root         (0)      164 2020-11-17 09:10:24.000000 signaturizer-1.1.7/signaturizer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4274 2020-07-13 16:10:30.000000 signaturizer-1.1.7/signaturizer/exporter.py
--rw-rw-rw-   0 root         (0) root         (0)    13859 2020-11-17 09:08:39.000000 signaturizer-1.1.7/signaturizer/signaturizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-17 09:13:28.000000 signaturizer-1.1.7/signaturizer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8713 2020-11-17 09:13:28.000000 signaturizer-1.1.7/signaturizer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      395 2020-11-17 09:13:28.000000 signaturizer-1.1.7/signaturizer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-11-17 09:13:28.000000 signaturizer-1.1.7/signaturizer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-11-17 09:13:28.000000 signaturizer-1.1.7/signaturizer.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       52 2020-11-17 09:13:28.000000 signaturizer-1.1.7/signaturizer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2020-11-17 09:13:28.000000 signaturizer-1.1.7/signaturizer.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-17 09:13:28.000000 signaturizer-1.1.7/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-07-02 13:57:14.000000 signaturizer-1.1.7/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1962 2020-07-02 13:57:15.000000 signaturizer-1.1.7/tests/helper.py
--rw-rw-rw-   0 root         (0) root         (0)     6001 2020-08-11 11:07:00.000000 signaturizer-1.1.7/tests/test_exporter.py
--rw-rw-rw-   0 root         (0) root         (0)     5003 2020-11-09 16:37:46.000000 signaturizer-1.1.7/tests/test_signaturizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-25 10:44:14.000000 signaturizer-1.1.9/
+-rw-r--r--   0 root         (0) root         (0)     8713 2021-01-25 10:44:14.000000 signaturizer-1.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2020-11-17 09:00:37.000000 signaturizer-1.1.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2021-01-25 10:44:14.000000 signaturizer-1.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1048 2021-01-25 10:30:20.000000 signaturizer-1.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-25 10:44:14.000000 signaturizer-1.1.9/signaturizer/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2021-01-25 10:30:20.000000 signaturizer-1.1.9/signaturizer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3637 2021-01-25 10:30:20.000000 signaturizer-1.1.9/signaturizer/exporter.py
+-rw-rw-rw-   0 root         (0) root         (0)    13396 2021-01-25 10:30:20.000000 signaturizer-1.1.9/signaturizer/signaturizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-25 10:44:14.000000 signaturizer-1.1.9/signaturizer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8713 2021-01-25 10:44:14.000000 signaturizer-1.1.9/signaturizer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      395 2021-01-25 10:44:14.000000 signaturizer-1.1.9/signaturizer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-01-25 10:44:14.000000 signaturizer-1.1.9/signaturizer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-01-25 10:44:14.000000 signaturizer-1.1.9/signaturizer.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2021-01-25 10:44:14.000000 signaturizer-1.1.9/signaturizer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2021-01-25 10:44:14.000000 signaturizer-1.1.9/signaturizer.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-25 10:44:14.000000 signaturizer-1.1.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-07-02 13:57:14.000000 signaturizer-1.1.9/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1962 2020-07-02 13:57:15.000000 signaturizer-1.1.9/tests/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     5207 2021-01-25 10:30:21.000000 signaturizer-1.1.9/tests/test_exporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     5097 2021-01-25 10:30:21.000000 signaturizer-1.1.9/tests/test_signaturizer.py
```

### Comparing `signaturizer-1.1.7/PKG-INFO` & `signaturizer-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signaturizer
-Version: 1.1.7
+Version: 1.1.9
 Summary: Generate Chemical Checker signatures from molecules SMILES.
 Home-page: http://gitlabsbnb.irbbarcelona.org/packages/signaturizer
 Author: Martino Bertoni
 Author-email: martino.bertoni@irbbarcelona.org
 License: MIT License
 Description: # Signaturizer
```

### Comparing `signaturizer-1.1.7/README.md` & `signaturizer-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `signaturizer-1.1.7/setup.py` & `signaturizer-1.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 __author__ = """Martino Bertoni"""
 __email__ = 'martino.bertoni@irbbarcelona.org'
-__version__ = '1.1.7'
+__version__ = '1.1.9'
 
 setup(
     name='signaturizer',
     version=__version__,
     author=__author__,
     author_email=__email__,
     description='Generate Chemical Checker signatures from molecules SMILES.',
     long_description=open('README.md').read().strip(),
     long_description_content_type="text/markdown",
     url='http://gitlabsbnb.irbbarcelona.org/packages/signaturizer',
     py_modules=find_packages(),
     packages=find_packages(),
     install_requires=[
-        'tensorflow<1.15',
-        'tensorflow_hub<0.10',
+        'tensorflow<2.4',
+        'tensorflow_hub',
         'numpy',
         'h5py',
         'tqdm'],
     zip_safe=False,
     license='MIT License',
     keywords='signaturizer bioactivity signatures chemicalchecker chemoinformatics',
     classifiers=[
```

### Comparing `signaturizer-1.1.7/signaturizer/signaturizer.py` & `signaturizer-1.1.9/signaturizer/signaturizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,56 +1,50 @@
 """Signaturize molecules."""
 import os
 import h5py
 import shutil
 import numpy as np
 from tqdm import tqdm
-import warnings
-with warnings.catch_warnings():
-    warnings.filterwarnings("ignore", category=FutureWarning)
-    warnings.filterwarnings("ignore", category=DeprecationWarning)
-    import tensorflow.compat.v1 as tf
-    import tensorflow_hub as hub
-    from tensorflow.compat.v1.keras.models import Model
-    from tensorflow.compat.v1.keras import Input
+import tensorflow as tf
+import tensorflow_hub as hub
+from tensorflow.keras import Model
+from tensorflow.keras import Input
+
 try:
     from rdkit import Chem
     from rdkit import RDLogger
     from rdkit.Chem import AllChem
 except ImportError:
     raise ImportError("requires RDKit " +
                       "https://www.rdkit.org/docs/Install.html")
 
-tf.logging.set_verbosity(tf.logging.ERROR)
-
 
 class Signaturizer(object):
     """Signaturizer Class.
 
     Loads TF-hub module, compose a single model, handle verbosity.
     """
 
     def __init__(self, model_name,
                  base_url="http://chemicalchecker.com/api/db/getSignaturizer/",
-                 version='v1.1', local=False, tf_version='1', verbose=False,
+                 version='2020_02', local=False, verbose=False,
                  applicability=True):
         """Initialize a Signaturizer instance.
 
         Args:
             model(str): The model to load. Possible values:
                 - the model name (the bioactivity space (e.g. "B1") )
                 - the model path (the directory containing 'saved_model.pb')
                 - a list of models names or paths (e.g. ["B1", "B2", "E5"])
                 - 'GLOBAL' to get the global (i.e. horizontally stacked)
                     bioactivity signature.
             base_url(str): The ChemicalChecker getModel API URL.
             version(int): Signaturizer version.
             local(bool): Wethere the specified model_name shoudl be
                 interpreted as a path to a local model.
-            tf_version(int): The Tesorflow version.
             verbose(bool): If True some more information will be printed.
             applicability(bool): Wether to also compute the applicability of
                 each prediction.
         """
         self.verbose = verbose
         self.applicability = applicability
         if not isinstance(model_name, list):
@@ -65,46 +59,41 @@
                 if 'GLOBAL' in model_name:
                     raise Exception('"GLOBAL" model can only be used alone.')
                 self.model_names = model_name
         # load modules as layer to compose a new model
         main_input = Input(shape=(2048,), dtype=tf.float32, name='main_input')
         sign_output = list()
         app_output = list()
-        as_dict = False
-        output_key = 'default'
-        if len(self.model_names) == 1:
-            as_dict = True
-            output_key = None
         for name in self.model_names:
             # build module spec
             if local:
                 if os.path.isdir(name):
                     url = name
                     if self.verbose:
                         print('LOADING local:', url)
                 else:
                     raise Exception('Module path not found!')
             else:
                 url = base_url + '%s/%s' % (version, name)
                 if self.verbose:
                     print('LOADING remote:', url)
 
-            sign_layer = hub.KerasLayer(url, signature='serving_default',
+            sign_layer = hub.KerasLayer(url, signature='signature',
                                         trainable=False, tags=['serve'],
-                                        output_key=output_key,
-                                        signature_outputs_as_dict=as_dict)
+                                        output_key='signature',
+                                        signature_outputs_as_dict=False)
             sign_output.append(sign_layer(main_input))
 
             if self.applicability:
                 try:
                     app_layer = hub.KerasLayer(
                         url, signature='applicability',
                         trainable=False, tags=['serve'],
-                        output_key=output_key,
-                        signature_outputs_as_dict=as_dict)
+                        output_key='applicability',
+                        signature_outputs_as_dict=False)
                     app_output.append(app_layer(main_input))
                 except Exception as ex:
                     print('WARNING: applicability predictions not available. '
                           + str(ex))
                     self.applicability = False
         # join signature output and prepare model
         if len(sign_output) > 1:
@@ -214,19 +203,19 @@
                 results.mfp[chunk] = sign0s
             # run applicability predictor
             if self.applicability:
                 apreds = self.app_model.predict(sign0s, batch_size=batch_size)
                 if failed:
                     apreds[np.array(failed)] = np.nan
                 results.applicability[chunk] = apreds
+        failed = np.isnan(results.signature[:, 0])
+        results.failed[:] = np.isnan(results.signature[:, 0])
         results.close()
         if self.verbose:
             print('PREDICTION complete!')
-        failed = np.isnan(results.signature[:, 0])
-        results.failed = failed
         if any(failed) > 0:
             print('Some molecules could not be recognized,'
                   ' the corresponding signatures are NaN')
             if self.verbose:
                 for idx in np.argwhere(failed).flatten():
                     print(molecules[idx])
         return results
```

### Comparing `signaturizer-1.1.7/signaturizer.egg-info/PKG-INFO` & `signaturizer-1.1.9/signaturizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signaturizer
-Version: 1.1.7
+Version: 1.1.9
 Summary: Generate Chemical Checker signatures from molecules SMILES.
 Home-page: http://gitlabsbnb.irbbarcelona.org/packages/signaturizer
 Author: Martino Bertoni
 Author-email: martino.bertoni@irbbarcelona.org
 License: MIT License
 Description: # Signaturizer
```

### Comparing `signaturizer-1.1.7/tests/helper.py` & `signaturizer-1.1.9/tests/helper.py`

 * *Files identical despite different names*

### Comparing `signaturizer-1.1.7/tests/test_exporter.py` & `signaturizer-1.1.9/tests/test_exporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import shutil
 import unittest
 import numpy as np
 from .helper import skip_if_import_exception, start_http_server
 
-from signaturizer.exporter import export_smilespred, export_savedmodel
+from signaturizer.exporter import export_smilespred
 from signaturizer import Signaturizer
 
 
-class TestSignaturizer(unittest.TestCase):
+class TestExporter(unittest.TestCase):
 
     def setUp(self):
         # path for test data
         test_dir = os.path.dirname(os.path.realpath(__file__))
         self.data_dir = os.path.join(test_dir, 'data')
         self.tmp_dir = os.path.join(test_dir, 'tmp')
         if os.path.exists(self.tmp_dir):
@@ -72,14 +72,15 @@
         base_url = "http://localhost:%d/" % (self.server_port)
         module = Signaturizer(module_file, base_url=base_url, version=version,
                               applicability=True)
         res = module.predict(self.test_smiles)
         pred = res.signature[:]
         ref_pred_file = os.path.join(
             self.data_dir, 'models', 'smiles_pred.npy')
+        #np.save(ref_pred_file, pred)
         pred_ref = np.load(ref_pred_file)
         np.testing.assert_almost_equal(pred_ref, pred)
         apred = res.applicability[:]
         ref_apred_file = os.path.join(
             self.data_dir, 'models', 'applicability_pred.npy')
         #np.save(ref_apred_file, apred)
         apred_ref = np.load(ref_apred_file)
@@ -118,24 +119,7 @@
         # test final step
         base_url = "http://localhost:%d/" % (self.server_port)
         module = Signaturizer(module_file, base_url=base_url, version=version)
         res = module.predict(self.test_smiles)
         pred = res.signature[:]
         np.testing.assert_almost_equal(pred_ref, pred)
 
-        # export savedmodel
-        module_destination = os.path.join(
-            self.tmp_dir, 'dest_savedmodel.tar.gz')
-        tmp_path_savedmodel = os.path.join(self.tmp_dir, 'export_savedmodel')
-        export_savedmodel(
-            tmp_path_smilespred, module_destination,
-            tmp_path=tmp_path_savedmodel, clear_tmp=False)
-        # test intermediate step
-        module = Signaturizer(tmp_path_savedmodel, local=True)
-        res = module.predict(self.test_smiles)
-        pred = res.signature[:]
-        np.testing.assert_almost_equal(pred_ref, pred)
-        # test final step
-        module = Signaturizer(module_file, base_url=base_url, version=version)
-        res = module.predict(self.test_smiles)
-        pred = res.signature[:]
-        np.testing.assert_almost_equal(pred_ref, pred)
```

### Comparing `signaturizer-1.1.7/tests/test_signaturizer.py` & `signaturizer-1.1.9/tests/test_signaturizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import math
-import pickle
 import shutil
 import unittest
 import numpy as np
 
 from signaturizer import Signaturizer
 
 
@@ -33,26 +32,28 @@
     def tearDown(self):
         if os.path.exists(self.tmp_dir):
             shutil.rmtree(self.tmp_dir, ignore_errors=True)
             pass
 
     def test_predict(self):
         # load reference predictions
-        ref_file = os.path.join(self.data_dir, 'pred.pkl')
-        pred_ref = pickle.load(open(ref_file, 'rb'))
+        ref_file = os.path.join(self.data_dir, 'pred.npy')
+        pred_ref = np.load(open(ref_file, 'rb'))
         # load module and predict
         module_dir = os.path.join(self.data_dir, 'B1')
         module = Signaturizer(module_dir, local=True)
         res = module.predict(self.test_smiles)
         np.testing.assert_almost_equal(pred_ref, res.signature[:])
         # test saving to file
         destination = os.path.join(self.tmp_dir, 'pred.h5')
         res = module.predict(self.test_smiles, destination)
         self.assertTrue(os.path.isfile(destination))
         np.testing.assert_almost_equal(pred_ref, res.signature[:])
+        self.assertEqual(len(res.applicability[:]), 2)
+        self.assertFalse(np.isnan(res.applicability[0]))
         # test prediction of invalid SMILES
         res = module.predict(self.invalid_smiles)
         for comp in res.signature[0]:
             self.assertFalse(math.isnan(comp))
         for comp in res.signature[1]:
             self.assertTrue(math.isnan(comp))
         for comp in res.signature[2]:
```

