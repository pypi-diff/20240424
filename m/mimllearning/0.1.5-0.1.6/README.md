# Comparing `tmp/mimllearning-0.1.5.tar.gz` & `tmp/mimllearning-0.1.6.tar.gz`

## Comparing `mimllearning-0.1.5.tar` & `mimllearning-0.1.6.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 mimllearning-0.1.5/.gitattributes
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 mimllearning-0.1.5/readme.md
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 mimllearning-0.1.5/todo.md
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.1.5/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0    83682 2020-02-02 00:00:00.000000 mimllearning-0.1.5/documentation/Formato datos tfg.png
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/__init__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/classifier/miml_classifier.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/classifier/mi/__init__.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/classifier/mi/all_positive_apr_classifier.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/classifier/mi/apr_classifier.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/classifier/mi/iterated_discrim_apr_classifier.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/classifier/mi/miles_classifier.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/classifier/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/classifier/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/data/__init__.py
--rw-r--r--   0        0        0     9087 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/data/bag.py
--rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/data/instance.py
--rw-r--r--   0        0        0    15284 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/datasets/__init__.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/datasets/arff_to_csv.py
--rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/datasets/load_dataset.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/datasets/toy.csv
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/test/data_test.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/transformation/__init__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/transformation/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/transformation/mimlTOml/__init__.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/tutorial/demo.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 mimllearning-0.1.5/src/miml/tutorial/demopypi.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 mimllearning-0.1.5/.gitignore
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 mimllearning-0.1.5/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 mimllearning-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 mimllearning-0.1.6/.gitattributes
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 mimllearning-0.1.6/readme.md
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 mimllearning-0.1.6/todo.md
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.1.6/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0    83682 2020-02-02 00:00:00.000000 mimllearning-0.1.6/documentation/Formato datos tfg.png
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/__init__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/mi/all_positive_apr_classifier.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/mi/iterated_discrim_apr_classifier.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/mi/miles_classifier.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/data/__init__.py
+-rw-r--r--   0        0        0     9087 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/data/instance.py
+-rw-r--r--   0        0        0    15284 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/datasets/__init__.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/datasets/arff_to_csv.py
+-rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/datasets/load_dataset.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/datasets/toy.csv
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/test/data_test.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/tutorial/classifiers_tutorial.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/tutorial/datasets_tutorial.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/tutorial/transformation_tutorial.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 mimllearning-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 mimllearning-0.1.6/README.md
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 mimllearning-0.1.6/PKG-INFO
```

### Comparing `mimllearning-0.1.5/readme.md` & `mimllearning-0.1.6/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 - [License](#license)
 
 ### Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install miml.
 
 ```bash
-$ pip install miml-package
+$ pip install mimllearning
 ```
 #### Requirements
 The requirement packages for miml library are: numpy, scikit-learn, scipy, tensorflow or tensorflow-gpu.
 Installing miml with the package manager does not install the package dependencies.
 So install them with the package manager manually if not already downloaded.
 
     $ pip install numpy
```

### Comparing `mimllearning-0.1.5/documentation/AnteproyectoDamianTFG.pdf` & `mimllearning-0.1.6/documentation/AnteproyectoDamianTFG.pdf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.5/documentation/Formato datos tfg.png` & `mimllearning-0.1.6/documentation/Formato datos tfg.png`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.5/src/miml/classifier/miml_classifier.py` & `mimllearning-0.1.6/src/miml/classifier/miml_classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from abc import ABC, abstractmethod
 
 import numpy as np
 
 from data.bag import Bag
 from data.miml_dataset import MIMLDataset
+from sklearn.metrics import classification_report, hamming_loss
 
-from sklearn.metrics import accuracy_score, average_precision_score, f1_score, hamming_loss, precision_score, \
-    recall_score
 
 class MIMLClassifier(ABC):
     """
     Class to represent a MIMLClassifier
     """
 
     def __init__(self) -> None:
```

### Comparing `mimllearning-0.1.5/src/miml/classifier/mi/all_positive_apr_classifier.py` & `mimllearning-0.1.6/src/miml/classifier/mi/all_positive_apr_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.5/src/miml/classifier/mi/iterated_discrim_apr_classifier.py` & `mimllearning-0.1.6/src/miml/classifier/mi/iterated_discrim_apr_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.5/src/miml/classifier/mi/miles_classifier.py` & `mimllearning-0.1.6/src/miml/classifier/mi/miles_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.5/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py` & `mimllearning-0.1.6/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.5/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py` & `mimllearning-0.1.6/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.5/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py` & `mimllearning-0.1.6/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+
 from classifier.miml_classifier import *
 
 from transformation.mimlTOml.miml_to_ml_transformation import MIMLtoMLTransformation
 
 
 class MIMLtoMLClassifier(MIMLClassifier):
 
@@ -55,19 +56,19 @@
         ----------
         dataset_test
         """
         super().evaluate(dataset_test)
         x_test, y_test = self.transformation.transform_dataset(dataset_test)
         results = self.predict(x_test)
 
-        accuracy = accuracy_score(dataset_test.get_labels_by_bag(), results)
-        average_precision = average_precision_score(dataset_test.get_labels_by_bag(), results)
-        f1_macro = f1_score(dataset_test.get_labels_by_bag(), results, average='macro')
-        f1_micro = f1_score(dataset_test.get_labels_by_bag(), results, average='micro')
-        hamming_loss_score = hamming_loss(dataset_test.get_labels_by_bag(), results)
-        precision_macro = precision_score(dataset_test.get_labels_by_bag(), results, average='macro')
-        precision_micro = precision_score(dataset_test.get_labels_by_bag(), results, average='micro')
-        recall_macro = recall_score(dataset_test.get_labels_by_bag(), results, average='macro')
-        recall_micro = recall_score(dataset_test.get_labels_by_bag(), results, average='micro')
+        print(classification_report(dataset_test.get_labels_by_bag(), results))
+        print(hamming_loss(dataset_test.get_labels_by_bag(), results))
+        #accuracy = accuracy_score(dataset_test.get_labels_by_bag(), results)
+        #average_precision = average_precision_score(dataset_test.get_labels_by_bag(), results)
+        #f1_macro = f1_score(dataset_test.get_labels_by_bag(), results, average='macro')
+        #f1_micro = f1_score(dataset_test.get_labels_by_bag(), results, average='micro')
+        #hamming_loss_score = hamming_loss(dataset_test.get_labels_by_bag(), results)
+        #precision_macro = precision_score(dataset_test.get_labels_by_bag(), results, average='macro')
+        #precision_micro = precision_score(dataset_test.get_labels_by_bag(), results, average='micro')
+        #recall_macro = recall_score(dataset_test.get_labels_by_bag(), results, average='macro')
+        #recall_micro = recall_score(dataset_test.get_labels_by_bag(), results, average='micro')
 
-        print(accuracy, average_precision, f1_macro, f1_micro, hamming_loss_score, precision_macro, precision_micro,
-              recall_macro, recall_micro)
```

### Comparing `mimllearning-0.1.5/src/miml/data/bag.py` & `mimllearning-0.1.6/src/miml/data/bag.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.5/src/miml/data/instance.py` & `mimllearning-0.1.6/src/miml/data/instance.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.5/src/miml/data/miml_dataset.py` & `mimllearning-0.1.6/src/miml/data/miml_dataset.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.5/src/miml/datasets/arff_to_csv.py` & `mimllearning-0.1.6/src/miml/datasets/arff_to_csv.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.5/src/miml/datasets/load_dataset.py` & `mimllearning-0.1.6/src/miml/datasets/load_dataset.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.5/src/miml/datasets/miml_birds.arff` & `mimllearning-0.1.6/src/miml/datasets/miml_birds.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.5/src/miml/datasets/miml_birds.csv` & `mimllearning-0.1.6/src/miml/datasets/miml_birds.csv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.5/src/miml/datasets/miml_birds_random_20test.arff` & `mimllearning-0.1.6/src/miml/datasets/miml_birds_random_20test.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.5/src/miml/datasets/miml_birds_random_80train.arff` & `mimllearning-0.1.6/src/miml/datasets/miml_birds_random_80train.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.5/src/miml/test/data_test.py` & `mimllearning-0.1.6/src/miml/test/data_test.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.5/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py` & `mimllearning-0.1.6/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.5/src/miml/transformation/mimlTOml/arithmetic.py` & `mimllearning-0.1.6/src/miml/transformation/mimlTOml/arithmetic.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.5/src/miml/transformation/mimlTOml/geometric.py` & `mimllearning-0.1.6/src/miml/transformation/mimlTOml/geometric.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.5/src/miml/transformation/mimlTOml/minmax.py` & `mimllearning-0.1.6/src/miml/transformation/mimlTOml/minmax.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.5/README.md` & `mimllearning-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 - [License](#license)
 
 ### Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install miml.
 
 ```bash
-$ pip install miml-package
+$ pip install mimllearning
 ```
 #### Requirements
 The requirement packages for miml library are: numpy, scikit-learn, scipy, tensorflow or tensorflow-gpu.
 Installing miml with the package manager does not install the package dependencies.
 So install them with the package manager manually if not already downloaded.
 
     $ pip install numpy
```

### Comparing `mimllearning-0.1.5/pyproject.toml` & `mimllearning-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [metadata]
 version = "0.1.4"
 name = "mimllearning"
 
 [project]
 name = "mimllearning"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Damian Martinez", email="damianmartinezavila@gmail.com" },
 ]
 description = "MIML Learning Library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mimllearning-0.1.5/PKG-INFO` & `mimllearning-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mimllearning
-Version: 0.1.5
+Version: 0.1.6
 Summary: MIML Learning Library
 Project-URL: Homepage, https://github.com/p82maavd/miml
 Author-email: Damian Martinez <damianmartinezavila@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -19,15 +19,15 @@
 - [License](#license)
 
 ### Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install miml.
 
 ```bash
-$ pip install miml-package
+$ pip install mimllearning
 ```
 #### Requirements
 The requirement packages for miml library are: numpy, scikit-learn, scipy, tensorflow or tensorflow-gpu.
 Installing miml with the package manager does not install the package dependencies.
 So install them with the package manager manually if not already downloaded.
 
     $ pip install numpy
```

