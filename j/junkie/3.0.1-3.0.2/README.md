# Comparing `tmp/junkie-3.0.1.tar.gz` & `tmp/junkie-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/junkie/junkie/dist/.tmp-qtm89409/junkie-3.0.1.tar", last modified: Sat Apr  6 20:08:44 2024, max compression
+gzip compressed data, was "/home/runner/work/junkie/junkie/dist/.tmp-fgn7uigz/junkie-3.0.2.tar", last modified: Wed Apr 24 09:33:03 2024, max compression
```

## Comparing `junkie-3.0.1.tar` & `junkie-3.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:08:44.000000 junkie-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-06 20:08:38.000000 junkie-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-04-06 20:08:44.000000 junkie-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-04-06 20:08:38.000000 junkie-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:08:44.000000 junkie-3.0.1/junkie/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-06 20:08:38.000000 junkie-3.0.1/junkie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-04-06 20:08:38.000000 junkie-3.0.1/junkie/_junkie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:08:44.000000 junkie-3.0.1/junkie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-04-06 20:08:44.000000 junkie-3.0.1/junkie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-06 20:08:44.000000 junkie-3.0.1/junkie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 20:08:44.000000 junkie-3.0.1/junkie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 20:08:44.000000 junkie-3.0.1/junkie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 20:08:44.000000 junkie-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-06 20:08:38.000000 junkie-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:08:44.000000 junkie-3.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 20:08:38.000000 junkie-3.0.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-06 20:08:38.000000 junkie-3.0.1/test/test_bugfix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-06 20:08:38.000000 junkie-3.0.1/test/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-06 20:08:38.000000 junkie-3.0.1/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    14669 2024-04-06 20:08:38.000000 junkie-3.0.1/test/test_junkie.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-06 20:08:38.000000 junkie-3.0.1/test/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-06 20:08:38.000000 junkie-3.0.1/test/test_readme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:33:03.000000 junkie-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 09:32:49.000000 junkie-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-04-24 09:33:03.000000 junkie-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-04-24 09:32:49.000000 junkie-3.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:33:03.000000 junkie-3.0.2/junkie/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-24 09:32:49.000000 junkie-3.0.2/junkie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-04-24 09:32:49.000000 junkie-3.0.2/junkie/_junkie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:33:03.000000 junkie-3.0.2/junkie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-04-24 09:33:03.000000 junkie-3.0.2/junkie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-24 09:33:03.000000 junkie-3.0.2/junkie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:33:03.000000 junkie-3.0.2/junkie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 09:33:03.000000 junkie-3.0.2/junkie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 09:33:03.000000 junkie-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-24 09:32:49.000000 junkie-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:33:03.000000 junkie-3.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:32:49.000000 junkie-3.0.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-24 09:32:49.000000 junkie-3.0.2/test/test_bugfix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-24 09:32:49.000000 junkie-3.0.2/test/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-24 09:32:49.000000 junkie-3.0.2/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14669 2024-04-24 09:32:49.000000 junkie-3.0.2/test/test_junkie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-24 09:32:49.000000 junkie-3.0.2/test/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-24 09:32:49.000000 junkie-3.0.2/test/test_readme.py
```

### Comparing `junkie-3.0.1/LICENSE` & `junkie-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `junkie-3.0.1/PKG-INFO` & `junkie-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junkie
-Version: 3.0.1
+Version: 3.0.2
 Summary: A dependency injection library for beginners and professionals
 Home-page: https://github.com/sealor/junkie
 Author: Stefan Richter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `junkie-3.0.1/README.md` & `junkie-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `junkie-3.0.1/junkie/_junkie.py` & `junkie-3.0.2/junkie/_junkie.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,53 +25,53 @@
         self._exit_stack: Optional[ExitStack] = None
 
         self._instances_by_name: dict = {}
         self._instances_by_name_stack: Junkie._Stack = Junkie._Stack()
         self._instances_by_name_stack.push(self._instances_by_name)
 
         self._instantiation_stack: Junkie._InstantiationStack = Junkie._InstantiationStack()
-        self._cycle_detection_instance_set = set()
 
         self._context["_junkie"] = self
 
     def __getitem__(self, item):
         return self._instances_by_name[item]
 
     def __setitem__(self, key, value):
+        self._instances_by_name = self._instances_by_name_stack.peek()
+
         if key in self._instances_by_name:
             raise JunkieError(f'Instance for "{key}" already exists')
         if key in self._context:
             raise JunkieError(f'Instance for "{key}" already exists in context')
 
         self._instances_by_name[key] = value
 
     def __len__(self) -> int:
         return self._instances_by_name.__len__()
 
     def __iter__(self) -> Iterator:
         return self._instances_by_name.__iter__()
 
     def __contains__(self, item) -> bool:
+        self._instances_by_name = self._instances_by_name_stack.peek()
+
         return self._instances_by_name.__contains__(item)
 
     @contextmanager
     def inject(self, *names_and_factories: Union[str, Callable]) -> Union[Any, Tuple[Any]]:
         LOGGER.debug("inject(%s)", Junkie._LogParams(*names_and_factories))
 
         with ExitStack() as self._exit_stack:
             self._instances_by_name = self._instances_by_name_stack.peek().copy()
-            self._instances_by_name_stack.push(self._instances_by_name)
-
-            if len(names_and_factories) == 1:
-                yield self._build_instance(names_and_factories[0])
-            else:
-                yield self._build_tuple(*names_and_factories)
 
-            self._instances_by_name_stack.pop()
-            self._instances_by_name = self._instances_by_name_stack.peek()
+            with self._instances_by_name_stack.push_temporarily(self._instances_by_name):
+                if len(names_and_factories) == 1:
+                    yield self._build_instance(names_and_factories[0])
+                else:
+                    yield self._build_tuple(*names_and_factories)
 
     def _build_tuple(self, *names_and_factories: Union[str, Callable]) -> Tuple[Any, ...]:
         instances = []
 
         for name_or_factory in names_and_factories:
             instance = self._build_instance(name_or_factory)
             instances.append(instance)
@@ -106,23 +106,29 @@
     def _build_by_factory_function(self, factory_function: Callable, instance_name: Union[str, None]) -> Any:
         if factory_function in BUILTINS:
             raise JunkieError(
                 f"{self._instantiation_stack}"
                 + f'Mapping for "{instance_name}" of builtin type "{get_factory_name(factory_function)}" is missing'
             )
 
-        if factory_function in self._cycle_detection_instance_set:
+        if factory_function in self._instantiation_stack:
             raise JunkieError(
                 f"{self._instantiation_stack}"
                 + f'Dependency cycle detected with "{get_factory_name(factory_function)}()"'
             )
 
-        self._cycle_detection_instance_set.add(factory_function)
-        self._instantiation_stack.push(factory_function)
+        with self._instantiation_stack.push_temporarily(factory_function):
+            instance = self._call_factory_function(factory_function, instance_name)
+
+            if instance_name is not None:
+                self._instances_by_name[instance_name] = instance
 
+            return instance
+
+    def _call_factory_function(self, factory_function, instance_name):
         positional_params, args, keyword_params, kwargs = self._build_parameters(factory_function)
 
         if LOGGER.isEnabledFor(logging.DEBUG):
             log_params = Junkie._LogParams(*positional_params.keys(), *args, **keyword_params, **kwargs)
             LOGGER.debug("%s = %s(%s)", instance_name or "_", get_factory_name(factory_function), log_params)
 
         instance = factory_function(*positional_params.values(), *args, **keyword_params, **kwargs)
@@ -130,20 +136,14 @@
         if hasattr(instance, "__enter__"):
             if LOGGER.isEnabledFor(logging.DEBUG):
                 LOGGER.debug("%s.__enter__()", instance_name or "_")
                 self._exit_stack.push(lambda *exception_details: LOGGER.debug("%s.__exit__()", instance_name or "_"))
 
             instance = self._exit_stack.enter_context(instance)
 
-        if instance_name is not None:
-            self._instances_by_name[instance_name] = instance
-
-        self._instantiation_stack.pop()
-        self._cycle_detection_instance_set.remove(factory_function)
-
         return instance
 
     def _build_parameters(self, factory_function: Callable) -> (OrderedDict, tuple, dict):
         positional_params = OrderedDict()
         args = ()
         keyword_params = OrderedDict()
         kwargs = {}
@@ -225,17 +225,28 @@
 
         def pop(self):
             return self._stack.pop()
 
         def peek(self):
             return self._stack[-1]
 
+        @contextmanager
+        def push_temporarily(self, item):
+            self.push(item)
+            try:
+                yield self
+            finally:
+                self.pop()
+
         def __len__(self):
             return self._stack.__len__()
 
+        def __contains__(self, item):
+            return item in self._stack
+
     class _InstantiationStack(_Stack):
         def __str__(self):
             if len(self._stack) == 0:
                 return ""
 
             return "".join([
                 f'\n{idx * " "}-> {get_factory_name(factory)}() at {self._get_source_info(factory)}'
```

