# Comparing `tmp/antelope_background-0.2.4.tar.gz` & `tmp/antelope_background-0.2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antelope_background-0.2.4.tar", last modified: Thu Apr 18 21:41:33 2024, max compression
+gzip compressed data, was "antelope_background-0.2.4.1.tar", last modified: Wed Apr 24 21:11:56 2024, max compression
```

## Comparing `antelope_background-0.2.4.tar` & `antelope_background-0.2.4.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:41:33.234599 antelope_background-0.2.4/
--rw-r--r--   0 b          (500) b          (506)     1520 2020-09-29 23:44:37.000000 antelope_background-0.2.4/LICENSE
--rw-r--r--   0 b          (500) b          (506)     3821 2024-04-18 21:41:33.234599 antelope_background-0.2.4/PKG-INFO
--rw-r--r--   0 b          (500) b          (506)     3471 2021-03-10 07:59:31.000000 antelope_background-0.2.4/README.md
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:41:33.231266 antelope_background-0.2.4/antelope_background/
--rw-r--r--   0 b          (500) b          (506)     2127 2024-03-13 21:49:28.000000 antelope_background-0.2.4/antelope_background/__init__.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:41:33.231266 antelope_background-0.2.4/antelope_background/background/
--rw-r--r--   0 b          (500) b          (506)      112 2024-03-13 21:49:28.000000 antelope_background-0.2.4/antelope_background/background/__init__.py
--rw-r--r--   0 b          (500) b          (506)    24828 2023-12-16 05:38:33.000000 antelope_background-0.2.4/antelope_background/background/flat_background.py
--rw-r--r--   0 b          (500) b          (506)    10778 2024-04-17 22:48:03.000000 antelope_background-0.2.4/antelope_background/background/implementation.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:41:33.231266 antelope_background-0.2.4/antelope_background/background/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2018-07-20 18:48:36.000000 antelope_background-0.2.4/antelope_background/background/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     1621 2020-09-29 23:57:25.000000 antelope_background-0.2.4/antelope_background/background/tests/test_flat_background.py
--rw-r--r--   0 b          (500) b          (506)      145 2021-03-10 07:42:08.000000 antelope_background-0.2.4/antelope_background/background/tests/test_implementation.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:41:33.234599 antelope_background-0.2.4/antelope_background/engine/
--rw-r--r--   0 b          (500) b          (506)      346 2024-03-13 21:47:33.000000 antelope_background-0.2.4/antelope_background/engine/__init__.py
--rw-r--r--   0 b          (500) b          (506)    29785 2024-03-15 22:38:06.000000 antelope_background-0.2.4/antelope_background/engine/background_engine.py
--rw-r--r--   0 b          (500) b          (506)     2217 2021-01-29 21:46:30.000000 antelope_background-0.2.4/antelope_background/engine/emission.py
--rw-r--r--   0 b          (500) b          (506)     4612 2024-03-13 00:24:04.000000 antelope_background-0.2.4/antelope_background/engine/product_flow.py
--rw-r--r--   0 b          (500) b          (506)    10150 2018-07-20 18:48:36.000000 antelope_background-0.2.4/antelope_background/engine/tarjan_stack.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:41:33.234599 antelope_background-0.2.4/antelope_background/providers/
--rw-r--r--   0 b          (500) b          (506)      178 2024-03-13 21:49:57.000000 antelope_background-0.2.4/antelope_background/providers/__init__.py
--rw-r--r--   0 b          (500) b          (506)     3075 2024-03-13 22:07:13.000000 antelope_background-0.2.4/antelope_background/providers/bm_static.py
--rw-r--r--   0 b          (500) b          (506)     1102 2024-03-14 00:30:16.000000 antelope_background-0.2.4/antelope_background/providers/check_terms.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-18 21:41:33.234599 antelope_background-0.2.4/antelope_background.egg-info/
--rw-r--r--   0 b          (500) b          (506)     3821 2024-04-18 21:41:33.000000 antelope_background-0.2.4/antelope_background.egg-info/PKG-INFO
--rw-r--r--   0 b          (500) b          (506)      926 2024-04-18 21:41:33.000000 antelope_background-0.2.4/antelope_background.egg-info/SOURCES.txt
--rw-r--r--   0 b          (500) b          (506)        1 2024-04-18 21:41:33.000000 antelope_background-0.2.4/antelope_background.egg-info/dependency_links.txt
--rw-r--r--   0 b          (500) b          (506)       44 2024-04-18 21:41:33.000000 antelope_background-0.2.4/antelope_background.egg-info/requires.txt
--rw-r--r--   0 b          (500) b          (506)       20 2024-04-18 21:41:33.000000 antelope_background-0.2.4/antelope_background.egg-info/top_level.txt
--rw-r--r--   0 b          (500) b          (506)       38 2024-04-18 21:41:33.234599 antelope_background-0.2.4/setup.cfg
--rw-r--r--   0 b          (500) b          (506)     1690 2024-04-17 22:51:41.000000 antelope_background-0.2.4/setup.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-24 21:11:56.163890 antelope_background-0.2.4.1/
+-rw-r--r--   0 b          (500) b          (506)     1520 2020-09-29 23:44:37.000000 antelope_background-0.2.4.1/LICENSE
+-rw-r--r--   0 b          (500) b          (506)     3825 2024-04-24 21:11:56.163890 antelope_background-0.2.4.1/PKG-INFO
+-rw-r--r--   0 b          (500) b          (506)     3471 2021-03-10 07:59:31.000000 antelope_background-0.2.4.1/README.md
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-24 21:11:56.163890 antelope_background-0.2.4.1/antelope_background/
+-rw-r--r--   0 b          (500) b          (506)     2138 2024-04-24 21:11:34.000000 antelope_background-0.2.4.1/antelope_background/__init__.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-24 21:11:56.163890 antelope_background-0.2.4.1/antelope_background/background/
+-rw-r--r--   0 b          (500) b          (506)      112 2024-03-13 21:49:28.000000 antelope_background-0.2.4.1/antelope_background/background/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    24955 2024-04-24 21:11:34.000000 antelope_background-0.2.4.1/antelope_background/background/flat_background.py
+-rw-r--r--   0 b          (500) b          (506)    10778 2024-04-17 22:48:03.000000 antelope_background-0.2.4.1/antelope_background/background/implementation.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-24 21:11:56.163890 antelope_background-0.2.4.1/antelope_background/background/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2018-07-20 18:48:36.000000 antelope_background-0.2.4.1/antelope_background/background/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     1621 2020-09-29 23:57:25.000000 antelope_background-0.2.4.1/antelope_background/background/tests/test_flat_background.py
+-rw-r--r--   0 b          (500) b          (506)      145 2021-03-10 07:42:08.000000 antelope_background-0.2.4.1/antelope_background/background/tests/test_implementation.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-24 21:11:56.163890 antelope_background-0.2.4.1/antelope_background/engine/
+-rw-r--r--   0 b          (500) b          (506)      346 2024-03-13 21:47:33.000000 antelope_background-0.2.4.1/antelope_background/engine/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    32815 2024-04-24 21:11:34.000000 antelope_background-0.2.4.1/antelope_background/engine/background_engine.py
+-rw-r--r--   0 b          (500) b          (506)     2217 2021-01-29 21:46:30.000000 antelope_background-0.2.4.1/antelope_background/engine/emission.py
+-rw-r--r--   0 b          (500) b          (506)     4612 2024-03-13 00:24:04.000000 antelope_background-0.2.4.1/antelope_background/engine/product_flow.py
+-rw-r--r--   0 b          (500) b          (506)    10254 2024-04-24 21:11:34.000000 antelope_background-0.2.4.1/antelope_background/engine/tarjan_stack.py
+-rw-r--r--   0 b          (500) b          (506)     6835 2024-04-24 21:11:34.000000 antelope_background-0.2.4.1/antelope_background/lci_tester.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-24 21:11:56.163890 antelope_background-0.2.4.1/antelope_background/providers/
+-rw-r--r--   0 b          (500) b          (506)      178 2024-03-13 21:49:57.000000 antelope_background-0.2.4.1/antelope_background/providers/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     6074 2024-04-24 21:11:34.000000 antelope_background-0.2.4.1/antelope_background/providers/bm_static.py
+-rw-r--r--   0 b          (500) b          (506)     1113 2024-04-24 21:11:34.000000 antelope_background-0.2.4.1/antelope_background/providers/check_terms.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-04-24 21:11:56.163890 antelope_background-0.2.4.1/antelope_background.egg-info/
+-rw-r--r--   0 b          (500) b          (506)     3825 2024-04-24 21:11:56.000000 antelope_background-0.2.4.1/antelope_background.egg-info/PKG-INFO
+-rw-r--r--   0 b          (500) b          (506)      960 2024-04-24 21:11:56.000000 antelope_background-0.2.4.1/antelope_background.egg-info/SOURCES.txt
+-rw-r--r--   0 b          (500) b          (506)        1 2024-04-24 21:11:56.000000 antelope_background-0.2.4.1/antelope_background.egg-info/dependency_links.txt
+-rw-r--r--   0 b          (500) b          (506)       46 2024-04-24 21:11:56.000000 antelope_background-0.2.4.1/antelope_background.egg-info/requires.txt
+-rw-r--r--   0 b          (500) b          (506)       20 2024-04-24 21:11:56.000000 antelope_background-0.2.4.1/antelope_background.egg-info/top_level.txt
+-rw-r--r--   0 b          (500) b          (506)       38 2024-04-24 21:11:56.163890 antelope_background-0.2.4.1/setup.cfg
+-rw-r--r--   0 b          (500) b          (506)     1852 2024-04-24 21:04:43.000000 antelope_background-0.2.4.1/setup.py
```

### Comparing `antelope_background-0.2.4/LICENSE` & `antelope_background-0.2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.4/PKG-INFO` & `antelope_background-0.2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: antelope_background
-Version: 0.2.4
+Version: 0.2.4.1
 Home-page: https://github.com/AntelopeLCA/background
 Author: Brandon Kuczenski
 Author-email: bkuczenski@ucsb.edu
 License: BSD 3-clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: antelope_core>=0.2.4
