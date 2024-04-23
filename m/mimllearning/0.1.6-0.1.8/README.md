# Comparing `tmp/mimllearning-0.1.6.tar.gz` & `tmp/mimllearning-0.1.8.tar.gz`

## Comparing `mimllearning-0.1.6.tar` & `mimllearning-0.1.8.tar`

### file list

```diff
@@ -1,47 +1,48 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 mimllearning-0.1.6/.gitattributes
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 mimllearning-0.1.6/readme.md
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 mimllearning-0.1.6/todo.md
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.1.6/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0    83682 2020-02-02 00:00:00.000000 mimllearning-0.1.6/documentation/Formato datos tfg.png
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/__init__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/miml_classifier.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/mi/__init__.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/mi/all_positive_apr_classifier.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/mi/apr_classifier.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/mi/iterated_discrim_apr_classifier.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/mi/miles_classifier.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/data/__init__.py
--rw-r--r--   0        0        0     9087 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/data/bag.py
--rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/data/instance.py
--rw-r--r--   0        0        0    15284 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/datasets/__init__.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/datasets/arff_to_csv.py
--rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/datasets/load_dataset.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/datasets/toy.csv
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/test/data_test.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/transformation/__init__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/transformation/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/transformation/mimlTOml/__init__.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/tutorial/classifiers_tutorial.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/tutorial/datasets_tutorial.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 mimllearning-0.1.6/src/miml/tutorial/transformation_tutorial.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 mimllearning-0.1.6/.gitignore
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 mimllearning-0.1.6/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 mimllearning-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 mimllearning-0.1.8/.gitattributes
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 mimllearning-0.1.8/readme.md
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 mimllearning-0.1.8/todo.md
+-rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 mimllearning-0.1.8/update.bat
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.1.8/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0    83682 2020-02-02 00:00:00.000000 mimllearning-0.1.8/documentation/Formato datos tfg.png
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/__init__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/classifier/mi/all_positive_apr_classifier.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/classifier/mi/iterated_discrim_apr_classifier.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/classifier/mi/miles_classifier.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/data/__init__.py
+-rw-r--r--   0        0        0     9087 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/data/instance.py
+-rw-r--r--   0        0        0    15284 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/datasets/__init__.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/datasets/arff_to_csv.py
+-rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/datasets/load_dataset.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/datasets/toy.csv
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/test/data_test.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/tutorial/classifiers_tutorial.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/tutorial/datasets_tutorial.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 mimllearning-0.1.8/src/miml/tutorial/transformation_tutorial.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 mimllearning-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 mimllearning-0.1.8/README.md
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 mimllearning-0.1.8/PKG-INFO
```

### Comparing `mimllearning-0.1.6/readme.md` & `mimllearning-0.1.8/readme.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/documentation/AnteproyectoDamianTFG.pdf` & `mimllearning-0.1.8/documentation/AnteproyectoDamianTFG.pdf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/documentation/Formato datos tfg.png` & `mimllearning-0.1.8/documentation/Formato datos tfg.png`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/src/miml/classifier/miml_classifier.py` & `mimllearning-0.1.8/src/miml/classifier/miml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/src/miml/classifier/mi/all_positive_apr_classifier.py` & `mimllearning-0.1.8/src/miml/classifier/mi/all_positive_apr_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/src/miml/classifier/mi/iterated_discrim_apr_classifier.py` & `mimllearning-0.1.8/src/miml/classifier/mi/iterated_discrim_apr_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/src/miml/classifier/mi/miles_classifier.py` & `mimllearning-0.1.8/src/miml/classifier/mi/miles_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py` & `mimllearning-0.1.8/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/src/miml/data/bag.py` & `mimllearning-0.1.8/src/miml/data/bag.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/src/miml/data/instance.py` & `mimllearning-0.1.8/src/miml/data/instance.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/src/miml/data/miml_dataset.py` & `mimllearning-0.1.8/src/miml/data/miml_dataset.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/src/miml/datasets/arff_to_csv.py` & `mimllearning-0.1.8/src/miml/datasets/arff_to_csv.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/src/miml/datasets/load_dataset.py` & `mimllearning-0.1.8/src/miml/datasets/load_dataset.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/src/miml/datasets/miml_birds.arff` & `mimllearning-0.1.8/src/miml/datasets/miml_birds.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/src/miml/datasets/miml_birds.csv` & `mimllearning-0.1.8/src/miml/datasets/miml_birds.csv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/src/miml/datasets/miml_birds_random_20test.arff` & `mimllearning-0.1.8/src/miml/datasets/miml_birds_random_20test.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/src/miml/datasets/miml_birds_random_80train.arff` & `mimllearning-0.1.8/src/miml/datasets/miml_birds_random_80train.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/src/miml/test/data_test.py` & `mimllearning-0.1.8/src/miml/test/data_test.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py` & `mimllearning-0.1.8/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/src/miml/transformation/mimlTOml/arithmetic.py` & `mimllearning-0.1.8/src/miml/transformation/mimlTOml/arithmetic.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/src/miml/transformation/mimlTOml/geometric.py` & `mimllearning-0.1.8/src/miml/transformation/mimlTOml/geometric.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/src/miml/transformation/mimlTOml/minmax.py` & `mimllearning-0.1.8/src/miml/transformation/mimlTOml/minmax.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/src/miml/tutorial/classifiers_tutorial.py` & `mimllearning-0.1.8/src/miml/tutorial/classifiers_tutorial.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 print(dataset_test.get_bag("366").get_labels()[0])
 classifier_ml.evaluate(dataset_test)
 
 classifier_mi = miml.MIMLtoMIBRClassifier(miml.AllPositiveAPRClassifier())
 classifier_mi.fit(dataset_train)
 print(classifier_mi.predict_bag(dataset_test.get_bag("366")))
 print(dataset_test.get_bag("366").get_labels()[0])
-#classifier_mi.evaluate(dataset_test)
+classifier_mi.evaluate(dataset_test)
```

### Comparing `mimllearning-0.1.6/README.md` & `mimllearning-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.6/pyproject.toml` & `mimllearning-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 requires = ["hatchling", "pkginfo >= 1.10"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/miml", "src/miml/*"]
 
 [metadata]
-version = "0.1.4"
+version = "0.1.8"
 name = "mimllearning"
 
 [project]
 name = "mimllearning"
-version = "0.1.6"
+version = "0.1.8"
 authors = [
   { name="Damian Martinez", email="damianmartinezavila@gmail.com" },
 ]
 description = "MIML Learning Library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mimllearning-0.1.6/PKG-INFO` & `mimllearning-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mimllearning
-Version: 0.1.6
+Version: 0.1.8
 Summary: MIML Learning Library
 Project-URL: Homepage, https://github.com/p82maavd/miml
 Author-email: Damian Martinez <damianmartinezavila@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

