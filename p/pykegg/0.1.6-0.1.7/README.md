# Comparing `tmp/pykegg-0.1.6.tar.gz` & `tmp/pykegg-0.1.7.tar.gz`

## Comparing `pykegg-0.1.6.tar` & `pykegg-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0      782 2020-02-02 00:00:00.000000 pykegg-0.1.6/recipe/meta.yaml
--rwxr-xr-x   0        0        0    10670 2020-02-02 00:00:00.000000 pykegg-0.1.6/src/pykegg/KGML_graph.py
--rwxr-xr-x   0        0        0      103 2020-02-02 00:00:00.000000 pykegg-0.1.6/src/pykegg/__init__.py
--rwxr-xr-x   0        0        0    33735 2020-02-02 00:00:00.000000 pykegg-0.1.6/src/pykegg/utils.py
--rwxr-xr-x   0        0        0     2679 2020-02-02 00:00:00.000000 pykegg-0.1.6/.gitignore
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pykegg-0.1.6/LICENSE
--rwxr-xr-x   0        0        0     1635 2020-02-02 00:00:00.000000 pykegg-0.1.6/README.md
--rwxr-xr-x   0        0        0      845 2020-02-02 00:00:00.000000 pykegg-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 pykegg-0.1.6/PKG-INFO
+-rwxr-xr-x   0        0        0      834 2020-02-02 00:00:00.000000 pykegg-0.1.7/recipe/meta.yaml
+-rwxr-xr-x   0        0        0    10670 2020-02-02 00:00:00.000000 pykegg-0.1.7/src/pykegg/KGML_graph.py
+-rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 pykegg-0.1.7/src/pykegg/__init__.py
+-rwxr-xr-x   0        0        0    33735 2020-02-02 00:00:00.000000 pykegg-0.1.7/src/pykegg/utils.py
+-rwxr-xr-x   0        0        0     2679 2020-02-02 00:00:00.000000 pykegg-0.1.7/.gitignore
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pykegg-0.1.7/LICENSE
+-rwxr-xr-x   0        0        0     1506 2020-02-02 00:00:00.000000 pykegg-0.1.7/README.md
+-rwxr-xr-x   0        0        0      864 2020-02-02 00:00:00.000000 pykegg-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pykegg-0.1.7/PKG-INFO
```

### Comparing `pykegg-0.1.6/recipe/meta.yaml` & `pykegg-0.1.7/recipe/meta.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,46 @@
-{% set name = "pykegg" %}
-{% set version = "0.1.6" %}
-
-package:
-  name: {{ name|lower }}
-  version: {{ version }}
-
-source:
-  url: https://pypi.io/packages/source/{{ name[0] }}/{{ name }}/pykegg-{{ version }}.tar.gz
-
-build:
-  noarch: python
-  script: {{ PYTHON }} -m pip install . -vv --no-deps --no-build-isolation
-  number: 0
-
-requirements:
-  host:
-    - python >=3.7
-    - hatchling
-    - pip
-  run:
-    - python >=3.7
-    - python-igraph
-    - pandas
-    - biopython
-    - requests
-    - opencv
-
-test:
-  imports:
-    - pykegg
-  commands:
-    - pip check
-  requires:
-    - pip
-
-about:
-  summary: Visualizing and analyzing KEGG information in Python
-  license: AGPL-3
-  license_file: LICENSE
-
-extra:
-  recipe-maintainers:
-    - noriakis
+{% set name = "pykegg" %}
+{% set version = "0.1.6" %}
+
+package:
+  name: {{ name|lower }}
+  version: {{ version }}
+
+source:
+  url: https://pypi.io/packages/source/{{ name[0] }}/{{ name }}/pykegg-{{ version }}.tar.gz
+  sha256: 0d70be0dec36317a014d932ae727a88c56f823dd00dc3db8133a89cd45d586bc
+
+build:
+  noarch: python
+  script: {{ PYTHON }} -m pip install . -vv --no-deps --no-build-isolation
+  number: 0
+
+requirements:
+  host:
+    - python >=3.7
+    - hatchling
+    - pip
+  run:
+    - python >=3.7
+    - python-igraph
+    - pandas
+    - biopython
+    - requests
+    - py-opencv
+    - matplotlib
+
+test:
+  imports:
+    - pykegg
+  commands:
+    - pip check
+  requires:
+    - pip
+
+about:
+  summary: Visualizing and analyzing KEGG information in Python
+  license: EPL-2.0
+  license_file: LICENSE
+
+extra:
+  recipe-maintainers:
+    - noriakis
```

### Comparing `pykegg-0.1.6/src/pykegg/KGML_graph.py` & `pykegg-0.1.7/src/pykegg/KGML_graph.py`

 * *Files identical despite different names*

### Comparing `pykegg-0.1.6/src/pykegg/utils.py` & `pykegg-0.1.7/src/pykegg/utils.py`

 * *Files identical despite different names*

### Comparing `pykegg-0.1.6/.gitignore` & `pykegg-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pykegg-0.1.6/README.md` & `pykegg-0.1.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -25,20 +25,16 @@
 cmap_grad = mpl.colors.LinearSegmentedColormap.from_list("cmap_grad", ["yellow","green"])
 norm = mpl.colors.Normalize(vmin=min(nds.lfc), vmax=max(nds.lfc))
 nds["color"] = [
         mpl.colors.to_hex(cmap_grad(norm(x))) if x is not None else None
         for x in nds.lfc
     ]
 Image.fromarray(pykegg.overlay_opencv_image(nds, pid="hsa03460"))