+Requires-Dist: antelope_core>=0.2.4.1
 Requires-Dist: scipy>=1.5
 Requires-Dist: numpy>=1.19
 
 # background
 Background LCI implementation including Tarjan Ordering.
 
 This is kept as a separate repo because it is the only place `numpy/scipy` is required.  The
```

### Comparing `antelope_background-0.2.4/README.md` & `antelope_background-0.2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.4/antelope_background/__init__.py` & `antelope_background-0.2.4.1/antelope_background/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,14 @@
 
     :param res: data resource providing index interface.  If the background has not been generated, then the index
      must return entity references that can also provide full inventory information.
     :param source: optional file to load/save ordered matrices (if present and exists, will load; if present and not
      exists, will save after construction)
     :return:
     """
-    if os.path.exists(source):
+    if source and os.path.exists(source):
         return TarjanBackgroundImplementation.from_file(res, source, **kwargs)
     else:
         tb = TarjanBackground(source, save_after=True, **kwargs)
         bg = tb.make_interface('background')
         bg.setup_bm(res.make_interface('index'))
         return bg
```

### Comparing `antelope_background-0.2.4/antelope_background/background/flat_background.py` & `antelope_background-0.2.4.1/antelope_background/background/flat_background.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,22 +179,23 @@
 
 
 class FlatBackground(object):
     """
     Static, ordered background stored in an easily serializable way
     """
     @classmethod
-    def from_index(cls, index, quiet=True, **kwargs):
+    def from_index(cls, index, quiet=True, preferred=None, **kwargs):
         """
         :param index: an index interface with operable processes() and terminate()
         :param quiet: passed to cls
