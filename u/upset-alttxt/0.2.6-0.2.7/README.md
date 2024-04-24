# Comparing `tmp/upset-alttxt-0.2.6.tar.gz` & `tmp/upset-alttxt-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upset-alttxt-0.2.6.tar", last modified: Fri Apr 12 22:27:55 2024, max compression
+gzip compressed data, was "upset-alttxt-0.2.7.tar", last modified: Wed Apr 24 16:36:18 2024, max compression
```

## Comparing `upset-alttxt-0.2.6.tar` & `upset-alttxt-0.2.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:27:55.219862 upset-alttxt-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-12 22:27:55.219862 upset-alttxt-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-12 22:27:55.219862 upset-alttxt-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:27:55.215862 upset-alttxt-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:27:55.215862 upset-alttxt-0.2.6/src/alttxt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/src/alttxt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/src/alttxt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/src/alttxt/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/src/alttxt/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/src/alttxt/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    13128 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/src/alttxt/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/src/alttxt/phrases.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/src/alttxt/regionclass.py
--rw-r--r--   0 runner    (1001) docker     (127)    43919 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/src/alttxt/tokenmap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:27:55.219862 upset-alttxt-0.2.6/src/upset_alttxt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-12 22:27:55.000000 upset-alttxt-0.2.6/src/upset_alttxt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-12 22:27:55.000000 upset-alttxt-0.2.6/src/upset_alttxt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 22:27:55.000000 upset-alttxt-0.2.6/src/upset_alttxt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 22:27:54.000000 upset-alttxt-0.2.6/src/upset_alttxt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 22:27:55.000000 upset-alttxt-0.2.6/src/upset_alttxt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 22:27:55.000000 upset-alttxt-0.2.6/src/upset_alttxt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:27:55.219862 upset-alttxt-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/tests/test_alttxt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:36:18.500395 upset-alttxt-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-24 16:36:13.000000 upset-alttxt-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-24 16:36:18.500395 upset-alttxt-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-24 16:36:13.000000 upset-alttxt-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-24 16:36:13.000000 upset-alttxt-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-24 16:36:18.504395 upset-alttxt-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 16:36:13.000000 upset-alttxt-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:36:18.496395 upset-alttxt-0.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:36:18.500395 upset-alttxt-0.2.7/src/alttxt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:36:13.000000 upset-alttxt-0.2.7/src/alttxt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-24 16:36:13.000000 upset-alttxt-0.2.7/src/alttxt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-24 16:36:13.000000 upset-alttxt-0.2.7/src/alttxt/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-04-24 16:36:13.000000 upset-alttxt-0.2.7/src/alttxt/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-24 16:36:13.000000 upset-alttxt-0.2.7/src/alttxt/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13497 2024-04-24 16:36:13.000000 upset-alttxt-0.2.7/src/alttxt/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-04-24 16:36:13.000000 upset-alttxt-0.2.7/src/alttxt/phrases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-24 16:36:13.000000 upset-alttxt-0.2.7/src/alttxt/regionclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44323 2024-04-24 16:36:13.000000 upset-alttxt-0.2.7/src/alttxt/tokenmap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:36:18.500395 upset-alttxt-0.2.7/src/upset_alttxt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-24 16:36:18.000000 upset-alttxt-0.2.7/src/upset_alttxt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-24 16:36:18.000000 upset-alttxt-0.2.7/src/upset_alttxt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:36:18.000000 upset-alttxt-0.2.7/src/upset_alttxt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:36:18.000000 upset-alttxt-0.2.7/src/upset_alttxt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-24 16:36:18.000000 upset-alttxt-0.2.7/src/upset_alttxt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 16:36:18.000000 upset-alttxt-0.2.7/src/upset_alttxt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:36:18.500395 upset-alttxt-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-24 16:36:13.000000 upset-alttxt-0.2.7/tests/test_alttxt.py
```

### Comparing `upset-alttxt-0.2.6/LICENSE` & `upset-alttxt-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `upset-alttxt-0.2.6/PKG-INFO` & `upset-alttxt-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upset-alttxt
-Version: 0.2.6
+Version: 0.2.7
 Summary: Generates alt text for UpSet plots
 Author: Visualization Design Lab
 License: BSD3
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
```

### Comparing `upset-alttxt-0.2.6/README.md` & `upset-alttxt-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `upset-alttxt-0.2.6/pyproject.toml` & `upset-alttxt-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,11 +20,11 @@
 warn_return_any = true
 warn_unreachable = false
 warn_unused_configs = true
 no_implicit_reexport = true
 
 [project]
 name = "upset-alttxt"
