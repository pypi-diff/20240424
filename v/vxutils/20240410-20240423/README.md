# Comparing `tmp/vxutils-20240410.tar.gz` & `tmp/vxutils-20240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vxutils-20240410.tar", max compression
+gzip compressed data, was "vxutils-20240423.tar", max compression
```

## Comparing `vxutils-20240410.tar` & `vxutils-20240423.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1998 2024-04-10 02:47:02.408906 vxutils-20240410/pyproject.toml
--rw-r--r--   0        0        0       24 2024-02-28 02:40:58.487414 vxutils-20240410/README.md
--rw-r--r--   0        0        0      421 2024-04-02 02:11:16.355963 vxutils-20240410/src/vxsched/__init__.py
--rw-r--r--   0        0        0     1370 2024-03-31 05:45:50.712223 vxutils-20240410/src/vxsched/__main__.py
--rw-r--r--   0        0        0     7776 2024-03-15 02:21:02.576581 vxutils-20240410/src/vxsched/core.py
--rw-r--r--   0        0        0    11734 2024-03-07 05:59:56.919198 vxutils-20240410/src/vxsched/event.py
--rw-r--r--   0        0        0        0 2024-03-07 06:18:59.347092 vxutils-20240410/src/vxsched/py.typed
--rw-r--r--   0        0        0     1202 2024-04-02 02:11:10.194079 vxutils-20240410/src/vxsched/subpubs.py
--rw-r--r--   0        0        0     1375 2024-04-03 04:23:00.014767 vxutils-20240410/src/vxutils/__init__.py
--rw-r--r--   0        0        0     3738 2024-03-31 05:45:39.670502 vxutils-20240410/src/vxutils/context.py
--rw-r--r--   0        0        0     9225 2024-02-20 02:25:26.235753 vxutils-20240410/src/vxutils/convertors.py
--rw-r--r--   0        0        0        0 2024-02-17 13:24:20.316286 vxutils-20240410/src/vxutils/datamodel/__init__.py
--rw-r--r--   0        0        0     4214 2024-02-18 02:09:20.092983 vxutils-20240410/src/vxutils/datamodel/adapter.py
--rw-r--r--   0        0        0     2369 2024-03-07 04:24:54.189680 vxutils-20240410/src/vxutils/datamodel/core.py
--rw-r--r--   0        0        0    15247 2024-03-12 05:04:59.968100 vxutils-20240410/src/vxutils/datamodel/dborm.py
--rw-r--r--   0        0        0     9071 2024-04-07 01:14:57.773870 vxutils-20240410/src/vxutils/decorators.py
--rw-r--r--   0        0        0     9568 2024-04-07 01:16:17.431751 vxutils-20240410/src/vxutils/dtutils.py
--rw-r--r--   0        0        0     7430 2024-04-10 02:46:27.989670 vxutils-20240410/src/vxutils/logger.py
--rw-r--r--   0        0        0    14529 2024-02-20 08:56:31.979240 vxutils-20240410/src/vxutils/networking/requests.py
--rw-r--r--   0        0        0     7987 2024-03-31 01:34:06.580192 vxutils-20240410/src/vxutils/networking/wechat.py
--rw-r--r--   0        0        0     6173 2024-03-15 02:47:00.420052 vxutils-20240410/src/vxutils/provider.py
--rw-r--r--   0        0        0        0 2024-02-15 15:46:34.000000 vxutils-20240410/src/vxutils/py.typed
--rw-r--r--   0        0        0      446 2024-03-10 03:13:04.515372 vxutils-20240410/src/vxutils/typehints.py
--rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 vxutils-20240410/PKG-INFO
+-rw-r--r--   0        0        0     1998 2024-04-23 09:59:59.121961 vxutils-20240423/pyproject.toml
+-rw-r--r--   0        0        0       24 2024-02-28 02:40:58.487414 vxutils-20240423/README.md
+-rw-r--r--   0        0        0      421 2024-04-02 02:11:16.355963 vxutils-20240423/src/vxsched/__init__.py
+-rw-r--r--   0        0        0     1374 2024-04-14 08:23:52.813822 vxutils-20240423/src/vxsched/__main__.py
+-rw-r--r--   0        0        0     7776 2024-03-15 02:21:02.576581 vxutils-20240423/src/vxsched/core.py
+-rw-r--r--   0        0        0    11734 2024-03-07 05:59:56.919198 vxutils-20240423/src/vxsched/event.py
+-rw-r--r--   0        0        0        0 2024-03-07 06:18:59.347092 vxutils-20240423/src/vxsched/py.typed
+-rw-r--r--   0        0        0     1202 2024-04-02 02:11:10.194079 vxutils-20240423/src/vxsched/subpubs.py
+-rw-r--r--   0        0        0     1375 2024-04-03 04:23:00.014767 vxutils-20240423/src/vxutils/__init__.py
+-rw-r--r--   0        0        0     3738 2024-03-31 05:45:39.670502 vxutils-20240423/src/vxutils/context.py
+-rw-r--r--   0        0        0     9225 2024-02-20 02:25:26.235753 vxutils-20240423/src/vxutils/convertors.py
+-rw-r--r--   0        0        0        0 2024-02-17 13:24:20.316286 vxutils-20240423/src/vxutils/datamodel/__init__.py
+-rw-r--r--   0        0        0     4436 2024-04-23 09:59:47.736934 vxutils-20240423/src/vxutils/datamodel/adapter.py
+-rw-r--r--   0        0        0     2369 2024-03-07 04:24:54.189680 vxutils-20240423/src/vxutils/datamodel/core.py
+-rw-r--r--   0        0        0    15247 2024-03-12 05:04:59.968100 vxutils-20240423/src/vxutils/datamodel/dborm.py
+-rw-r--r--   0        0        0     9071 2024-04-07 01:14:57.773870 vxutils-20240423/src/vxutils/decorators.py
+-rw-r--r--   0        0        0     9568 2024-04-07 01:16:17.431751 vxutils-20240423/src/vxutils/dtutils.py
+-rw-r--r--   0        0        0     7430 2024-04-10 02:46:27.989670 vxutils-20240423/src/vxutils/logger.py
+-rw-r--r--   0        0        0    14529 2024-02-20 08:56:31.979240 vxutils-20240423/src/vxutils/networking/requests.py
+-rw-r--r--   0        0        0     7987 2024-03-31 01:34:06.580192 vxutils-20240423/src/vxutils/networking/wechat.py
+-rw-r--r--   0        0        0     6173 2024-03-15 02:47:00.420052 vxutils-20240423/src/vxutils/provider.py
+-rw-r--r--   0        0        0        0 2024-02-15 15:46:34.000000 vxutils-20240423/src/vxutils/py.typed
+-rw-r--r--   0        0        0      446 2024-03-10 03:13:04.515372 vxutils-20240423/src/vxutils/typehints.py
+-rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 vxutils-20240423/PKG-INFO
```

### Comparing `vxutils-20240410/pyproject.toml` & `vxutils-20240423/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vxutils"
-version = "20240410"
+version = "20240423"
 description = "python 常用工具箱"
 license = "MIT"
 authors = ["vex1023 <vex1023@qq.com>"]
 homepage = "https://gitee.com/vxquant/vxutils"
 keywords = ["quant", "tools"]
 readme = "README.md"