### Comparing `junkie-3.0.1/junkie.egg-info/PKG-INFO` & `junkie-3.0.2/junkie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junkie
-Version: 3.0.1
+Version: 3.0.2
 Summary: A dependency injection library for beginners and professionals
 Home-page: https://github.com/sealor/junkie
 Author: Stefan Richter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `junkie-3.0.1/setup.py` & `junkie-3.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='junkie',
-    version='3.0.1',
+    version='3.0.2',
     packages=setuptools.find_packages(exclude="test"),
     author='Stefan Richter',
     description='A dependency injection library for beginners and professionals',
     url="https://github.com/sealor/junkie",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

### Comparing `junkie-3.0.1/test/test_dict.py` & `junkie-3.0.2/test/test_dict.py`

 * *Files identical despite different names*

### Comparing `junkie-3.0.1/test/test_error.py` & `junkie-3.0.2/test/test_error.py`

 * *Files identical despite different names*

### Comparing `junkie-3.0.1/test/test_junkie.py` & `junkie-3.0.2/test/test_junkie.py`

 * *Files identical despite different names*

### Comparing `junkie-3.0.1/test/test_parameter.py` & `junkie-3.0.2/test/test_parameter.py`

 * *Files identical despite different names*

### Comparing `junkie-3.0.1/test/test_readme.py` & `junkie-3.0.2/test/test_readme.py`

 * *Files identical despite different names*

