# Comparing `tmp/odk_tools-0.1.2.tar.gz` & `tmp/odk_tools-0.1.3.tar.gz`

## Comparing `odk_tools-0.1.2.tar` & `odk_tools-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 odk_tools-0.1.2/src/odk_tools/__init__.py
--rw-r--r--   0        0        0    20111 2020-02-02 00:00:00.000000 odk_tools-0.1.2/src/odk_tools/classes.py
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 odk_tools-0.1.2/src/odk_tools/functions.py
--rw-r--r--   0        0        0    20494 2020-02-02 00:00:00.000000 odk_tools-0.1.2/src/odk_tools/odk.py
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 odk_tools-0.1.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 odk_tools-0.1.2/LICENSE
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 odk_tools-0.1.2/README.md
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 odk_tools-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 odk_tools-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 odk_tools-0.1.3/src/odk_tools/__init__.py
+-rw-r--r--   0        0        0    20111 2020-02-02 00:00:00.000000 odk_tools-0.1.3/src/odk_tools/classes.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 odk_tools-0.1.3/src/odk_tools/functions.py
+-rw-r--r--   0        0        0    20494 2020-02-02 00:00:00.000000 odk_tools-0.1.3/src/odk_tools/odk.py
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 odk_tools-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 odk_tools-0.1.3/LICENSE
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 odk_tools-0.1.3/README.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 odk_tools-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 odk_tools-0.1.3/PKG-INFO
```

### Comparing `odk_tools-0.1.2/src/odk_tools/classes.py` & `odk_tools-0.1.3/src/odk_tools/classes.py`

 * *Files identical despite different names*

### Comparing `odk_tools-0.1.2/src/odk_tools/functions.py` & `odk_tools-0.1.3/src/odk_tools/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     if type(subs.columns) == pd.core.indexes.base.Index:
         if len(reps) == 0:
             subs = subs.set_index('KEY', drop=False)
             return subs
         else:
             subs = subs.set_index('KEY', drop=False)
             out = subs.join(other=[value.set_index('PARENT_KEY').rename(columns={
-                            'KEY': 'KEY'+key.split('-')[-1]}) for key, value in reps.items()], how='inner', validate='one_to_many')
+                            'KEY': 'KEY'+key.split('-')[-1]}) for key, value in reps.items()], how='outer', validate='one_to_many')
             drops = []
             for j in range(len(out.columns)):
                 a = out.columns[j]
                 for i in range(len(out.columns)):
                     b = out.columns[i]
                     if (a[:-2] == b[:-2]) & (a[-2:] == '_x') & (b[-2:] == '_y'):
                         out[a] = out[b]
@@ -31,29 +31,31 @@
             return out
     else:
         if len(reps) == 0:
             subs = subs.set_index('KEY', drop=False)
             return subs
         else:
             subs = subs.set_index('KEY', drop=False)
-            out = subs.join(other=[value.set_index('PARENT_KEY').rename(columns={
-                            'KEY': 'KEY'+key.split('-')[-1]},level='code') for key, value in reps.items()], how='inner')
+            out = subs
+            for key,value in reps.items():
+                middle = out.join(value.set_index('PARENT_KEY').rename(columns={
+                    'KEY': 'KEY'+key.split('-')[-1]}, level='code'), how='outer', lsuffix='_x', rsuffix='_y')
+                out = middle
             drops = []
             for j in range(len(out.columns.get_level_values('code'))):
                 a = out.columns.get_level_values('code')[j]
                 for i in range(len(out.columns.get_level_values('code'))):
                     b = out.columns.get_level_values('code')[i]
                     if (a[:-2] == b[:-2]) & (a[-2:] == '_x') & (b[-2:] == '_y'):
                         out[a] = out[b]
                         out.rename(columns={a: a[:-2]}, inplace=True,level='code')
                         drops.append(b)
             out.drop(columns=drops, inplace=True,level='code')
             return out
 
-
 def multi_merge(forms = Dict[Form,str])->pd.DataFrame:
     to_be_merged = []
     for key,value in forms.items():
         df = form_merge(key).set_index(value, drop=False)
         h = df.columns.to_frame()
         h['survey'] = [key.survey_name for i in range(len(h))]
         df.columns = pd.MultiIndex.from_frame(h).reorder_levels(['survey']+list(set(df.columns.names).difference(set('survey'))))
```

### Comparing `odk_tools-0.1.2/src/odk_tools/odk.py` & `odk_tools-0.1.3/src/odk_tools/odk.py`

 * *Files identical despite different names*

### Comparing `odk_tools-0.1.2/LICENSE` & `odk_tools-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `odk_tools-0.1.2/pyproject.toml` & `odk_tools-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "odk_tools"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Federico Lorenzetti", email="lorenzetti.federico@gmail.com" },
 ]
 description = "A collection of tools for interacting with an ODK server and uploading/downloading submissions"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `odk_tools-0.1.2/PKG-INFO` & `odk_tools-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: odk_tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: A collection of tools for interacting with an ODK server and uploading/downloading submissions
 Project-URL: Homepage, https://github.com/federlorenz/odk_tools
 Author-email: Federico Lorenzetti <lorenzetti.federico@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

