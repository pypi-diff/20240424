# Comparing `tmp/fastapi_assistant-0.1.25.tar.gz` & `tmp/fastapi_assistant-0.1.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fastapi_assistant-0.1.25.tar", last modified: Mon Jan 15 08:48:31 2024, max compression
+gzip compressed data, was "dist/fastapi_assistant-0.1.27.tar", last modified: Wed Apr 24 14:58:55 2024, max compression
```

## Comparing `fastapi_assistant-0.1.25.tar` & `fastapi_assistant-0.1.27.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 lgh        (501) staff       (20)        0 2024-01-15 08:48:31.771957 fastapi_assistant-0.1.25/
--rw-r--r--   0 lgh        (501) staff       (20)       52 2023-08-18 02:48:13.000000 fastapi_assistant-0.1.25/MANIFEST.in
--rw-r--r--   0 lgh        (501) staff       (20)      631 2024-01-15 08:48:31.771677 fastapi_assistant-0.1.25/PKG-INFO
--rw-r--r--   0 lgh        (501) staff       (20)       74 2023-09-18 11:43:58.000000 fastapi_assistant-0.1.25/README.md
-drwxr-xr-x   0 lgh        (501) staff       (20)        0 2024-01-15 08:48:31.764412 fastapi_assistant-0.1.25/fastapi_assistant/
--rw-r--r--   0 lgh        (501) staff       (20)       27 2023-09-18 11:43:58.000000 fastapi_assistant-0.1.25/fastapi_assistant/__init__.py
-drwxr-xr-x   0 lgh        (501) staff       (20)        0 2024-01-15 08:48:31.768283 fastapi_assistant-0.1.25/fastapi_assistant/bases/
--rw-r--r--   0 lgh        (501) staff       (20)      156 2023-09-18 11:43:58.000000 fastapi_assistant-0.1.25/fastapi_assistant/bases/__init__.py
--rw-r--r--   0 lgh        (501) staff       (20)     7367 2024-01-15 08:46:48.000000 fastapi_assistant-0.1.25/fastapi_assistant/bases/dao.py
--rw-r--r--   0 lgh        (501) staff       (20)     1589 2023-12-18 03:46:20.000000 fastapi_assistant-0.1.25/fastapi_assistant/bases/enums.py
--rw-r--r--   0 lgh        (501) staff       (20)     1340 2023-09-18 11:43:58.000000 fastapi_assistant-0.1.25/fastapi_assistant/bases/model.py
--rw-r--r--   0 lgh        (501) staff       (20)     2922 2023-12-18 03:36:45.000000 fastapi_assistant-0.1.25/fastapi_assistant/bases/schema.py
--rw-r--r--   0 lgh        (501) staff       (20)     5241 2023-11-03 12:11:37.000000 fastapi_assistant-0.1.25/fastapi_assistant/bases/service.py
--rw-r--r--   0 lgh        (501) staff       (20)     4131 2023-12-16 02:34:36.000000 fastapi_assistant-0.1.25/fastapi_assistant/builder_api.py
--rw-r--r--   0 lgh        (501) staff       (20)     2163 2023-10-23 02:38:14.000000 fastapi_assistant-0.1.25/fastapi_assistant/builder_db_engine.py
-drwxr-xr-x   0 lgh        (501) staff       (20)        0 2024-01-15 08:48:31.769700 fastapi_assistant-0.1.25/fastapi_assistant/core/
--rw-r--r--   0 lgh        (501) staff       (20)      141 2023-09-18 12:04:36.000000 fastapi_assistant-0.1.25/fastapi_assistant/core/__init__.py
--rw-r--r--   0 lgh        (501) staff       (20)      921 2023-11-03 12:11:37.000000 fastapi_assistant-0.1.25/fastapi_assistant/core/exceptions.py
--rw-r--r--   0 lgh        (501) staff       (20)      966 2023-09-18 10:23:39.000000 fastapi_assistant-0.1.25/fastapi_assistant/core/scheduler.py
--rw-r--r--   0 lgh        (501) staff       (20)     3188 2023-09-18 11:43:58.000000 fastapi_assistant-0.1.25/fastapi_assistant/core/sqlalchemy.py
-drwxr-xr-x   0 lgh        (501) staff       (20)        0 2024-01-15 08:48:31.771204 fastapi_assistant-0.1.25/fastapi_assistant/libs/
--rw-r--r--   0 lgh        (501) staff       (20)       77 2023-10-20 09:00:53.000000 fastapi_assistant-0.1.25/fastapi_assistant/libs/__init__.py
--rw-r--r--   0 lgh        (501) staff       (20)     5526 2023-12-07 10:18:44.000000 fastapi_assistant-0.1.25/fastapi_assistant/libs/date_time.py
--rw-r--r--   0 lgh        (501) staff       (20)     3490 2023-12-08 03:55:10.000000 fastapi_assistant-0.1.25/fastapi_assistant/libs/excel_tool.py
--rw-r--r--   0 lgh        (501) staff       (20)      244 2023-09-18 11:43:58.000000 fastapi_assistant-0.1.25/fastapi_assistant/libs/pagination.py
--rw-r--r--   0 lgh        (501) staff       (20)     1176 2023-09-18 11:43:58.000000 fastapi_assistant-0.1.25/fastapi_assistant/log_settings.py
-drwxr-xr-x   0 lgh        (501) staff       (20)        0 2024-01-15 08:48:31.766091 fastapi_assistant-0.1.25/fastapi_assistant.egg-info/
--rw-r--r--   0 lgh        (501) staff       (20)      631 2024-01-15 08:48:31.000000 fastapi_assistant-0.1.25/fastapi_assistant.egg-info/PKG-INFO
--rw-r--r--   0 lgh        (501) staff       (20)      862 2024-01-15 08:48:31.000000 fastapi_assistant-0.1.25/fastapi_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 lgh        (501) staff       (20)        1 2024-01-15 08:48:31.000000 fastapi_assistant-0.1.25/fastapi_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 lgh        (501) staff       (20)      225 2024-01-15 08:48:31.000000 fastapi_assistant-0.1.25/fastapi_assistant.egg-info/requires.txt
--rw-r--r--   0 lgh        (501) staff       (20)       18 2024-01-15 08:48:31.000000 fastapi_assistant-0.1.25/fastapi_assistant.egg-info/top_level.txt
--rw-r--r--   0 lgh        (501) staff       (20)       38 2024-01-15 08:48:31.772749 fastapi_assistant-0.1.25/setup.cfg
--rw-r--r--   0 lgh        (501) staff       (20)     1540 2024-01-15 08:46:48.000000 fastapi_assistant-0.1.25/setup.py
+drwxr-xr-x   0 lgh        (501) staff       (20)        0 2024-04-24 14:58:55.441353 fastapi_assistant-0.1.27/
+-rw-r--r--   0 lgh        (501) staff       (20)       52 2023-08-18 02:48:13.000000 fastapi_assistant-0.1.27/MANIFEST.in
+-rw-r--r--   0 lgh        (501) staff       (20)      631 2024-04-24 14:58:55.440884 fastapi_assistant-0.1.27/PKG-INFO
+-rw-r--r--   0 lgh        (501) staff       (20)       74 2023-09-18 11:43:58.000000 fastapi_assistant-0.1.27/README.md
+drwxr-xr-x   0 lgh        (501) staff       (20)        0 2024-04-24 14:58:55.432366 fastapi_assistant-0.1.27/fastapi_assistant/
+-rw-r--r--   0 lgh        (501) staff       (20)       27 2023-09-18 11:43:58.000000 fastapi_assistant-0.1.27/fastapi_assistant/__init__.py
+drwxr-xr-x   0 lgh        (501) staff       (20)        0 2024-04-24 14:58:55.437127 fastapi_assistant-0.1.27/fastapi_assistant/bases/
+-rw-r--r--   0 lgh        (501) staff       (20)      156 2023-09-18 11:43:58.000000 fastapi_assistant-0.1.27/fastapi_assistant/bases/__init__.py
+-rw-r--r--   0 lgh        (501) staff       (20)     7439 2024-04-24 10:36:10.000000 fastapi_assistant-0.1.27/fastapi_assistant/bases/dao.py
+-rw-r--r--   0 lgh        (501) staff       (20)     1589 2023-12-18 03:46:20.000000 fastapi_assistant-0.1.27/fastapi_assistant/bases/enums.py
+-rw-r--r--   0 lgh        (501) staff       (20)     1340 2023-09-18 11:43:58.000000 fastapi_assistant-0.1.27/fastapi_assistant/bases/model.py
+-rw-r--r--   0 lgh        (501) staff       (20)     2922 2023-12-18 03:36:45.000000 fastapi_assistant-0.1.27/fastapi_assistant/bases/schema.py
+-rw-r--r--   0 lgh        (501) staff       (20)     5241 2024-04-24 10:35:31.000000 fastapi_assistant-0.1.27/fastapi_assistant/bases/service.py
+-rw-r--r--   0 lgh        (501) staff       (20)     4131 2023-12-16 02:34:36.000000 fastapi_assistant-0.1.27/fastapi_assistant/builder_api.py
+-rw-r--r--   0 lgh        (501) staff       (20)     2163 2024-04-24 08:41:10.000000 fastapi_assistant-0.1.27/fastapi_assistant/builder_db_engine.py
+drwxr-xr-x   0 lgh        (501) staff       (20)        0 2024-04-24 14:58:55.438894 fastapi_assistant-0.1.27/fastapi_assistant/core/
+-rw-r--r--   0 lgh        (501) staff       (20)      141 2023-09-18 12:04:36.000000 fastapi_assistant-0.1.27/fastapi_assistant/core/__init__.py
+-rw-r--r--   0 lgh        (501) staff       (20)      921 2023-11-03 12:11:37.000000 fastapi_assistant-0.1.27/fastapi_assistant/core/exceptions.py
+-rw-r--r--   0 lgh        (501) staff       (20)      966 2023-09-18 10:23:39.000000 fastapi_assistant-0.1.27/fastapi_assistant/core/scheduler.py
+-rw-r--r--   0 lgh        (501) staff       (20)     3188 2023-09-18 11:43:58.000000 fastapi_assistant-0.1.27/fastapi_assistant/core/sqlalchemy.py
+drwxr-xr-x   0 lgh        (501) staff       (20)        0 2024-04-24 14:58:55.440544 fastapi_assistant-0.1.27/fastapi_assistant/libs/
+-rw-r--r--   0 lgh        (501) staff       (20)      108 2024-04-24 10:19:14.000000 fastapi_assistant-0.1.27/fastapi_assistant/libs/__init__.py
+-rw-r--r--   0 lgh        (501) staff       (20)     5526 2023-12-07 10:18:44.000000 fastapi_assistant-0.1.27/fastapi_assistant/libs/date_time.py
+-rw-r--r--   0 lgh        (501) staff       (20)     3670 2024-04-24 11:51:07.000000 fastapi_assistant-0.1.27/fastapi_assistant/libs/excel_tool.py
+-rw-r--r--   0 lgh        (501) staff       (20)      244 2023-09-18 11:43:58.000000 fastapi_assistant-0.1.27/fastapi_assistant/libs/pagination.py
+-rw-r--r--   0 lgh        (501) staff       (20)     3574 2024-04-24 14:43:10.000000 fastapi_assistant-0.1.27/fastapi_assistant/libs/template_import.py
+-rw-r--r--   0 lgh        (501) staff       (20)     1176 2023-09-18 11:43:58.000000 fastapi_assistant-0.1.27/fastapi_assistant/log_settings.py
+drwxr-xr-x   0 lgh        (501) staff       (20)        0 2024-04-24 14:58:55.434222 fastapi_assistant-0.1.27/fastapi_assistant.egg-info/
+-rw-r--r--   0 lgh        (501) staff       (20)      631 2024-04-24 14:58:55.000000 fastapi_assistant-0.1.27/fastapi_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 lgh        (501) staff       (20)      904 2024-04-24 14:58:55.000000 fastapi_assistant-0.1.27/fastapi_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 lgh        (501) staff       (20)        1 2024-04-24 14:58:55.000000 fastapi_assistant-0.1.27/fastapi_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 lgh        (501) staff       (20)      225 2024-04-24 14:58:55.000000 fastapi_assistant-0.1.27/fastapi_assistant.egg-info/requires.txt
+-rw-r--r--   0 lgh        (501) staff       (20)       18 2024-04-24 14:58:55.000000 fastapi_assistant-0.1.27/fastapi_assistant.egg-info/top_level.txt
+-rw-r--r--   0 lgh        (501) staff       (20)       38 2024-04-24 14:58:55.441473 fastapi_assistant-0.1.27/setup.cfg
+-rw-r--r--   0 lgh        (501) staff       (20)     1540 2024-04-24 14:58:42.000000 fastapi_assistant-0.1.27/setup.py
```

### Comparing `fastapi_assistant-0.1.25/PKG-INFO` & `fastapi_assistant-0.1.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_assistant
-Version: 0.1.25
+Version: 0.1.27
 Summary: fastapi脚手架，封装了基本curd、excel处理、异常、仿照django实现的get_or_one,create_or_update
 Home-page: https://gitee.com/ileona/fastapi-assistant.git
 Author: lxshen
 Author-email: lxshen613@163.com
 License: UNKNOWN
 Description: ### RestFastApi
             fast_api脚手架，封装了一些基本工具和curl
