# Comparing `tmp/inline_snapshot-0.8.1.tar.gz` & `tmp/inline_snapshot-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inline_snapshot-0.8.1.tar", max compression
+gzip compressed data, was "inline_snapshot-0.8.2.tar", max compression
```

## Comparing `inline_snapshot-0.8.1.tar` & `inline_snapshot-0.8.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1082 2024-02-18 19:11:48.706993 inline_snapshot-0.8.1/LICENSE
--rw-r--r--   0        0        0     4642 2024-04-21 20:44:07.304452 inline_snapshot-0.8.1/README.md
--rw-r--r--   0        0        0      176 2024-04-22 06:54:14.689618 inline_snapshot-0.8.1/inline_snapshot/__init__.py
--rw-r--r--   0        0        0     1400 2024-04-09 10:01:00.849766 inline_snapshot-0.8.1/inline_snapshot/_align.py
--rw-r--r--   0        0        0     5733 2024-04-21 20:44:07.304452 inline_snapshot-0.8.1/inline_snapshot/_change.py
--rw-r--r--   0        0        0      539 2024-02-27 18:46:50.343219 inline_snapshot-0.8.1/inline_snapshot/_config.py
--rw-r--r--   0        0        0     4944 2024-04-21 20:44:07.304452 inline_snapshot-0.8.1/inline_snapshot/_external.py
--rw-r--r--   0        0        0     2779 2024-04-21 20:44:07.304452 inline_snapshot-0.8.1/inline_snapshot/_find_external.py
--rw-r--r--   0        0        0      372 2024-02-27 18:46:50.343219 inline_snapshot-0.8.1/inline_snapshot/_format.py
--rw-r--r--   0        0        0    21627 2024-04-22 06:53:50.245080 inline_snapshot-0.8.1/inline_snapshot/_inline_snapshot.py
--rw-r--r--   0        0        0      452 2024-04-09 10:01:00.849766 inline_snapshot-0.8.1/inline_snapshot/_location.py
--rw-r--r--   0        0        0     5911 2024-04-21 20:44:07.304452 inline_snapshot-0.8.1/inline_snapshot/_rewrite_code.py
--rw-r--r--   0        0        0       64 2024-04-09 10:01:00.849766 inline_snapshot-0.8.1/inline_snapshot/_sentinels.py
--rw-r--r--   0        0        0     3565 2024-04-09 10:01:00.849766 inline_snapshot-0.8.1/inline_snapshot/_utils.py
--rw-r--r--   0        0        0        0 2024-02-27 18:46:50.343219 inline_snapshot-0.8.1/inline_snapshot/py.typed
--rw-r--r--   0        0        0     6477 2024-04-21 20:44:07.304452 inline_snapshot-0.8.1/inline_snapshot/pytest_plugin.py
--rw-r--r--   0        0        0     2640 2024-04-22 06:54:14.713618 inline_snapshot-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     6511 1970-01-01 00:00:00.000000 inline_snapshot-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-02-18 19:11:48.706993 inline_snapshot-0.8.2/LICENSE
+-rw-r--r--   0        0        0     4642 2024-04-24 07:01:03.261658 inline_snapshot-0.8.2/README.md
+-rw-r--r--   0        0        0      176 2024-04-24 19:10:05.207071 inline_snapshot-0.8.2/inline_snapshot/__init__.py
+-rw-r--r--   0        0        0     1400 2024-04-09 10:01:00.849766 inline_snapshot-0.8.2/inline_snapshot/_align.py
+-rw-r--r--   0        0        0     5733 2024-04-21 20:44:07.304452 inline_snapshot-0.8.2/inline_snapshot/_change.py
+-rw-r--r--   0        0        0      539 2024-02-27 18:46:50.343219 inline_snapshot-0.8.2/inline_snapshot/_config.py
+-rw-r--r--   0        0        0     4944 2024-04-21 20:44:07.304452 inline_snapshot-0.8.2/inline_snapshot/_external.py
+-rw-r--r--   0        0        0     2779 2024-04-21 20:44:07.304452 inline_snapshot-0.8.2/inline_snapshot/_find_external.py
+-rw-r--r--   0        0        0      372 2024-02-27 18:46:50.343219 inline_snapshot-0.8.2/inline_snapshot/_format.py
+-rw-r--r--   0        0        0    22110 2024-04-24 19:10:02.339013 inline_snapshot-0.8.2/inline_snapshot/_inline_snapshot.py
+-rw-r--r--   0        0        0      452 2024-04-09 10:01:00.849766 inline_snapshot-0.8.2/inline_snapshot/_location.py
+-rw-r--r--   0        0        0     5911 2024-04-21 20:44:07.304452 inline_snapshot-0.8.2/inline_snapshot/_rewrite_code.py
+-rw-r--r--   0        0        0       64 2024-04-09 10:01:00.849766 inline_snapshot-0.8.2/inline_snapshot/_sentinels.py
+-rw-r--r--   0        0        0     3565 2024-04-09 10:01:00.849766 inline_snapshot-0.8.2/inline_snapshot/_utils.py
+-rw-r--r--   0        0        0        0 2024-02-27 18:46:50.343219 inline_snapshot-0.8.2/inline_snapshot/py.typed
+-rw-r--r--   0        0        0     6417 2024-04-24 19:10:02.339013 inline_snapshot-0.8.2/inline_snapshot/pytest_plugin.py
+-rw-r--r--   0        0        0     2640 2024-04-24 19:10:05.223071 inline_snapshot-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     6511 1970-01-01 00:00:00.000000 inline_snapshot-0.8.2/PKG-INFO
```

### Comparing `inline_snapshot-0.8.1/LICENSE` & `inline_snapshot-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.1/README.md` & `inline_snapshot-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.1/inline_snapshot/_align.py` & `inline_snapshot-0.8.2/inline_snapshot/_align.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.1/inline_snapshot/_change.py` & `inline_snapshot-0.8.2/inline_snapshot/_change.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.1/inline_snapshot/_config.py` & `inline_snapshot-0.8.2/inline_snapshot/_config.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.1/inline_snapshot/_external.py` & `inline_snapshot-0.8.2/inline_snapshot/_external.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.1/inline_snapshot/_find_external.py` & `inline_snapshot-0.8.2/inline_snapshot/_find_external.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.1/inline_snapshot/_inline_snapshot.py` & `inline_snapshot-0.8.2/inline_snapshot/_inline_snapshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 
 snapshots = {}  # type: Dict[Tuple[int, int], Snapshot]
 
 _active = False
 
 _files_with_snapshots: Set[str] = set()
 
