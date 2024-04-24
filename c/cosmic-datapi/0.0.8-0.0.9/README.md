# Comparing `tmp/cosmic_datapi-0.0.8.tar.gz` & `tmp/cosmic_datapi-0.0.9.tar.gz`

## Comparing `cosmic_datapi-0.0.8.tar` & `cosmic_datapi-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/requirements.txt
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/examples/_template.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/examples/example.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/examples/lamps.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/examples/state_generator_example.py
--rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/scripts/build.sh
--rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/scripts/install.sh
--rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/scripts/install_datamods.sh
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/scripts/publish.sh
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/src/cosmic_datapi/__init__.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/src/cosmic_datapi/api/__init__.py
--rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/src/cosmic_datapi/api/actions.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/src/cosmic_datapi/api/models.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/src/cosmic_datapi/builders/__init__.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/src/cosmic_datapi/builders/block.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/src/cosmic_datapi/builders/block_events.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/src/cosmic_datapi/builders/block_state.py
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/src/cosmic_datapi/builders/block_state_generator.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/src/cosmic_datapi/builders/model.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/.gitignore
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/readme.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/license.txt
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/examples/_template.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/examples/cuboid_example.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/examples/example.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/examples/lamps.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/examples/state_generator_example.py
+-rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/scripts/build.sh
+-rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/scripts/install.sh
+-rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/scripts/install_datamods.sh
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/scripts/publish.sh
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/src/cosmic_datapi/__init__.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/src/cosmic_datapi/api/__init__.py
+-rw-r--r--   0        0        0     5979 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/src/cosmic_datapi/api/actions.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/src/cosmic_datapi/api/models.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/src/cosmic_datapi/builders/__init__.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/src/cosmic_datapi/builders/block.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/src/cosmic_datapi/builders/block_events.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/src/cosmic_datapi/builders/block_state.py
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/src/cosmic_datapi/builders/block_state_generator.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/src/cosmic_datapi/builders/model.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/.gitignore
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/readme.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 cosmic_datapi-0.0.9/PKG-INFO
```

### Comparing `cosmic_datapi-0.0.8/examples/example.py` & `cosmic_datapi-0.0.9/examples/example.py`

 * *Files identical despite different names*

### Comparing `cosmic_datapi-0.0.8/examples/lamps.py` & `cosmic_datapi-0.0.9/examples/lamps.py`

 * *Files identical despite different names*

### Comparing `cosmic_datapi-0.0.8/examples/state_generator_example.py` & `cosmic_datapi-0.0.9/examples/state_generator_example.py`

 * *Files identical despite different names*

### Comparing `cosmic_datapi-0.0.8/src/cosmic_datapi/__init__.py` & `cosmic_datapi-0.0.9/src/cosmic_datapi/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from . import builders
-from typing import Union
+from typing import Union, Callable
 import tqdm
 import os
 import shutil
 
 
 class Mod:
     def __init__(self, namespace: str):
@@ -26,35 +26,39 @@
                 else:
                     shutil.copytree(path, self.output_dir, dirs_exist_ok = True)
                 bar.update()
 
             bar.set_description("Done!")
             bar.close()
 
+    def include(self, path: Union[str, list[str]]) -> "Mod":
+        if not (os.path.exists(path) or os.path.isfile(path)):
+            print(f"error: {path} is included but does not exist.")
+            exit(1)
+
+        if type(path) == list:
+            self._included_paths.extend(path)
+        else:
+            self._included_paths.append(path)
+
+        return self
+
+    # Generators
     def _generator(self, clazz, *args, **kwargs):
         builder = clazz(self, *args, **kwargs)
         self._generators.append(builder)
         return builder
 
     def block(self, name: str) -> builders.BlockBuilder:
         return self._generator(builders.BlockBuilder, name)
 
     def block_events(self, name: str) -> builders.BlockEventsBuilder:
         return self._generator(builders.BlockEventsBuilder, name)
 
     def block_model(self, name: str) -> builders.BlockModelBuilder:
         return self._generator(builders.BlockModelBuilder, name)
 
+    def cuboid_block_model(self, name: str) -> builders.CuboidBlockModelBuilder:
+        return self._generator(builders.CuboidBlockModelBuilder, name)
+
     def block_state_generator(self, name: str) -> builders.BlockStateGeneratorBuilder:
         return self._generator(builders.BlockStateGeneratorBuilder, name)
-
-    def include(self, path: Union[str, list[str]]) -> "Mod":
-        if not (os.path.exists(path) or os.path.isfile(path)):
-            print(f"error: {path} is included but does not exist.")
-            exit(1)
-
-        if type(path) == list:
-            self._included_paths.extend(path)
-        else:
-            self._included_paths.append(path)
-
-        return self
```

### Comparing `cosmic_datapi-0.0.8/src/cosmic_datapi/api/__init__.py` & `cosmic_datapi-0.0.9/src/cosmic_datapi/api/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmic_datapi-0.0.8/src/cosmic_datapi/api/actions.py` & `cosmic_datapi-0.0.9/src/cosmic_datapi/api/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         z_off: int = 0,
         x_normal: int = 0,
         y_normal: int = 0,
         z_normal: int = 0,
         trigger_before_set_id: Optional[str] = None,
         trigger_after_set_id: Optional[str] = None
     ):
-        super().__init__(x_off, y_off, z_off)
+        super().__init__("base:set_spherical_segment", x_off, y_off, z_off)
         self.data["radius"] = radius
         self.data["angleDeg"] = angle_deg
         self.data["xNormal"] = x_normal
         self.data["yNormal"] = y_normal
         self.data["zNormal"] = z_normal
         if block_state_id is not None:
             self.data["blockStateId"] = block_state_id
```

### Comparing `cosmic_datapi-0.0.8/src/cosmic_datapi/builders/block.py` & `cosmic_datapi-0.0.9/src/cosmic_datapi/builders/block.py`

 * *Files identical despite different names*

### Comparing `cosmic_datapi-0.0.8/src/cosmic_datapi/builders/block_events.py` & `cosmic_datapi-0.0.9/src/cosmic_datapi/builders/block_events.py`

 * *Files identical despite different names*

### Comparing `cosmic_datapi-0.0.8/src/cosmic_datapi/builders/block_state.py` & `cosmic_datapi-0.0.9/src/cosmic_datapi/builders/block_state.py`

 * *Files identical despite different names*

### Comparing `cosmic_datapi-0.0.8/src/cosmic_datapi/builders/block_state_generator.py` & `cosmic_datapi-0.0.9/src/cosmic_datapi/builders/block_state_generator.py`

 * *Files identical despite different names*

### Comparing `cosmic_datapi-0.0.8/pyproject.toml` & `cosmic_datapi-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cosmic-datapi"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name = "EmmaTheMartian", email = "emmathemartian@gmail.com" },
 ]
 description = "Basically a library to create data mods in Cosmic Reach really fast."
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `cosmic_datapi-0.0.8/PKG-INFO` & `cosmic_datapi-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cosmic-datapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Basically a library to create data mods in Cosmic Reach really fast.
 Project-URL: Homepage, https://codeberg.org/EmmaTheMartian/cosmic-datapi
 Project-URL: Issues, https://codeberg.org/EmmaTheMartian/cosmic-datapi/issues
 Author-email: EmmaTheMartian <emmathemartian@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

