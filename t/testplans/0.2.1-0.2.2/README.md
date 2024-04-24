# Comparing `tmp/testplans-0.2.1.tar.gz` & `tmp/testplans-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testplans-0.2.1.tar", last modified: Mon Apr 22 15:12:17 2024, max compression
+gzip compressed data, was "testplans-0.2.2.tar", last modified: Wed Apr 24 09:56:02 2024, max compression
```

## Comparing `testplans-0.2.1.tar` & `testplans-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 15:12:17.298848 testplans-0.2.1/
--rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 testplans-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     5494 2024-04-22 15:12:17.298848 testplans-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4584 2024-04-22 15:10:50.000000 testplans-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-22 15:12:17.299904 testplans-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 testplans-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 15:12:17.291127 testplans-0.2.1/testplans/
--rw-rw-rw-   0        0        0      105 2024-02-01 12:13:36.000000 testplans-0.2.1/testplans/__init__.py
--rw-rw-rw-   0        0        0      776 2024-03-15 14:57:12.000000 testplans-0.2.1/testplans/_results.py
--rw-rw-rw-   0        0        0     3845 2024-04-22 15:01:51.000000 testplans-0.2.1/testplans/api.py
--rw-rw-rw-   0        0        0     7686 2024-04-22 13:45:33.000000 testplans-0.2.1/testplans/devices.py
--rw-rw-rw-   0        0        0     6347 2024-04-22 14:33:47.000000 testplans-0.2.1/testplans/gui.py
--rw-rw-rw-   0        0        0    10511 2024-04-22 15:01:51.000000 testplans-0.2.1/testplans/main.py
--rw-rw-rw-   0        0        0     1561 2024-04-22 14:50:31.000000 testplans-0.2.1/testplans/models.py
--rw-rw-rw-   0        0        0    11041 2024-04-22 13:46:38.000000 testplans-0.2.1/testplans/tc.py
--rw-rw-rw-   0        0        0     8911 2024-03-29 14:14:49.000000 testplans-0.2.1/testplans/tm.py
-drwxrwxrwx   0        0        0        0 2024-04-22 15:12:17.297603 testplans-0.2.1/testplans.egg-info/
--rw-rw-rw-   0        0        0     5494 2024-04-22 15:12:17.000000 testplans-0.2.1/testplans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-04-22 15:12:17.000000 testplans-0.2.1/testplans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 15:12:17.000000 testplans-0.2.1/testplans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-22 15:12:17.000000 testplans-0.2.1/testplans.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 09:56:02.925351 testplans-0.2.2/
+-rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 testplans-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     5494 2024-04-24 09:56:02.925210 testplans-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4584 2024-04-22 15:10:50.000000 testplans-0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 09:56:02.925702 testplans-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 testplans-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:56:02.917649 testplans-0.2.2/testplans/
+-rw-rw-rw-   0        0        0      105 2024-02-01 12:13:36.000000 testplans-0.2.2/testplans/__init__.py
+-rw-rw-rw-   0        0        0      776 2024-03-15 14:57:12.000000 testplans-0.2.2/testplans/_results.py
+-rw-rw-rw-   0        0        0     3845 2024-04-22 15:01:51.000000 testplans-0.2.2/testplans/api.py
+-rw-rw-rw-   0        0        0     7686 2024-04-22 13:45:33.000000 testplans-0.2.2/testplans/devices.py
+-rw-rw-rw-   0        0        0     6347 2024-04-22 14:33:47.000000 testplans-0.2.2/testplans/gui.py
+-rw-rw-rw-   0        0        0    10511 2024-04-22 15:01:51.000000 testplans-0.2.2/testplans/main.py
+-rw-rw-rw-   0        0        0     1561 2024-04-22 14:50:31.000000 testplans-0.2.2/testplans/models.py
+-rw-rw-rw-   0        0        0    10986 2024-04-24 09:53:50.000000 testplans-0.2.2/testplans/tc.py
+-rw-rw-rw-   0        0        0     8911 2024-03-29 14:14:49.000000 testplans-0.2.2/testplans/tm.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:56:02.923679 testplans-0.2.2/testplans.egg-info/
+-rw-rw-rw-   0        0        0     5494 2024-04-24 09:56:02.000000 testplans-0.2.2/testplans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-04-24 09:56:02.000000 testplans-0.2.2/testplans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 09:56:02.000000 testplans-0.2.2/testplans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-24 09:56:02.000000 testplans-0.2.2/testplans.egg-info/top_level.txt
```

### Comparing `testplans-0.2.1/LICENSE` & `testplans-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `testplans-0.2.1/PKG-INFO` & `testplans-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testplans
-Version: 0.2.1
+Version: 0.2.2
 Summary: simple testplan framework for several DUTs
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/testplans
 Keywords: testplan,testplan structure framework,testplan gui,testplan multy dut,testplan several dut
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `testplans-0.2.1/README.md` & `testplans-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `testplans-0.2.1/setup.py` & `testplans-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.1/testplans/_results.py` & `testplans-0.2.2/testplans/_results.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.1/testplans/api.py` & `testplans-0.2.2/testplans/api.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.1/testplans/devices.py` & `testplans-0.2.2/testplans/devices.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.1/testplans/gui.py` & `testplans-0.2.2/testplans/gui.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.1/testplans/main.py` & `testplans-0.2.2/testplans/main.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.1/testplans/models.py` & `testplans-0.2.2/testplans/models.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.1/testplans/tc.py` & `testplans-0.2.2/testplans/tc.py`

 * *Files 10% similar despite different names*