+        :param preferred: a preferred-provider dict as specified in BackgroundEngine init
         :param kwargs: passed to add_all_ref_products()
         :return:
         """
-        be = BackgroundEngine(index)
+        be = BackgroundEngine(index, preferred=preferred)
         be.add_all_ref_products(**kwargs)
         return cls.from_background_engine(be, quiet=quiet)
 
     @classmethod
     def from_background_engine(cls, be, **kwargs):
         af, ad, bf = be.make_foreground()
```

### Comparing `antelope_background-0.2.4/antelope_background/background/implementation.py` & `antelope_background-0.2.4.1/antelope_background/background/implementation.py`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.4/antelope_background/background/tests/test_flat_background.py` & `antelope_background-0.2.4.1/antelope_background/background/tests/test_flat_background.py`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.4/antelope_background/engine/background_engine.py` & `antelope_background-0.2.4.1/antelope_background/engine/background_engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,57 @@
 """
 Tarjan's strongly connected components algorithm is recursive.  Python doesn't do well with deep recursion, so
-ultimately this code will need to be implemented on a more grown-up language.  For now, however, the recursion
-limit test that ships with python reported a segfault at a recursion limit exceeding 19100 -- bigger than ecoinvent!
-So for the time being we are safe.
-may need to use threading to go higher (see http://stackoverflow.com/questions/2917210/)
-Validate recursion depth on a given system using PYTHONROOT/Tools/scripts/find_recursionlimit.py
+we will re-implement the recursion as an iteration with a stack:
+https://www.refactoring.com/catalog/replaceRecursionWithIteration.html
+
 """
-import sys  # for recursion limit
 import re  # for product_flows search
 
+from collections import deque
+
 import numpy as np
 from scipy.sparse import csr_matrix  # , csc_matrix,
 
 from antelope import comp_dir
+from antelope.refs import ProcessRef
 from antelope_core.contexts import NullContext
 
 from .tarjan_stack import TarjanStack
 from .product_flow import ProductFlow, NoMatchingReference
 from .emission import Emission
 
 
-MAX_SAFE_RECURSION_LIMIT = 18000  # this should be validated using
+class Marker:
+    """
+    Marker objects for interpreting the recursion queue
+    """
+    marker = None
+
+
+class ParentMarker(Marker):
+    """
+    Used to mark the beginning of a new parent
+    """
+    marker = 'parent'
+
+
+class RecurseMarker(Marker):
+    """
+    Used to mark the exchange that begins entry into recursion
+    """
+    marker = 'recurse'
+    def __init__(self, term):
+        self.term = term
+
+
+class DequeError(Exception):
+    """
+    Something has gone wrong
+    """
+    pass
 
 
 class RepeatAdjustment(Exception):
     pass
 
 
 class TerminationError(Exception):
@@ -86,95 +113,81 @@
         return self._term
 
 
 class NoAllocation(Exception):
     pass
 
 
-'''
-def is_elementary(flow):
-    """
-    in future, this sholud lookup to a standalone compartment manager
-    :param flow:
-    :return:
-    """
-    comp = flow['Compartment'][0]
-    if comp == 'air' or comp == 'water' or comp == 'soil' or comp == 'natural resource':
-        # Ecoinvent + USLCI
-        return True
-    elif comp == 'resource':
-        # USLCI
-        return True
-    return False
-'''
-
-
 class BackgroundEngine(object):
     """
     Class for converting a collection of linked processes into a coherent technology matrix.
     """
-    def __init__(self, index_interface, quiet=True):
-        """
+    def __init__(self, query, quiet=True, preferred=None):
         """
-        self.fg = index_interface
-        self.preferred_processes = {None: []}  # use to resolve termination errors. dict of flow_ref -> process
+        Construct an ordered background matrix from a query that implements basic, index and exchange.
+        Required routes:
+         query.get() <- for all processes and flows
+         query.count('process')
+         query.processes() <- complete
+         flow.targets()
+         process.references()
+         process.reference(ref_flow)
+         process.inventory(ref_flow)
+
+         process.__getitem__() <-- SpatialScope (only used in rare cases)
+
+        :param query:
+        :param quiet:
+        :param preferred: a dict mapping flow external refs to their preferred processes (by external ref).
+        The special entry None should map to a list of process external_refs that should be preferred whenever they
+        are found (in the order of preference)
+        """
+        self.fg = query
+        self._preferred_processes = {None: []}  # use to resolve termination errors. dict of flow_ref -> process
+        if preferred:
+            self._preferred_processes.update(preferred)
         self.missing_references = []
         self._quiet = quiet
-        self._lowlinks = dict()  # dict mapping product_flow key to lowlink -- which is a key into TarjanStack.sccs
+        self._lowlinks = dict()  # dict mapping product_flow key to lowlink (int) -- which is key into TarjanStack.sccs
 
         self.tstack = TarjanStack()  # ordering of sccs
 
         # hold exchanges before updating component graph
         self._interior_incoming = []  # terminated entries -> added to the component graph
         self._cutoff_incoming = []  # entries with no termination -> emissions
 
         # _interior_incoming entries get sorted into:
         self._interior = []  # MatrixEntries whose parent (column) is background - A*
         self._foreground = []  # MatrixEntries whose parent is upstream of the background - Af + Ad
         self._bg_emission = []  # CutoffEntries whose parent is background - B*
         self._cutoff = []  # CutoffEntries whose parent is foreground - Bf
 
-        self._surplus_coproducts = dict()  # maps surplus coproducts to their reference products
-
         self._product_flows = dict()  # maps product_flow.key to index-- being position in _pf_index
         self._pf_index = []  # maps index to product_flow in order added
 
         self._a_matrix = None  # includes only interior exchanges -- dependencies in _interior
         self._b_matrix = None  # SciPy.csc_matrix for bg only
 
         self._all_added = False
 
-        self._rec_limit = self.fg.count('process')
-        if self.required_recursion_limit > MAX_SAFE_RECURSION_LIMIT:
-            raise EnvironmentError('This database may require too high a recursion limit-- time to learn lisp.')
+        self._r_stack = deque()  # recursion stack
+        self._p_stack = list()  # recursion parents
 
         self._emissions = dict()  # maps emission key to index
         self._ef_index = []  # maps index to emission
 
     def _print(self, *args):
         if not self._quiet:
             print(*args)
 
     @property
     def lci_db(self):
         return self._a_matrix, self._b_matrix
 
     @property
-    def surplus_coproducts(self):
-        return self._surplus_coproducts
-
-    @property
-    def fully_allocated(self):
-        return len(self._surplus_coproducts) == 0
-
-    @property
-    def required_recursion_limit(self):
-        return max(sys.getrecursionlimit(), self._rec_limit)
-
-    @property
     def mdim(self):
         return len(self._emissions)
 
     @property
     def emissions(self):
         return self._ef_index
 
@@ -191,18 +204,20 @@
         self._product_flows[pf.key] = pf.index
         self._set_lowlink(pf, pf.index)
         self._pf_index.append(pf)
         self.tstack.add_to_stack(pf)
 
     def _rm_product_flow_children(self, bad_pf):
         """
-        This needs desperately to be tested
+        Used only to back-out the links in-progress when a TerminationError is encountered.
+        This needs desperately to be tested. U
         :param bad_pf:
         :return:
         """
+        self._r_stack.clear()
         while len(self._interior_incoming) > 0:
             pf = self.tstack.pop_from_stack()
             self._print('!!!removing %s' % pf)
             while 1:
                 z = self._pf_index.pop()
                 self._lowlinks.pop(z.key)
                 self._product_flows.pop(z.key)
@@ -220,15 +235,16 @@
         """
         Sets lowlink to be the lower of the existing lowlink or the supplied lowlink
         :param pf:
         :param lowlink:
         :return:
         """
         if pf.key in self._lowlinks:
-            self._lowlinks[pf.key] = min(self._lowlink(pf), lowlink)
+            existing = self._lowlinks[pf.key]
+            self._lowlinks[pf.key] = min(existing, lowlink)
         else:
             self._lowlinks[pf.key] = lowlink
 
     def check_product_flow(self, flow, termination):
         """
         returns the product flow if it exists, or None if it doesn't
         :param flow:
@@ -270,48 +286,50 @@
         else:
             index = len(self._ef_index)
             ef = Emission(index, flow, direction, cx)
             self._emissions[ef.key] = index
             self._ef_index.append(ef)
             return ef
 
-    def terminate(self, exch, strategy):
+    def terminate(self, exch, strategy) -> ProcessRef | None:
         """
         Find the ProductFlow that terminates a given exchange.  If an exchange has an explicit termination, use it.
         Else if flow / direction / term are already seen, use it.
         Else if flow is found in list of preferred providers, use designated provider (None -> cutoff)
         lastly, ask archive for valid targets. If this list has length != 1, defer to designated strategy or raise error
         :param exch:
         :param strategy:
         :return:
         """
         if isinstance(exch.termination, str):
             return self.fg.get(exch.termination)
         else:
             if (exch.flow.external_ref, exch.direction, exch.termination) in self._emissions:
                 return None
-            if exch.flow.external_ref in self.preferred_processes:
-                term = self.preferred_processes[exch.flow.external_ref]
+            if exch.flow.external_ref in self._preferred_processes:
+                term = self._preferred_processes[exch.flow.external_ref]
                 if term is None:
                     return None
                 if not hasattr(term, 'entity_type'):
                     term = self.fg.get(term)
                 if term.entity_type != 'process':
                     raise TypeError('%s: Bad preferred provider %s' % (exch.flow.external_ref, term))
                 return term
 
             terms = [t for t in self.fg.targets(exch.flow, direction=exch.direction)]
             if len(terms) == 0:
                 return None
             elif len(terms) == 1:
                 term = terms[0]
             else:
-                for pref in self.preferred_processes[None]:
-                    if pref in terms:
-                        return pref
+                t_map = {t.external_ref: t for t in terms}
+                pref = self._preferred_processes[None]
+                for p in pref:
+                    if p in t_map:
+                        return t_map[p]
                 if strategy == 'abort':
                     print('flow: %s\nAmbiguous termination found for %s: %s' % (exch.flow.external_ref,
                                                                                 exch.direction, exch.flow))
                     raise TerminationError
                 elif strategy == 'first':
                     term = terms[0]
                 elif strategy == 'last':
@@ -319,15 +337,15 @@
                 elif strategy == 'cutoff':
                     return None
                 elif strategy == 'mix':
                     raise NotImplementedError('MIX not presently supported (for some reason)')
                     # return self.fg.mix(exch.flow, exch.direction)
                 else:
                     raise KeyError('Unknown multi-termination strategy %s' % strategy)
-            return self.fg.get(term.external_ref)  # required to get full exchange list
+            return term  # targets() returns refs- no need to get again
 
     @staticmethod
     def construct_sparse(nums, nrows, ncols):
         """
 
         :param nums:
         :param nrows:
@@ -340,64 +358,14 @@
             try:
                 return csr_matrix((nums[:, 2], (nums[:, 0], nums[:, 1])), shape=(nrows, ncols))
             except IndexError:
                 print('nrows: %s  ncols: %s' % (nrows, ncols))
                 print(nums)
                 raise
 
-    '''
-    def compute_lci(self, product_flow, **kwargs):
-        if self.is_in_background(product_flow):
-            num_ad = np.array([[self.tstack.bg_dict(product_flow.index), 0, 1.0]])
-            ad = self.construct_sparse(num_ad, self.tstack.ndim, 1)
-            x, bx = self.compute_bg_lci(ad, **kwargs)
-            return bx
-        else:
-            af, ad, bf = self.make_foreground(product_flow)
-            x_tilde = np.linalg.inv(np.eye(af.shape[0]) - af.todense())[:, 0]
-            ad_tilde = ad * x_tilde
-            x, bx = self.compute_bg_lci(ad_tilde, **kwargs)
-            bf_tilde = csc_matrix(bf * x_tilde)
-            if bx is None:
-                return bf_tilde
-            return bx + bf_tilde
-
-    def compute_bg_lci(self, ad, threshold=1e-8, count=100):
-        """
-        Computes background LCI via iterative matrix multiplication.
-        :param ad: a vector of background activity levels
-        :param threshold: [1e-8] size of the increment (1-norm) relative to the total LCI to finish early
-        :param count: [100] maximum number of iterations to perform
-        :return:
-        """
-        x = csr_matrix(ad)  # tested this with ecoinvent: convert to sparse: 280 ms; keep full: 4.5 sec
-        total = self.construct_sparse([], *x.shape)
-        if self._a_matrix is None:
-            return total, None
-
-        mycount = 0
-        sumtotal = 0.0
-
-        while mycount < count:
-            total += x
-            x = self._a_matrix.dot(x)
-            inc = sum(abs(x).data)
-            if inc == 0:
-                print('exact result')
-                break
-            sumtotal += inc
-            if inc / sumtotal < threshold:
-                break
-            mycount += 1
-        print('completed %d iterations' % mycount)
-
-        b = self._b_matrix * total
-        return total, b
-    '''
-
     def _construct_b_matrix(self):
         """
         b matrix only includes emissions from background + downstream processes.
         [foreground processes LCI will have to be computed the foreground way]
         :return:
         """
         if self._b_matrix is not None:
@@ -414,15 +382,15 @@
 
     def _construct_a_matrix(self):
         ndim = self.tstack.ndim
         num_bg = np.array([[self.tstack.bg_dict(i.term.index), self.tstack.bg_dict(i.parent.index), i.value]
                            for i in self._interior])
         self._a_matrix = self.construct_sparse(num_bg, ndim, ndim)
 
-    '''Deprecated
+    '''required for create_flat_background
     '''
     def foreground_flows(self, search=None, outputs=True):
         for k in self.tstack.foreground_flows(outputs=outputs):
             if search is None:
                 yield k
             else:
                 if bool(re.search(search, str(k), flags=re.IGNORECASE)):
@@ -567,57 +535,29 @@
 
         for k in self.missing_references:
             print('Missing reference (term:%s;flow:%s)' % k)
         self.missing_references = []
 
         # self.make_foreground()
 
-    def add_all_ref_products(self, multi_term='abort', default_allocation=None, prefer=None):
+    def add_all_ref_products(self, multi_term='abort', default_allocation=None):
         """
 
         :param multi_term:
         :param default_allocation:
-        :param prefer: Specify preferred providers.  Because I am so sloppy, this routine has been written to accept
-        all kinds of possible formats for input:
-         dict: { flow_ref: process* } un-terminated flow-ref prefers named process
-           *- could be entity_type=process or external_ref of a process
-         list: [(flow_ref, process_ref), ...] .. un-terminated flow prefers named process
-           * same
-           ** for both of these, either flows or external_refs of flows can be passed as keys
-         list: [process, ...] .. list of processes to prefer if an ambiguous match is encountered (legacy)
-           * external_refs are converted into processes
         The list-of-2-tuples is tested in UsLciEcospoldTest; the legacy list-of-processes is tested in UsLciOlcaTest
         :return:
         """
         if self._all_added:
             return
-        if prefer is not None:
-            if isinstance(prefer, dict):
-                for k, v in prefer.items():
-                    if hasattr(k, 'external_ref'):
-                        k = k.external_ref
-                    self.preferred_processes[k] = v
-            elif isinstance(prefer, list):
-                try:
-                    for k, v in prefer:
-                        if hasattr(k, 'external_ref'):
-                            k = k.external_ref
-                        self.preferred_processes[k] = v
-                except TypeError:
-                    for p in prefer:
-                        if not hasattr(p, 'entity_type'):
-                            p = self.fg.get(p)
-                        self.preferred_processes[None].append(p)
-            else:
-                raise TypeError('Unable to interpret preferred process specification %s' % prefer)
-        for p in self.fg.processes():
+        for p in self.fg.processes(count=self.fg.count('process')):
             for x in p.references():
                 j = self.check_product_flow(x.flow, p)
                 if j is None:
-                    self._add_ref_product(x.flow, p, multi_term, default_allocation)
+                    self._add_ref_product_deque(x.flow, p, multi_term, default_allocation)
         self._update_component_graph()
         self._all_added = True
 
     def add_ref_product(self, flow, term, multi_term='abort', default_allocation=None):
         """
         Here we are adding a reference product - column of the A + B matrix.  The termination must be supplied.
         :param flow: a product flow
@@ -630,113 +570,264 @@
          'abort' - the default- do not allow a nondeterministic termination
         :param default_allocation: an LcQuantity to use for allocation if unallocated processes are encountered
         :return:
         """
         j = self.check_product_flow(flow, term)
 
         if j is None:
-            try:
-                j = self._add_ref_product(flow, term, multi_term, default_allocation)
-            except TerminationError:
-                print('add_ref_product failed.')
-                return
+            j = self._add_ref_product_deque(flow, term, multi_term, default_allocation)
 
             self._update_component_graph()
         return j
 
+    '''
     def _add_ref_product(self, flow, term, multi_term, default_allocation):
-        old_recursion_limit = sys.getrecursionlimit()
-        sys.setrecursionlimit(self.required_recursion_limit)
-
         j = self._create_product_flow(flow, term)
+        if j is None:
+            # _create_product_flow already prints a MissingReference message
+            return
         try:
             self._traverse_term_exchanges(j, multi_term, default_allocation)
         except TerminationError:
             self._rm_product_flow_children(j)
             print('Termination Error: process %s: ref_flow %s, ' % (j.process.external_ref, j.flow.external_ref))
 
             raise
 
-        sys.setrecursionlimit(old_recursion_limit)
         return j
 
     def _traverse_term_exchanges(self, parent, multi_term, default_allocation):
         """
         Implements the Tarjan traversal
         :param parent: a ProductFlow
         :param default_allocation:
         :return:
         """
         rx = parent.process.reference(parent.flow)
 
+        """ # this could never happen
         if not rx.is_reference:
             print('### Nonreference RX found!\nterm: %s\nflow: %s\next_id: %s' % (rx.process,
                                                                                   rx.flow,
                                                                                   rx.process.external_ref))
             rx = parent.process.reference()
             print('    using ref %s\n' % rx)
+        """
 
         exchs = parent.process.inventory(ref_flow=rx)  # allocated exchanges
 
         for exch in exchs:
             if exch.is_reference:  # in parent.process.reference_entity:
                 # we're done with the exchange
                 raise TypeError('Reference exchange encountered in bg inventory %s' % exch)
             val = pval = exch.value  # allocated exchange
+
+            # for interior flows-- enforce normative direction
+            if exch.direction == 'Output':
+                pval *= -1
+
             if val is None or val == 0:
                 # don't add zero entries (or descendants) to sparse matrix
                 continue
-            if exch.flow == rx.flow and exch.direction == comp_dir(rx.direction) and val == 1.0 and exch.type == 'cutoff':
+            if exch.flow == rx.flow and exch.direction == comp_dir(rx.direction) and\
+                    val == 1.0 and exch.type == 'cutoff':
                 # skip pass-thru flows
                 print('Skipping pass-thru exchange: %s' % exch)
                 continue
 
-            # interior flow-- enforce normative direction
-            if exch.direction == 'Output':
-                pval *= -1
             # normal non-reference exchange. Either a dependency (if interior) or a cutoff (if exterior).
             term = self.terminate(exch, multi_term)
             if term is None:
                 # cutoff -- add the exchange value to the exterior matrix
-                emission = self._add_emission(exch.flow, exch.direction, exch.termination)  # check, create, and add all at once
+                emission = self._add_emission(exch.flow, exch.direction, exch.termination)  # check, create, and add
                 self.add_cutoff(parent, emission, val)
                 continue
 
             # so it's interior-- does it exist already?
             i = self.check_product_flow(exch.flow, term)
             if i is None:
-                # not visited -- need to visit
-                i = self._create_product_flow(exch.flow, term)
+                i = self._add_ref_product(exch.flow, term, multi_term, default_allocation)
+
                 if i is None:
                     print('Cutting off at Parent process: %s\n%s -X- %s\n' % (parent.process.external_ref,
                                                                               exch.flow.name,
                                                                               term))
                     continue
-                if i.debug:
-                    print('Parent: %s' % parent.process)
-                try:
-                    self._traverse_term_exchanges(i, multi_term, default_allocation)
-                except TerminationError:
-                    self._rm_product_flow_children(i)
-                    raise
-
                 # carry back lowlink, if lower
                 self._set_lowlink(parent, self._lowlink(i))
             elif self.tstack.check_stack(i):
                 # visited and currently on stack - carry back index if lower
                 self._set_lowlink(parent, self.index(i))
             else:
                 # visited, not on stack- nothing to do
                 pass
             # add the exchange value to the interior matrix
             self.add_interior(parent, i, pval)
 
         # name an SCC if we've found one
         if self._lowlink(parent) == self.index(parent):
             self.tstack.label_scc(self.index(parent), parent.key)
+    '''
+
+    def _add_ref_product_deque(self, flow, term, multi_term, default_allocation):
+        if len(self._r_stack) != 0:
+            raise DequeError('Recursion stack is not empty')
+        j = self._create_product_flow(flow, term)
+        if j is None:
+            # _create_product_flow already prints a MissingReference message
+            return
+
+        self._dq_put_node_on_stack(j)
+
+        while len(self._r_stack) > 0:
+            try:
+                self._dq_handle_stack(multi_term, default_allocation)
+            except TerminationError:
+                self._rm_product_flow_children(j)
+                print('Termination Error: process %s: ref_flow %s, ' % (j.process.external_ref, j.flow.external_ref))
+
+                raise
+
+        return j
+
+    def _dq_put_node_on_stack(self, parent):
+        """
+        The theory here is that we use both ends of the stack to keep track of what we are doing.
+        The left-hand end is the recursion stack- we push things onto it as we traverse the graph
+        the right-hand end is the parent stack- we use it to keep track of the parent nodes we have
+        processed.  I suspect this will be equal to tstack._stack but I don't feel like investigating.
+
+        When we push a new node onto the stack- we put the node on the right, and a marker object on the left.
+        then we stack the exchanges on top of the marker object.
+        When we have cleared the stack back to the marker object, we know we're done with the node.
+
+        :param parent:
+        :return:
+        """
+        self._r_stack.appendleft(ParentMarker())
+        self._r_stack.append(parent)
+
+        rx = parent.process.reference(parent.flow)
+        exchs = parent.process.inventory(ref_flow=rx)  # allocated exchanges
+
+        self._r_stack.extendleft(list(exchs))
+
+    def _dq_handle_stack(self, multi_term, default_allocation):
+        obj = self._r_stack[0]
+        parent = self._r_stack[-1]
+
+        if isinstance(obj, ParentMarker):
+            """
+            # we have exhausted a parent node's exchanges and arrived back at the node-- we check to see if we've
+            discovered an SCC
+            """
+            # we have completed this parent node
+            self._r_stack.popleft()  # the recursion marker
+            parent = self._r_stack.pop()  # the parent node
+            # name an SCC if we've found one
+            if self._lowlink(parent) == self.index(parent):
+                self.tstack.label_scc(self.index(parent), parent.key)
+            # and we're done
+            return
+
+        elif isinstance(obj, RecurseMarker):
+            """
+            # we have completed recursion-- 
+            The exchange that triggered recursion is next on the stack and we need to handle the parent's lowlink
+            """
+            # carry back lowlink, if lower
+            marker = self._r_stack.popleft()
+            i = marker.term
+            self._set_lowlink(parent, self._lowlink(i))
+
+            ''' # add interior
+            '''
+            exch = self._r_stack.popleft()
+
+            pval = exch.value  # allocated exchange
+
+            # for interior flows-- enforce normative direction
+            if exch.direction == 'Output':
+                pval *= -1
+
+            self.add_interior(parent, i, pval)
+            # and we're done
+            return
+
+        else:
+            """
+            # obj is an exchange
+            We are in the middle of recursion, progressing through a child node's exchanges.  We proceed depending
+            on each exchange's characteristics -- 
+             - exterior--- is a recursive base case
+             - interior, novel--- we must recurse
+             - interior, on tarjan stack--- no recursion necessary but we have to update lowlink
+             - interior, not on tarjan stack--- nothing to do
+            """
+            exch = self._r_stack[0]
+
+            if exch.is_reference:  # in parent.process.reference_entity:
+                raise TypeError('Reference exchange encountered in bg inventory %s' % exch)
+
+            val = exch.value  # allocated exchange value
+
+            if val is None or val == 0:
+                # don't add zero entries (or descendants) to sparse matrix
+                self._r_stack.popleft()
+                return
+
+            if exch.flow == parent.flow and exch.direction == comp_dir(parent.direction) and\
+                    val == 1.0 and exch.type == 'cutoff':
+                # skip pass-thru flows
+                print('Skipping pass-thru exchange: %s' % exch)
+                self._r_stack.popleft()
+                return
+
+            # normal non-reference exchange. Either a dependency (if interior) or a cutoff (if exterior).
+            term = self.terminate(exch, multi_term)
+
+            if term is None:
+                # cutoff -- add the exchange value to the exterior matrix
+                exch = self._r_stack.popleft()  # finished with this exchange
+                emission = self._add_emission(exch.flow, exch.direction, exch.termination)  # check, create, and add
+                self.add_cutoff(parent, emission, val)
+
+            else:
+                # interior exchange
+                if exch.direction == 'Output':
+                    val *= -1
+
+                i = self.check_product_flow(exch.flow, term)
+
+                if i is None:
+                    # no product flow exists
+                    i = self._create_product_flow(exch.flow, term)
+                    if i is None:
+                        # MissingReference cutoff
+                        print('Cutting off at Parent process: %s\n%s -X- %s\n' % (parent.process.external_ref,
+                                                                                  exch.flow.name,
+                                                                                  term))
+                        return
+
+                    # we leave the exchange on the stack, and recurse into the target node
+                    self._r_stack.appendleft(RecurseMarker(i))
+                    self._dq_put_node_on_stack(i)
+                    return
+
+                elif self.tstack.check_stack(i):
+                    # visited and currently on stack - carry back index if lower
+                    self._set_lowlink(parent, self.index(i))
+
+                else:
+                    # visited, not on stack- nothing to do with lowlink
+                    pass
+
+                self._r_stack.popleft()
+
+                self.add_interior(parent, i, val)
 
     def add_cutoff(self, parent, emission, val):
         """
         Create an exchange for a cutoff flow (incl. elementary flows)
         :param parent: product flow- B matrix column
         :param emission: emission - B matrix row
         :param val: raw exchange value
```

### Comparing `antelope_background-0.2.4/antelope_background/engine/emission.py` & `antelope_background-0.2.4.1/antelope_background/engine/emission.py`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.4/antelope_background/engine/product_flow.py` & `antelope_background-0.2.4.1/antelope_background/engine/product_flow.py`

 * *Files identical despite different names*

### Comparing `antelope_background-0.2.4/antelope_background/engine/tarjan_stack.py` & `antelope_background-0.2.4.1/antelope_background/engine/tarjan_stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 
 
 class TarjanStack(object):
     """
     Stores the current stack and provides a record of named SCCs
     """
     def __init__(self):
-        self._stack = []
-        self._stack_hash = set()
+        self._stack = []  # product flows being reviewed
+        self._stack_hash = set()  # a (premature?) optimization to avoid costly list-membership testing
+
         self._sccs = defaultdict(set)  # dict mapping lowest index (lowlink = SCC ID) to the set of scc peers
         self._scc_of = dict()  # dict mapping product flow to SCC ID (reverse mapping of _sccs)
 
         self._component_cols_by_row = defaultdict(set)  # nonzero columns in given row (upstream dependents)
         self._component_rows_by_col = defaultdict(set)  # nonzero rows in given column (downstream dependencies)
 
         self._background = None  # single scc_id representing largest scc
```

### Comparing `antelope_background-0.2.4/antelope_background/providers/check_terms.py` & `antelope_background-0.2.4.1/antelope_background/providers/check_terms.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     :param prefer: a dict that maps flow external_refs to preferred providers
     """
     if prefer is None:
         prefer = dict()
 
     # first, validate preferred-providers
     for k, v in prefer.items():
-        if v is None:
+        if v is None or v == []:
             continue
         try:
             query.get(v).reference(k)
         except NoReference:
             raise ValueError('Bad preferred provider %s for flow %s' % (v, k))
 
     ct = CheckTerms(query)
```

### Comparing `antelope_background-0.2.4/antelope_background.egg-info/PKG-INFO` & `antelope_background-0.2.4.1/antelope_background.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: antelope_background
-Version: 0.2.4
+Version: 0.2.4.1
 Home-page: https://github.com/AntelopeLCA/background
 Author: Brandon Kuczenski
 Author-email: bkuczenski@ucsb.edu
 License: BSD 3-clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: antelope_core>=0.2.4
+Requires-Dist: antelope_core>=0.2.4.1
 Requires-Dist: scipy>=1.5
 Requires-Dist: numpy>=1.19
 
 # background
 Background LCI implementation including Tarjan Ordering.
 
 This is kept as a separate repo because it is the only place `numpy/scipy` is required.  The
```

### Comparing `antelope_background-0.2.4/antelope_background.egg-info/SOURCES.txt` & `antelope_background-0.2.4.1/antelope_background.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 antelope_background/__init__.py
+antelope_background/lci_tester.py
 antelope_background.egg-info/PKG-INFO
 antelope_background.egg-info/SOURCES.txt
 antelope_background.egg-info/dependency_links.txt
 antelope_background.egg-info/requires.txt
 antelope_background.egg-info/top_level.txt
 antelope_background/background/__init__.py
 antelope_background/background/flat_background.py
```

### Comparing `antelope_background-0.2.4/setup.py` & `antelope_background-0.2.4.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from setuptools import setup, find_packages
 
 requires = [
-    "antelope_core>=0.2.4",
+    "antelope_core>=0.2.4.1",
     "scipy>=1.5",
     "numpy>=1.19"
 ]
 
 """
 Change Log
+0.2.4.1 2024-04-24 - refactor recursion out of Tarjan algorithm; write LciTester
+                     depends on antelope_core 0.2.4.1 for search pagination
+
 0.2.4 - 2024-04-17 - Remove antelope.ExteriorFlow in favor of antelope.models.ExteriorFlow
 
 0.2.3 - 2024-03-21 - Correct dependencies
 
 0.2.2 - 2024-03-12 - termination test; changed some exceptions
 
 0.2.1 - 2023-04-10 - xdb passes benchmarks.
@@ -30,15 +33,15 @@
 0.1.5 - 2021-02-05 - bump version to keep pace with antelope_core 
 0.1.4 - 2021-01-29 - bugfixes to get CI passing.  match consistent versions with other packages.
 
 0.1.0 - 2021-01-06 - first published release
 """
 
 
-VERSION = '0.2.4'
+VERSION = '0.2.4.1'
 
 setup(
     name="antelope_background",
     version=VERSION,
     author="Brandon Kuczenski",
     author_email="bkuczenski@ucsb.edu",
     license="BSD 3-clause",
```