```

### Comparing `vxutils-20240410/src/vxsched/__main__.py` & `vxutils-20240423/src/vxsched/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 def main() -> None:
     parser = ArgumentParser(description="调度器")
     parser.add_argument("-c", "--config", default="etc/config.json", help="配置文件")
     parser.add_argument("-m", "--mod", default="mod", help="事件列表")
     parser.add_argument("-l", "--log", default="", help="日志目录")
     parser.add_argument(
-        "-d", "--debug", default=False, help="调试模式", action="store_true"
+        "-v", "--verbose", default=False, help="调试模式", action="store_true"
     )
     args = parser.parse_args()
-    level = "DEBUG" if args.debug else "INFO"
+    level = "DEBUG" if args.verbose else "INFO"
     if args.log:
         loggerConfig(level=level, filename=args.log)
         logging.debug("启用日志文件: %s", args.log)
     else:
         loggerConfig(level=level, colored=True)
 
     configfile = Path(args.config)
```

### Comparing `vxutils-20240410/src/vxsched/core.py` & `vxutils-20240423/src/vxsched/core.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240410/src/vxsched/event.py` & `vxutils-20240423/src/vxsched/event.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240410/src/vxsched/subpubs.py` & `vxutils-20240423/src/vxsched/subpubs.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240410/src/vxutils/__init__.py` & `vxutils-20240423/src/vxutils/__init__.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240410/src/vxutils/context.py` & `vxutils-20240423/src/vxutils/context.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240410/src/vxutils/convertors.py` & `vxutils-20240423/src/vxutils/convertors.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240410/src/vxutils/datamodel/adapter.py` & `vxutils-20240423/src/vxutils/datamodel/adapter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """数据转换器"""
 
