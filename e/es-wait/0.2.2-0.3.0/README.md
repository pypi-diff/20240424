# Comparing `tmp/es_wait-0.2.2.tar.gz` & `tmp/es_wait-0.3.0.tar.gz`

## Comparing `es_wait-0.2.2.tar` & `es_wait-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 es_wait-0.2.2/pytest.ini
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 es_wait-0.2.2/src/es_wait/__init__.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 es_wait-0.2.2/src/es_wait/args.py
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 es_wait-0.2.2/src/es_wait/base.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 es_wait-0.2.2/src/es_wait/exists.py
--rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 es_wait-0.2.2/src/es_wait/health.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 es_wait-0.2.2/src/es_wait/relocate.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 es_wait-0.2.2/src/es_wait/restore.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 es_wait-0.2.2/src/es_wait/snapshot.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 es_wait-0.2.2/src/es_wait/task.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 es_wait-0.2.2/.gitignore
--rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.2.2/LICENSE
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.2.2/README.md
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 es_wait-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 es_wait-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 es_wait-0.3.0/pytest.ini
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 es_wait-0.3.0/src/es_wait/__init__.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 es_wait-0.3.0/src/es_wait/args.py
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 es_wait-0.3.0/src/es_wait/base.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 es_wait-0.3.0/src/es_wait/exists.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 es_wait-0.3.0/src/es_wait/health.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 es_wait-0.3.0/src/es_wait/relocate.py
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 es_wait-0.3.0/src/es_wait/restore.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 es_wait-0.3.0/src/es_wait/snapshot.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 es_wait-0.3.0/src/es_wait/task.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 es_wait-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.3.0/LICENSE
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.3.0/README.md
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 es_wait-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 es_wait-0.3.0/PKG-INFO
```

### Comparing `es_wait-0.2.2/src/es_wait/args.py` & `es_wait-0.3.0/src/es_wait/args.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.2.2/src/es_wait/base.py` & `es_wait-0.3.0/src/es_wait/base.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.2.2/src/es_wait/exists.py` & `es_wait-0.3.0/src/es_wait/exists.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.2.2/src/es_wait/health.py` & `es_wait-0.3.0/src/es_wait/health.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             action: t.Literal[
                 'allocation', 'cluster_routing', 'mount', 'replicas', 'shrink'] = None,
             pause: float = 1.5,
             timeout: float = 15,
             ) -> None:
         super().__init__(client=client, action=action, pause=pause, timeout=timeout)
         self.logger = logging.getLogger('es_wait.Health')
-        self.empty_check(action)
+        self.empty_check('action')
         self.checkid = self.getcheckid
 
     @property
     def argmap(self) -> t.Union[t.Dict[str, int], t.Dict[str, str]]:
         """This is a little way to ensure many possibilities come down to one"""
         if self.action in self.RELO_ACTIONS:
             return self.RELO_ARGS
```

### Comparing `es_wait-0.2.2/src/es_wait/relocate.py` & `es_wait-0.3.0/src/es_wait/relocate.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             pause: float = 9,
             timeout: float = -1,
             name: str = None,
         ) -> None:
         super().__init__(client=client, action=action, pause=pause, timeout=timeout)
         self.logger = logging.getLogger('es_wait.Health')
         self.name = name
-        self.empty_check(name)
+        self.empty_check('name')
         self.checkid = f'check for the {self.name} index relocation process to complete'
 
     @property
     def check(self) -> bool:
         """
         This function calls `client.cluster.` :py:meth:`~.elasticsearch.client.ClusterClient.state`
         with a given index to check if all of the shards for that index are in the ``STARTED``
```

### Comparing `es_wait-0.2.2/src/es_wait/restore.py` & `es_wait-0.3.0/src/es_wait/restore.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             pause: float = 9,
             timeout: float = -1,
             index_list: t.Sequence[str] = None,
         ) -> None:
         super().__init__(client=client, action=action, pause=pause, timeout=timeout)
         self.logger = logging.getLogger('es_wait.Snapshot')
         self.index_list = index_list
-        self.empty_check(index_list)
+        self.empty_check('index_list')
         self.checkid = 'check for completion of index_list restoration from snapshot'
 
     @property
     def check(self) -> bool:
         """
         Calls `client.indices.` :py:meth:`~.elasticsearch.client.IndicesClient.recovery`
         with a list of indices to check for complete recovery.  It will return ``True`` if recovery
```

### Comparing `es_wait-0.2.2/src/es_wait/snapshot.py` & `es_wait-0.3.0/src/es_wait/snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
             snapshot: str = None,
             repository: str = None,
         ) -> None:
         super().__init__(client=client, action=action, pause=pause, timeout=timeout)
         self.logger = logging.getLogger('es_wait.Snapshot')
         self.snapshot = snapshot
         self.repository = repository
-        self.empty_check(snapshot)
-        self.empty_check(repository)
+        self.empty_check('snapshot')
+        self.empty_check('repository')
         self.checkid = f'check for snapshot {self.snapshot} completion'
 
     @property
     def check(self) -> bool:
         """
         This function calls `client.snapshot.` :py:meth:`~.elasticsearch.client.SnapshotClient.get`
         and tests to see whether the snapshot is complete, and if so, with what status.  It will log
```

### Comparing `es_wait-0.2.2/src/es_wait/task.py` & `es_wait-0.3.0/src/es_wait/task.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.2.2/.gitignore` & `es_wait-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `es_wait-0.2.2/LICENSE` & `es_wait-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `es_wait-0.2.2/pyproject.toml` & `es_wait-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `es_wait-0.2.2/PKG-INFO` & `es_wait-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: es-wait
-Version: 0.2.2
+Version: 0.3.0
 Summary: Helping you wait for certain Elasticsearch tasks and API calls to finish
 Project-URL: Documentation, https://github.com/untergeek/es-wait#readme
 Project-URL: Issues, https://github.com/untergeek/es-wait/issues
 Project-URL: Source, https://github.com/untergeek/es-wait
 Author-email: Aaron Mildenstein <untergeek@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
```