```diff
@@ -158,37 +158,37 @@
 
     # DETAILS ---------------------------------------------------------------------------------------------------------
     def details_update(self, details: Dict[str, Any]) -> None:
         self.details.update(details)
         # self.signals.signal__tc_state_changed.emit(self)
 
     # =================================================================================================================
-    # def info_pretty(self) -> str:
-    #     # fixme: ref from info_get
-    #     result = ""
-    #
-    #     result += f"NAME={self.NAME}\n"
-    #     result += f"DESCRIPTION={self.DESCRIPTION}\n"
-    #     result += f"SKIP={self.SKIP}\n"
-    #     result += f"skip_tc_dut={self.skip_tc_dut}\n"
-    #     result += f"ASYNC={self.ASYNC}\n"
-    #     result += f"INDEX={self.INDEX}\n"
-    #     result += f"result={self.result}\n"
-    #     result += f"progress={self.progress}\n"
-    #     result += f"exx={self.exx}\n"
-    #
-    #     result += f"SETTINGS=====================\n"
-    #     if self.SETTINGS:
-    #         for name, value in self.SETTINGS.dict.items():
-    #             result += f"{name}: {value}\n"
-    #
-    #     result += f"details=====================\n"
-    #     for name, value in self.details.items():
-    #         result += f"{name}: {value}\n"
-    #     return result
+    def info_pretty(self) -> str:
+        # fixme: ref from info_get
+        result = ""
+
+        result += f"NAME={self.NAME}\n"
+        result += f"DESCRIPTION={self.DESCRIPTION}\n"
+        result += f"SKIP={self.SKIP}\n"
+        result += f"skip_tc_dut={self.skip_tc_dut}\n"
+        result += f"ASYNC={self.ASYNC}\n"
+        result += f"INDEX={self.INDEX}\n"
+        result += f"result={self.result}\n"
+        result += f"progress={self.progress}\n"
+        result += f"exx={self.exx}\n"
+
+        result += f"SETTINGS=====================\n"
+        if self.SETTINGS:
+            for name, value in self.SETTINGS.dict.items():
+                result += f"{name}: {value}\n"
+
+        result += f"details=====================\n"
+        for name, value in self.details.items():
+            result += f"{name}: {value}\n"
+        return result
 
     @classmethod
     def get__info(cls) -> ModelTcClsInfo:
         """
         get info/structure about TcCls
         """
         result = {
```

### Comparing `testplans-0.2.1/testplans/tm.py` & `testplans-0.2.2/testplans/tm.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.1/testplans.egg-info/PKG-INFO` & `testplans-0.2.2/testplans.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testplans
-Version: 0.2.1
+Version: 0.2.2
 Summary: simple testplan framework for several DUTs
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/testplans
 Keywords: testplan,testplan structure framework,testplan gui,testplan multy dut,testplan several dut
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