-from typing import Type, Dict, Callable, Any, Tuple, Optional, Union, NotRequired
-from collections.abc import Mapping
+from typing import Type, Dict, Callable, Any, Optional, Union
 from operator import getitem
+from pydantic import BaseModel
 
 # from vxutils import logger
 
 # from vxutils.database.fields import _NOTSET
-
 NOSET = object()
 
 
 class DataAdapterError(Exception):
     """数据转换器异常"""
 
     pass
@@ -84,15 +83,15 @@
         "target4": OriginCol("origin4",default="ok"),
         "target5": TransCol(lambda x: x["origin5"]+1),
     }
     """
 
     def __init__(
         self,
-        target_cls: Type[Mapping[str, Any]],
+        target_cls: Union[Type[BaseModel], Type[Dict[str, Any]]],
         coladapters: Dict[str, Union[str, Callable[[Any], Any]]],
     ) -> None:
         self._target_cls = target_cls
         self._coladapters: Dict[str, Callable[[Any], Any]] = {}
         for target_col, coladapter in coladapters.items():
             if isinstance(coladapter, VXColAdapter):
                 self._coladapters[target_col] = coladapter
@@ -109,18 +108,22 @@
             for target_col, coladapter in self._coladapters.items():
                 try:
                     data[target_col] = coladapter(other_data)
                 except DataAdapterError as e:
                     if not ignore_col_error:
                         raise e
             target_data = self._target_cls(**data)
-            if key:
-                return getitem(target_data, key), target_data
-
-            return target_data
+            if not key:
+                return target_data
+            elif isinstance(target_data, BaseModel):
+                return getattr(target_data, key), target_data
+            elif isinstance(target_data, dict):
+                return target_data.get(key, ""), target_data
+            else:
+                return key, target_data
         except Exception as e:
             raise DataAdapterError(e) from e
 
 
 if __name__ == "__main__":
     from vxutils import VXContext
```

### Comparing `vxutils-20240410/src/vxutils/datamodel/core.py` & `vxutils-20240423/src/vxutils/datamodel/core.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240410/src/vxutils/datamodel/dborm.py` & `vxutils-20240423/src/vxutils/datamodel/dborm.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240410/src/vxutils/decorators.py` & `vxutils-20240423/src/vxutils/decorators.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240410/src/vxutils/dtutils.py` & `vxutils-20240423/src/vxutils/dtutils.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240410/src/vxutils/logger.py` & `vxutils-20240423/src/vxutils/logger.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240410/src/vxutils/networking/requests.py` & `vxutils-20240423/src/vxutils/networking/requests.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240410/src/vxutils/networking/wechat.py` & `vxutils-20240423/src/vxutils/networking/wechat.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240410/src/vxutils/provider.py` & `vxutils-20240423/src/vxutils/provider.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240410/PKG-INFO` & `vxutils-20240423/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vxutils
-Version: 20240410
+Version: 20240423
 Summary: python 常用工具箱
 Home-page: https://gitee.com/vxquant/vxutils
 License: MIT
 Keywords: quant,tools
 Author: vex1023
 Author-email: vex1023@qq.com
 Requires-Python: >=3.8,<4.0
```