-
-## Plot using plotnine
-# options.figure_size = (7,5)
-pykegg.plot_kegg_pathway_plotnine(g, node_x_nudge=25, label_size=5, show_label="gene")
 ```
 
 ## Documentation
-[https://pykegg.readthedocs.io/](https://pykegg.readthedocs.io/)
+[https://noriakis.github.io/pykegg-docs](https://noriakis.github.io/pykegg-docs)
 
 ## TODO
 - [ ] The function for converting identifiers (especially for ENTREZID <-> SYMBOL) without connection to servers, like using [`genomic-features`](https://genomic-features.readthedocs.io/en/latest/).
 - [ ] Parallel edge support by nudging x and y position
 - [ ] Better error handling
```

### Comparing `pykegg-0.1.6/pyproject.toml` & `pykegg-0.1.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,16 @@
   { name="Noriaki Sato", email="nori@hgc.jp" },
 ]
 dependencies = [
     "igraph",
     "pandas",
     "biopython",
     "requests",
-    "opencv-python"
+    "opencv-python",
+    "matplotlib"
 ]
 description = "Visualizing and analyzing KEGG information in Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `pykegg-0.1.6/PKG-INFO` & `pykegg-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.3
 Name: pykegg
-Version: 0.1.6
+Version: 0.1.7
 Summary: Visualizing and analyzing KEGG information in Python
 Project-URL: Homepage, https://github.com/noriakis/pykegg
 Project-URL: Bug Tracker, https://github.com/noriakis/pykegg/issues
 Author-email: Noriaki Sato <nori@hgc.jp>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: biopython
 Requires-Dist: igraph
+Requires-Dist: matplotlib
 Requires-Dist: opencv-python
 Requires-Dist: pandas
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # pykegg
 Analyze and visualize KEGG information using network approach.
@@ -44,20 +45,16 @@
 cmap_grad = mpl.colors.LinearSegmentedColormap.from_list("cmap_grad", ["yellow","green"])
 norm = mpl.colors.Normalize(vmin=min(nds.lfc), vmax=max(nds.lfc))
 nds["color"] = [
         mpl.colors.to_hex(cmap_grad(norm(x))) if x is not None else None
         for x in nds.lfc
     ]
 Image.fromarray(pykegg.overlay_opencv_image(nds, pid="hsa03460"))
-
-## Plot using plotnine
-# options.figure_size = (7,5)
-pykegg.plot_kegg_pathway_plotnine(g, node_x_nudge=25, label_size=5, show_label="gene")
 ```
 
 ## Documentation
-[https://pykegg.readthedocs.io/](https://pykegg.readthedocs.io/)
+[https://noriakis.github.io/pykegg-docs](https://noriakis.github.io/pykegg-docs)
 
 ## TODO
 - [ ] The function for converting identifiers (especially for ENTREZID <-> SYMBOL) without connection to servers, like using [`genomic-features`](https://genomic-features.readthedocs.io/en/latest/).
 - [ ] Parallel edge support by nudging x and y position
 - [ ] Better error handling
```