+_missing_values = 0
+
 
 class Flags:
     """
     fix: the value needs to be changed to pass the tests
     update: the value should be updated because the token-stream has changed
     create: the snapshot is empty `snapshot()`
     trim: the snapshot contains more values than neccessary. 1 could be trimmed in `5 in snapshot([1,5])`.
@@ -228,14 +230,18 @@
         return not isinstance(value, dirty_equals.DirtyEquals)
 
 
 class EqValue(GenericValue):
     _current_op = "x == snapshot"
 
     def __eq__(self, other):
+        global _missing_values
+        if self._old_value is undefined:
+            _missing_values += 1
+
         other = copy.deepcopy(other)
 
         if self._new_value is undefined:
             self._new_value = other
 
         return self._visible_value() == other
 
@@ -384,14 +390,17 @@
     """Generic implementation for <=, >="""
 
     @staticmethod
     def cmp(a, b):
         raise NotImplemented
 
     def _generic_cmp(self, other):
+        global _missing_values
+        if self._old_value is undefined:
+            _missing_values += 1
         other = copy.deepcopy(other)
 
         if self._new_value is undefined:
             self._new_value = other
         else:
             self._new_value = (
                 self._new_value if self.cmp(self._new_value, other) else other
@@ -470,14 +479,18 @@
     __ge__ = MinMaxValue._generic_cmp
 
 
 class CollectionValue(GenericValue):
     _current_op = "x in snapshot"
 
     def __contains__(self, item):
+        global _missing_values
+        if self._old_value is undefined:
+            _missing_values += 1
+
         item = copy.deepcopy(item)
 
         if self._new_value is undefined:
             self._new_value = [item]
         else:
             if item not in self._new_value:
                 self._new_value.append(item)
@@ -532,19 +545,22 @@
             )
 
 
 class DictValue(GenericValue):
     _current_op = "snapshot[key]"
 
     def __getitem__(self, index):
+        global _missing_values
+
         if self._new_value is undefined:
             self._new_value = {}
 
         old_value = self._old_value
         if old_value is undefined:
+            _missing_values += 1
             old_value = {}
 
         child_node = None
         if self._ast_node is not None:
             assert isinstance(self._ast_node, ast.Dict)
             if index in old_value:
                 pos = list(old_value.keys()).index(index)
@@ -560,14 +576,15 @@
     def _new_code(self):
         return (
             "{"
             + ", ".join(
                 [
                     f"{self._value_to_code(k)}: {v._new_code()}"
                     for k, v in self._new_value.items()
+                    if not isinstance(v, UndecidedValue)
                 ]
             )
             + "}"
         )
 
     def _get_changes(self) -> Iterator[Change]:
 
@@ -585,15 +602,17 @@
                 yield from self._new_value[key]._get_changes()
             else:
                 # delete entries
                 yield Delete("trim", self._source, node, self._old_value[key])
 
         to_insert = []
         for key, new_value_element in self._new_value.items():
-            if key not in self._old_value:
+            if key not in self._old_value and not isinstance(
+                new_value_element, UndecidedValue
+            ):
                 # add new values
                 to_insert.append((key, new_value_element._new_code()))
 
         if to_insert:
             new_code = [(self._value_to_code(k), v) for k, v in to_insert]
             yield DictInsert(
                 "create",
@@ -603,16 +622,14 @@
                 new_code,
                 to_insert,
             )
 
 
 T = TypeVar("T")
 
-found_snapshots = []
-
 
 class ReprWrapper:
     def __init__(self, func):
         self.func = func
 
     def __call__(self, *args, **kwargs):
         return self.func(*args, **kwargs)
@@ -673,18 +690,15 @@
     if key not in snapshots:
         node = expr.node
         if node is None:
             # we can run without knowing of the calling expression but we will not be able to fix code
             snapshots[key] = Snapshot(obj, None)
         else:
             assert isinstance(node, ast.Call)
-            assert isinstance(node.func, ast.Name)
-            assert node.func.id == "snapshot"
             snapshots[key] = Snapshot(obj, expr)
-        found_snapshots.append(snapshots[key])
 
     return snapshots[key]._value
 
 
 def used_externals(tree):
     if sys.version_info < (3, 8):
         return [
@@ -730,23 +744,27 @@
                 except:
                     return
             else:
                 return
 
             assert self._expr is not None
 
-            tokens = list(self._expr.source.asttokens().get_tokens(self._expr.node))
-            assert tokens[0].string == "snapshot"
-            assert tokens[1].string == "("
+            call = self._expr.node
+            tokens = list(self._expr.source.asttokens().get_tokens(call))
+
+            assert isinstance(call, ast.Call)
+            assert len(call.args) == 0
+            assert len(call.keywords) == 0
+            assert tokens[-2].string == "("
             assert tokens[-1].string == ")"
 
             change = ChangeRecorder.current.new_change()
             change.set_tags("inline_snapshot")
             change.replace(
-                (end_of(tokens[1]), start_of(tokens[-1])),
+                (end_of(tokens[-2]), start_of(tokens[-1])),
                 new_code,
                 filename=self._filename,
             )
             return
 
         changes = self._value._get_changes()
         apply_all(
```

### Comparing `inline_snapshot-0.8.1/inline_snapshot/_rewrite_code.py` & `inline_snapshot-0.8.2/inline_snapshot/_rewrite_code.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.1/inline_snapshot/_utils.py` & `inline_snapshot-0.8.2/inline_snapshot/_utils.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.1/inline_snapshot/pytest_plugin.py` & `inline_snapshot-0.8.2/inline_snapshot/pytest_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import pytest
 
 from . import _config
 from . import _external
 from . import _find_external
 from . import _inline_snapshot
 from ._find_external import ensure_import
-from ._inline_snapshot import undefined
 from ._inline_snapshot import used_externals
 from ._rewrite_code import ChangeRecorder
 
 
 def pytest_addoption(parser):
     group = parser.getgroup("inline-snapshot")
 
@@ -64,20 +63,22 @@
         ]
 
     _external.storage.prune_new_files()
 
 
 @pytest.fixture(autouse=True)
 def snapshot_check():
-    found = _inline_snapshot.found_snapshots = []
+    _inline_snapshot._missing_values = 0
     yield
-    missing_values = sum(snapshot._value._old_value is undefined for snapshot in found)
-    if missing_values and not _inline_snapshot._update_flags.create:
+
+    missing_values = _inline_snapshot._missing_values
+
+    if missing_values != 0 and not _inline_snapshot._update_flags.create:
         pytest.fail(
-            "your snapshot is missing a value run pytest with --inline-snapshot=create to create the value",
+            f"your snapshot is missing {missing_values} value run pytest with --inline-snapshot=create to create the value",
             pytrace=False,
         )
 
 
 def pytest_assertrepr_compare(config, op, left, right):
     results = []
     if isinstance(left, _inline_snapshot.GenericValue):
```

### Comparing `inline_snapshot-0.8.1/pyproject.toml` & `inline_snapshot-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 ]
 description = "golden master/snapshot/approval testing library which puts the values right into your source code"
 keywords = ["pytest", "testing", "snapshot", "approval", "golden-master"]
 license = "MIT"
 name = "inline-snapshot"
 readme = "README.md"
 repository = "https://github.com/15r10nk/inline-snapshots"
-version = "0.8.1"
+version = "0.8.2"
 
 [tool.poetry.dependencies]
 asttokens = ">=2.0.5"
 black = ">=23.3.0"
 click = ">=8.1.4"
 executing = ">=2.0.0"
 python = ">=3.7"
```

### Comparing `inline_snapshot-0.8.1/PKG-INFO` & `inline_snapshot-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inline-snapshot
-Version: 0.8.1
+Version: 0.8.2
 Summary: golden master/snapshot/approval testing library which puts the values right into your source code
 Home-page: https://github.com/15r10nk/inline-snapshots
 License: MIT
 Keywords: pytest,testing,snapshot,approval,golden-master
 Author: Frank Hoffmann
 Author-email: 15r10nk@polarbit.de
 Requires-Python: >=3.7
```