```

### Comparing `fastapi_assistant-0.1.25/fastapi_assistant/bases/dao.py` & `fastapi_assistant-0.1.27/fastapi_assistant/bases/dao.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-import math
 from typing import List, Optional, Tuple, Any, Dict
 
 from sqlalchemy import func
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.orm import Session
 
-from fastapi_assistant.bases.enums import FilterConditionEnum
 from fastapi_assistant.bases.model import EnhancedModel
 from fastapi_assistant.bases.schema import ListArgsSchema, ListFilterSchema, ListOrderSchema, ListCustomizeFilterSchema
 from fastapi_assistant.core.sqlalchemy import get_or_create, update_or_create
 
 
 class BasicDao(object):
     Model = EnhancedModel
@@ -32,26 +30,28 @@
         :param is_commit:
         :return:
         """
         try:
             db.add(obj)
             db.flush()
         except Exception as e:
-            db.rollback()
+            if is_commit:
+                db.rollback()
             raise e
         if is_commit:
             db.commit()
 
     async def dict_create(self, db: Session, object_dict: Dict[str, Any], is_commit: bool = True) -> Model:
         model = self.Model(**object_dict)
         try:
             db.add(model)
             db.flush()
         except Exception as e:
-            db.rollback()
+            if is_commit:
+                db.rollback()
             raise e
         if is_commit:
             db.commit()
         return model
 
     async def get_or_create(self, db: Session, defaults=None, is_commit: bool = True, **kwargs) -> Tuple[Model, bool]:
         """