-version = "0.2.6"
+version = "0.2.7"
 description = "Generates alt text for UpSet plots"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `upset-alttxt-0.2.6/setup.cfg` & `upset-alttxt-0.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `upset-alttxt-0.2.6/src/alttxt/__main__.py` & `upset-alttxt-0.2.7/src/alttxt/__main__.py`

 * *Files identical despite different names*

### Comparing `upset-alttxt-0.2.6/src/alttxt/enums.py` & `upset-alttxt-0.2.7/src/alttxt/enums.py`

 * *Files identical despite different names*

### Comparing `upset-alttxt-0.2.6/src/alttxt/generator.py` & `upset-alttxt-0.2.7/src/alttxt/generator.py`

 * *Files identical despite different names*

### Comparing `upset-alttxt-0.2.6/src/alttxt/models.py` & `upset-alttxt-0.2.7/src/alttxt/models.py`

 * *Files identical despite different names*

### Comparing `upset-alttxt-0.2.6/src/alttxt/parser.py` & `upset-alttxt-0.2.7/src/alttxt/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,28 +146,33 @@
             # a list of set names in the case of intersections
             name: str = item.get("elementName", self.default_field)
             if name.lower() == "unincluded":
                 name = "the empty intersection"
             # size
             size: int = int(item.get("size", self.default_field))
             # Deviation - rounded to 2 decimals
-            dev: float = round(item.get("deviation", self.default_field), 2)
+            # Backwards compatibility (<v0.2.7)
+            try:
+                dev: float = round(item.get("attributes", self.default_field)["deviation"], 2)
+            except KeyError:
+                dev: float = round(item.get("deviation", self.default_field), 2)
+
             # Degree
             degree: int = int(item.get("degree", self.default_field))
             # Classification
             classification = self.classify_subset(degree, len(data["visibleSets"]))
 
-               # Process setMembership to store only the names of sets with "Yes" membership
+            # Process setMembership to store only the names of sets with "Yes" membership
             setMembership = {key[4:] if key.startswith("Set_") else key: value for key, value in item.get("setMembership", {}).items() if value == "Yes"}
-        
+
             # Only store the keys (set names) that have "Yes" as their value
             yes_sets = {key for key, value in setMembership.items() if value == "Yes"}
 
             subsets.append(Subset(name=name, size=size, dev=dev, degree=degree, classification=classification, setMembership=yes_sets))
-        
+
         lowercase_data_visible_subsets = {k.lower(): k for k in data_visible_subsets.keys()}
 
         all_subsets: list[Subset] = []
         data_all_subsets = data["processedData"]["values"]
         count: list[int] = []
         for key, item in data_all_subsets.items():
 
@@ -182,15 +187,20 @@
             # a list of set names in the case of intersections
             name: str = item.get("elementName", self.default_field)
             if name.lower() == "unincluded":
                 name = "the empty intersection"
             # size
             size: int = int(item.get("size", self.default_field))
             # Deviation - rounded to 2 decimals
-            dev: float = round(item.get("deviation", self.default_field), 2)
+            # Backwards compatibility (<v0.2.7)
+            try:
+                dev: float = round(item.get("attributes", self.default_field)["deviation"], 2)
+            except KeyError:
+                dev: float = round(item.get("deviation", self.default_field), 2)
+
             # Degree - the degree might not be available in the raw data, handle accordingly
             degree: int = item.get("degree")
             if degree is not None:
                 degree = int(degree)
             else:
                 degree = 0  # or some default value
```

### Comparing `upset-alttxt-0.2.6/src/alttxt/phrases.py` & `upset-alttxt-0.2.7/src/alttxt/phrases.py`

 * *Files identical despite different names*

### Comparing `upset-alttxt-0.2.6/src/alttxt/regionclass.py` & `upset-alttxt-0.2.7/src/alttxt/regionclass.py`

 * *Files identical despite different names*

### Comparing `upset-alttxt-0.2.6/src/alttxt/tokenmap.py` & `upset-alttxt-0.2.7/src/alttxt/tokenmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -906,16 +906,23 @@
         # Extract only the names of the most and second most dominant sets
         most_dominant_set = most_common_sets[0][0]
         second_most_dominant_set = most_common_sets[1][0] if len(most_common_sets) > 1 else None
 
         return f"{most_dominant_set}, and {second_most_dominant_set}"
 
     def find_sets_in_large_subsets(self):
+
         # Sort subsets by size in descending order
         sorted_subsets = sorted(self.data.subsets, key=lambda subset: subset.size, reverse=True)
+
+        # Check the top two largest subsets and remove them if they have empty setMembership
+        if len(sorted_subsets) > 1 and len(sorted_subsets[1].setMembership) == 0:
+            sorted_subsets.pop(1)  # Remove the second largest if empty
+        elif len(sorted_subsets) > 2 and len(sorted_subsets[2].setMembership) == 0:
+            sorted_subsets.pop(2)  # Remove the third largest if empty
         
         # Extract set names from the 2nd largest subset
         second_largest_sets = sorted_subsets[1].setMembership
         sets = []
 
         if len(second_largest_sets) == 1:
             # Extract set names from the 3rd largest subset
```

### Comparing `upset-alttxt-0.2.6/src/upset_alttxt.egg-info/PKG-INFO` & `upset-alttxt-0.2.7/src/upset_alttxt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upset-alttxt
-Version: 0.2.6
+Version: 0.2.7
 Summary: Generates alt text for UpSet plots
 Author: Visualization Design Lab
 License: BSD3
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
```

### Comparing `upset-alttxt-0.2.6/src/upset_alttxt.egg-info/SOURCES.txt` & `upset-alttxt-0.2.7/src/upset_alttxt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