@@ -107,15 +107,16 @@
         """
         filters = self.base_filters()
         filters.append(self.Model.id == pk)
         try:
             db.query(self.Model).filter(*filters).update(update_data, synchronize_session=False)
             db.flush()
         except Exception as e:
-            db.rollback()
+            if is_commit:
+                db.rollback()
             raise e
         if is_commit:
             db.commit()
 
     async def delete(self, db: Session, pk: int, is_commit: bool = True):
         """
         删除一条数据，定义了 is_deleted 进行软删除，否者真删除
@@ -128,14 +129,16 @@
             if filters:
                 filters.append(self.Model.id == pk)
                 db.query(self.Model).filter(*filters).update({self.Model.is_deleted: True}, synchronize_session=False)
             else:
                 db.query(self.Model).filter(self.Model.id == pk).delete()
             db.flush()
         except Exception as e:
+            if is_commit:
+                db.rollback()
             raise e
         if is_commit:
             db.commit()
 
     async def count(self, db: Session, args: ListArgsSchema) -> int:
         """
         获取记录数
```

### Comparing `fastapi_assistant-0.1.25/fastapi_assistant/bases/enums.py` & `fastapi_assistant-0.1.27/fastapi_assistant/bases/enums.py`

 * *Files identical despite different names*

### Comparing `fastapi_assistant-0.1.25/fastapi_assistant/bases/model.py` & `fastapi_assistant-0.1.27/fastapi_assistant/bases/model.py`

 * *Files identical despite different names*

### Comparing `fastapi_assistant-0.1.25/fastapi_assistant/bases/schema.py` & `fastapi_assistant-0.1.27/fastapi_assistant/bases/schema.py`

 * *Files identical despite different names*

### Comparing `fastapi_assistant-0.1.25/fastapi_assistant/bases/service.py` & `fastapi_assistant-0.1.27/fastapi_assistant/bases/service.py`

 * *Files identical despite different names*

### Comparing `fastapi_assistant-0.1.25/fastapi_assistant/builder_api.py` & `fastapi_assistant-0.1.27/fastapi_assistant/builder_api.py`

 * *Files identical despite different names*

### Comparing `fastapi_assistant-0.1.25/fastapi_assistant/builder_db_engine.py` & `fastapi_assistant-0.1.27/fastapi_assistant/builder_db_engine.py`

 * *Files identical despite different names*

### Comparing `fastapi_assistant-0.1.25/fastapi_assistant/core/exceptions.py` & `fastapi_assistant-0.1.27/fastapi_assistant/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_assistant-0.1.25/fastapi_assistant/core/scheduler.py` & `fastapi_assistant-0.1.27/fastapi_assistant/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `fastapi_assistant-0.1.25/fastapi_assistant/core/sqlalchemy.py` & `fastapi_assistant-0.1.27/fastapi_assistant/core/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fastapi_assistant-0.1.25/fastapi_assistant/libs/date_time.py` & `fastapi_assistant-0.1.27/fastapi_assistant/libs/date_time.py`

 * *Files identical despite different names*

### Comparing `fastapi_assistant-0.1.25/fastapi_assistant/libs/excel_tool.py` & `fastapi_assistant-0.1.27/fastapi_assistant/libs/excel_tool.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import os
-import random
 from io import BytesIO
-from typing import List
+from typing import List, Dict
+from urllib.parse import quote
 
 import numpy as np
+from fastapi import UploadFile
 from fastapi.responses import StreamingResponse
 import pandas as pd
 from styleframe import StyleFrame
 
 
 def export_exl(header: List[str], data, file_name='download.xlsx') -> StreamingResponse:
     output = BytesIO()
@@ -26,82 +26,83 @@
         best_fit=best_fit,
         columns_and_rows_to_freeze=columns_and_rows_to_freeze,
         row_to_add_filters=0,
     )
     excel_writer.close()
     output.seek(0)
     headers = {"content-type": "application/vnd.ms-excel",
-               "content-disposition": 'attachment;filename={}'.format(file_name.encode("utf-8").decode("latin1"))}
+               "content-disposition": 'attachment;filename={}'.format(quote(file_name))}
     return StreamingResponse(output, media_type='xls/xlsx', headers=headers)
 
 
+def export_csv(data: List, file_name='download.csv') -> StreamingResponse:
+    output = BytesIO()
+    df = pd.DataFrame(data)
+    df.to_csv(output, index=False, encoding='utf-8_sig')
+    output.seek(0)
+    headers = {"content-type": "application/vnd.ms-excel",
+               "content-disposition": 'attachment;filename={}'.format(quote(file_name))}
+    return StreamingResponse(output, media_type='text/csv', headers=headers)
+
+
 class ExcelTools:
     def __init__(self, columns_map=None, order=None):
         """
         :param columns_map: 列名映射 => {"name":"姓名"，"score":"成绩","sex":"性别"}
         :param order: 列排序列表 => ["name","sex","score"]
         """
         self.columns_map = columns_map
         self.order = order
 
-    def excel_to_df(self, excel, skip_rows=0) -> pd.DataFrame:
-        fx = excel.read()
-        file_name = ''.join(random.choice("0123456789abcdefgh") for i in range(16)) + '.xlsx'
-        try:
-            with open(file_name, 'wb') as f:
-                f.write(fx)
-
-            df = pd.read_excel(file_name, skiprows=skip_rows)
-        except Exception as e:
-            raise e
-        finally:
-            os.remove(file_name)
-        df = df.replace(np.nan, '', regex=True)
+    async def excel_to_df(self, excel: UploadFile, skip_rows=0) -> pd.DataFrame:
+        contents = await excel.read()
+        buffer = BytesIO(contents)
+        df = pd.read_excel(buffer, skiprows=skip_rows)
+
+        df.replace(np.nan, '', inplace=True)
 
         # 去除所有列数据中的空格
-        df = df.applymap(lambda x: x.strip() if isinstance(x, str) else x)
+        df = df.apply(lambda x: x.str.strip() if x.dtype == "object" else x)
 
         # 列名映射
         if self.columns_map:
             columns_map = dict(zip(self.columns_map.values(), self.columns_map.keys()))
-            df = df.rename(columns=columns_map)
+            df.rename(columns=columns_map, inplace=True)
 
         return df
 
-    def excel_to_dict(self, excel, skip_rows=0):
+    async def excel_to_dict(self, excel: UploadFile, skip_rows=0):
         """
         Excel转Python dict
         :param excel:
         :param skip_rows:
         :return:
         """
-        if not excel:
-            return []
-        df = self.excel_to_df(excel, skip_rows=skip_rows)
-        result = df.to_dict(orient='records')
-        return result
+        if excel:
+            df = await self.excel_to_df(excel, skip_rows=skip_rows)
+            return df.to_dict(orient='records')
+        return []
 
-    def dict_to_excel(self, datas):
+    def dict_to_excel(self, datas: List[Dict]):
         """
         :param datas: 数据集 => [{"name":"张三","score":90，"sex":"男"}]
         :return:
         """
         output = BytesIO()
         pf = pd.DataFrame(datas)
         if self.order:
             pf = pf[self.order]
-        # 将列名替换为中文
         if self.columns_map:
             pf.rename(columns=self.columns_map, inplace=True)
-        # 指定生成的Excel表格名称
-        writer = pd.ExcelWriter(output, engine='xlsxwriter')
-        pf.fillna(' ', inplace=True)
-        pf.to_excel(writer, sheet_name='sheet1', index=False)
-        worksheet = writer.sheets['sheet1']
-
-        for i, col in enumerate(pf.columns):
-            column_len = pf[col].astype(str).str.len().max()
-            column_len = max(column_len, len(col)) + 2
-            worksheet.set_column(i, i, column_len)
-        writer.close()
+
+        with pd.ExcelWriter(output, engine='xlsxwriter') as writer:
+            pf.fillna(' ', inplace=True)
+            pf.to_excel(writer, sheet_name='sheet1', index=False)
+            worksheet = writer.sheets['sheet1']
+
+            for i, col in enumerate(pf.columns):
+                column_len = pf[col].astype(str).str.len().max()
+                column_len = max(column_len, len(col)) + 2
+                worksheet.set_column(i, i, column_len)
+
         output.seek(0)
         return output
```

### Comparing `fastapi_assistant-0.1.25/fastapi_assistant/log_settings.py` & `fastapi_assistant-0.1.27/fastapi_assistant/log_settings.py`

 * *Files identical despite different names*

### Comparing `fastapi_assistant-0.1.25/fastapi_assistant.egg-info/PKG-INFO` & `fastapi_assistant-0.1.27/fastapi_assistant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-assistant
-Version: 0.1.25
+Version: 0.1.27
 Summary: fastapi脚手架，封装了基本curd、excel处理、异常、仿照django实现的get_or_one,create_or_update
 Home-page: https://gitee.com/ileona/fastapi-assistant.git
 Author: lxshen
 Author-email: lxshen613@163.com
 License: UNKNOWN
 Description: ### RestFastApi
             fast_api脚手架，封装了一些基本工具和curl
```

### Comparing `fastapi_assistant-0.1.25/fastapi_assistant.egg-info/SOURCES.txt` & `fastapi_assistant-0.1.27/fastapi_assistant.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 fastapi_assistant/core/__init__.py
 fastapi_assistant/core/exceptions.py
 fastapi_assistant/core/scheduler.py
 fastapi_assistant/core/sqlalchemy.py
 fastapi_assistant/libs/__init__.py
 fastapi_assistant/libs/date_time.py
 fastapi_assistant/libs/excel_tool.py
-fastapi_assistant/libs/pagination.py
+fastapi_assistant/libs/pagination.py
+fastapi_assistant/libs/template_import.py
```

### Comparing `fastapi_assistant-0.1.25/setup.py` & `fastapi_assistant-0.1.27/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 setuptools.setup(
     name="fastapi_assistant",  # 模块名称
-    version="0.1.25",  # 当前版本
+    version="0.1.27",  # 当前版本
     author="lxshen",  # 作者w
     author_email="lxshen613@163.com",  # 作者邮箱
     description="fastapi脚手架，封装了基本curd、excel处理、异常、仿照django实现的get_or_one,create_or_update",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     url="https://gitee.com/ileona/fastapi-assistant.git",  # 模块github地址
     # packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
```

