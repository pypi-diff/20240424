# Comparing `tmp/monzo_utils-0.0.9-py3-none-any.whl.zip` & `tmp/monzo_utils-0.0.90-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,42 @@
-Zip file size: 24676 bytes, number of entries: 23
+Zip file size: 37971 bytes, number of entries: 40
 -rw-r--r--  2.0 unx        0 b- defN 23-Nov-10 22:36 monzo_utils/lib/__init__.py
--rw-r--r--  2.0 unx     9628 b- defN 23-Nov-11 09:35 monzo_utils/lib/db.py
--rw-r--r--  2.0 unx    24974 b- defN 23-Nov-11 09:37 monzo_utils/lib/monzo_api.py
+-rw-r--r--  2.0 unx     1419 b- defN 24-Jan-25 21:32 monzo_utils/lib/config.py
+-rw-r--r--  2.0 unx     7941 b- defN 24-Jan-25 21:32 monzo_utils/lib/db.py
+-rw-r--r--  2.0 unx     1870 b- defN 23-Nov-12 13:34 monzo_utils/lib/log.py
+-rw-r--r--  2.0 unx     9336 b- defN 24-Apr-24 19:11 monzo_utils/lib/monzo_api.py
+-rw-r--r--  2.0 unx    27325 b- defN 24-Apr-20 12:23 monzo_utils/lib/monzo_payments.py
+-rw-r--r--  2.0 unx    19498 b- defN 24-Apr-24 19:11 monzo_utils/lib/monzo_sync.py
 -rw-r--r--  2.0 unx      238 b- defN 23-Nov-10 20:55 monzo_utils/lib/singleton.py
+-rw-r--r--  2.0 unx      108 b- defN 24-Jan-25 21:32 monzo_utils/lib/transactions_seen.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Nov-12 20:00 monzo_utils/lib/db_driver/__init__.py
+-rw-r--r--  2.0 unx     1579 b- defN 23-Nov-12 20:51 monzo_utils/lib/db_driver/mysql.py
+-rw-r--r--  2.0 unx     1259 b- defN 23-Nov-12 20:39 monzo_utils/lib/db_driver/sqlite.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Nov-10 22:36 monzo_utils/model/__init__.py
--rw-r--r--  2.0 unx     1729 b- defN 23-Nov-10 22:44 monzo_utils/model/account.py
--rw-r--r--  2.0 unx     2796 b- defN 23-Nov-11 09:35 monzo_utils/model/base.py
+-rw-r--r--  2.0 unx     2252 b- defN 24-Feb-01 22:37 monzo_utils/model/account.py
+-rw-r--r--  2.0 unx      465 b- defN 23-Nov-11 18:09 monzo_utils/model/amazon_payments.py
+-rw-r--r--  2.0 unx     5029 b- defN 24-Feb-01 22:37 monzo_utils/model/base.py
+-rw-r--r--  2.0 unx       85 b- defN 23-Nov-11 18:09 monzo_utils/model/card_payment.py
 -rw-r--r--  2.0 unx       87 b- defN 23-Nov-10 22:43 monzo_utils/model/counterparty.py
+-rw-r--r--  2.0 unx       85 b- defN 23-Nov-11 18:09 monzo_utils/model/direct_debit.py
+-rw-r--r--  2.0 unx     2780 b- defN 24-Feb-01 22:37 monzo_utils/model/finance.py
+-rw-r--r--  2.0 unx     6011 b- defN 24-Jan-31 23:46 monzo_utils/model/flex.py
+-rw-r--r--  2.0 unx     3020 b- defN 24-Feb-09 19:23 monzo_utils/model/flex_summary.py
 -rw-r--r--  2.0 unx       83 b- defN 23-Nov-10 22:43 monzo_utils/model/merchant.py
 -rw-r--r--  2.0 unx       90 b- defN 23-Nov-10 22:43 monzo_utils/model/merchant_address.py
+-rw-r--r--  2.0 unx    16506 b- defN 24-Apr-20 12:23 monzo_utils/model/payment.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Nov-10 22:43 monzo_utils/model/pot.py
 -rw-r--r--  2.0 unx      629 b- defN 23-Nov-10 22:43 monzo_utils/model/provider.py
--rw-r--r--  2.0 unx      159 b- defN 23-Nov-10 22:43 monzo_utils/model/transaction.py
+-rw-r--r--  2.0 unx      564 b- defN 24-Jan-25 21:32 monzo_utils/model/refund.py
+-rw-r--r--  2.0 unx       87 b- defN 23-Nov-11 18:09 monzo_utils/model/standing_order.py
+-rw-r--r--  2.0 unx      393 b- defN 23-Nov-12 20:42 monzo_utils/model/transaction.py
 -rw-r--r--  2.0 unx       94 b- defN 23-Nov-10 22:43 monzo_utils/model/transaction_metadata.py
--rwxr-xr-x  2.0 unx    28797 b- defN 23-Nov-11 09:38 monzo_utils-0.0.9.data/scripts/monzo-payments
--rwxr-xr-x  2.0 unx    12731 b- defN 23-Nov-11 09:38 monzo_utils-0.0.9.data/scripts/monzo-search
--rwxr-xr-x  2.0 unx     3514 b- defN 23-Nov-11 09:38 monzo_utils-0.0.9.data/scripts/monzo-status
--rwxr-xr-x  2.0 unx      509 b- defN 23-Nov-11 09:38 monzo_utils-0.0.9.data/scripts/monzo-sync
--rw-r--r--  2.0 unx     1078 b- defN 23-Nov-11 09:38 monzo_utils-0.0.9.dist-info/LICENSE
--rw-r--r--  2.0 unx      307 b- defN 23-Nov-11 09:38 monzo_utils-0.0.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Nov-11 09:38 monzo_utils-0.0.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       35 b- defN 23-Nov-11 09:38 monzo_utils-0.0.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1997 b- defN 23-Nov-11 09:38 monzo_utils-0.0.9.dist-info/RECORD
-23 files, 89644 bytes uncompressed, 21382 bytes compressed:  76.1%
+-rwxr-xr-x  2.0 unx      897 b- defN 24-Apr-24 19:12 monzo_utils-0.0.90.data/scripts/monzo-payments
+-rwxr-xr-x  2.0 unx    12970 b- defN 24-Apr-24 19:12 monzo_utils-0.0.90.data/scripts/monzo-search
+-rwxr-xr-x  2.0 unx     3241 b- defN 24-Apr-24 19:12 monzo_utils-0.0.90.data/scripts/monzo-status
+-rwxr-xr-x  2.0 unx      688 b- defN 24-Apr-24 19:12 monzo_utils-0.0.90.data/scripts/monzo-sync
+-rw-r--r--  2.0 unx     1078 b- defN 24-Apr-24 19:12 monzo_utils-0.0.90.dist-info/LICENSE
+-rw-r--r--  2.0 unx      479 b- defN 24-Apr-24 19:12 monzo_utils-0.0.90.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 19:12 monzo_utils-0.0.90.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-Apr-24 19:12 monzo_utils-0.0.90.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3492 b- defN 24-Apr-24 19:12 monzo_utils-0.0.90.dist-info/RECORD
+40 files, 131908 bytes uncompressed, 32309 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -1,70 +1,121 @@
 Filename: monzo_utils/lib/__init__.py
 Comment: 
 
+Filename: monzo_utils/lib/config.py
+Comment: 
+
 Filename: monzo_utils/lib/db.py
 Comment: 
 
+Filename: monzo_utils/lib/log.py
+Comment: 
+
 Filename: monzo_utils/lib/monzo_api.py
 Comment: 
 
+Filename: monzo_utils/lib/monzo_payments.py
+Comment: 
+
+Filename: monzo_utils/lib/monzo_sync.py
+Comment: 
+
 Filename: monzo_utils/lib/singleton.py
 Comment: 
 
+Filename: monzo_utils/lib/transactions_seen.py
+Comment: 
+
+Filename: monzo_utils/lib/db_driver/__init__.py
+Comment: 
+
+Filename: monzo_utils/lib/db_driver/mysql.py
+Comment: 
+
+Filename: monzo_utils/lib/db_driver/sqlite.py
+Comment: 
+
 Filename: monzo_utils/model/__init__.py
 Comment: 
 
 Filename: monzo_utils/model/account.py
 Comment: 
 
+Filename: monzo_utils/model/amazon_payments.py
+Comment: 
+
 Filename: monzo_utils/model/base.py
 Comment: 
 
+Filename: monzo_utils/model/card_payment.py
+Comment: 
+
 Filename: monzo_utils/model/counterparty.py
 Comment: 
 
+Filename: monzo_utils/model/direct_debit.py
+Comment: 
+
+Filename: monzo_utils/model/finance.py
+Comment: 
+
+Filename: monzo_utils/model/flex.py
+Comment: 
+
+Filename: monzo_utils/model/flex_summary.py
+Comment: 
+
 Filename: monzo_utils/model/merchant.py
 Comment: 
 
 Filename: monzo_utils/model/merchant_address.py
 Comment: 
 
+Filename: monzo_utils/model/payment.py
+Comment: 
+
 Filename: monzo_utils/model/pot.py
 Comment: 
 
 Filename: monzo_utils/model/provider.py
 Comment: 
 
+Filename: monzo_utils/model/refund.py
+Comment: 
+
+Filename: monzo_utils/model/standing_order.py
+Comment: 
+
 Filename: monzo_utils/model/transaction.py
 Comment: 
 
 Filename: monzo_utils/model/transaction_metadata.py
 Comment: 
 
-Filename: monzo_utils-0.0.9.data/scripts/monzo-payments
+Filename: monzo_utils-0.0.90.data/scripts/monzo-payments
 Comment: 
 
-Filename: monzo_utils-0.0.9.data/scripts/monzo-search
+Filename: monzo_utils-0.0.90.data/scripts/monzo-search
 Comment: 
 
-Filename: monzo_utils-0.0.9.data/scripts/monzo-status
+Filename: monzo_utils-0.0.90.data/scripts/monzo-status
 Comment: 
 
-Filename: monzo_utils-0.0.9.data/scripts/monzo-sync
+Filename: monzo_utils-0.0.90.data/scripts/monzo-sync
 Comment: 
 
-Filename: monzo_utils-0.0.9.dist-info/LICENSE
+Filename: monzo_utils-0.0.90.dist-info/LICENSE
 Comment: 
 
-Filename: monzo_utils-0.0.9.dist-info/METADATA
+Filename: monzo_utils-0.0.90.dist-info/METADATA
 Comment: 
 
-Filename: monzo_utils-0.0.9.dist-info/WHEEL
+Filename: monzo_utils-0.0.90.dist-info/WHEEL
 Comment: 
 
-Filename: monzo_utils-0.0.9.dist-info/top_level.txt
+Filename: monzo_utils-0.0.90.dist-info/top_level.txt
 Comment: 
 
-Filename: monzo_utils-0.0.9.dist-info/RECORD
+Filename: monzo_utils-0.0.90.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## monzo_utils/lib/db.py

```diff
@@ -1,201 +1,131 @@
 import MySQLdb
 import re
 import sys
 import os
 import json
 import datetime
+import importlib
 from monzo_utils.lib.singleton import Singleton
+from monzo_utils.lib.config import Config
 
 class DB(metaclass=Singleton):
 
-    def __getattr__(self, name):
-        match = re.match('^find_([\w]+)_by_(.*?)$', name)
-
-        if match:
-            table = match.group(1)
-
-            if table[0:4] == 'all_':
-                table = table[4:]
-                find_all = True
-            else:
-                find_all = False
-
-            fields = match.group(2).split('_and_')
-
-            def find_object_by_fields(*args, **kwargs):
-                sql = "select * from `" + table + "` where ("
-
-                sql_args = []
-
-                for i in range(0, len(fields)):
-                    if i >0:
-                        sql += " and "
-
-                    if type(args[i]) == list:
-                        sql += "("
-                        for j in range(0, len(args[i])):
-                            if j >0:
-                                sql += " or "
-
-                            if 'search' in kwargs and type(kwargs['search']) == list and fields[i] in kwargs['search']:
-                                sql += f"`{fields[i]}` like %s"
-                                sql_args.append('%' + args[i][j] + '%')
-                            else:
-                                sql += f"`{fields[i]}` = %s"
-                                sql_args.append(args[i][j])
-
-                        sql += ")"
-                    else:
-                        if 'search' in kwargs and type(kwargs['search']) == list and fields[i] in kwargs['search']:
-                            sql += "`" + fields[i] + "` like %s"
-                            sql_args.append('%' + args[i] + '%')
-                        else:
-                            sql += "`" + fields[i] + "` = %s"
-                            sql_args.append(args[i])
-
-                sql += ")"
-
-                if 'where' in kwargs:
-                    for where_clause in kwargs['where']:
-                        sql += f" and {where_clause['clause']}"
-
-                        if 'params' in where_clause:
-                            sql_args += where_clause['params']
-
-                if 'orderby' in kwargs:
-                    sql += f" order by {kwargs['orderby']}"
-
-                    if 'orderdir' in kwargs:
-                        sql += f" {kwargs['orderdir']}"
-
-                if 'limit' in kwargs:
-                    sql += f" limit {kwargs['limit']}"
-
-                if find_all:
-                    return self.query(sql, sql_args)
-                else:
-                    return self.one(sql, sql_args)
-
-            return find_object_by_fields
+    def __init__(self, db_config=None, config_path=None):
+        if db_config:
+            self.config = db_config
         else:
-            print("DB class method missing: %s" % (name))
-            sys.exit(1)
+            self.config = Config(None, config_path).db
 
+        self.driver = getattr(importlib.import_module(f"monzo_utils.lib.db_driver.{self.config['driver']}"), self.config['driver'])(self.config)
 
-    def __init__(self, config):
-        self.config = config
         self.columns = {}
-        self.connect()
-
-
-    def connect(self):
-        self.db = MySQLdb.connect(
-            host=self.config['host'],
-            port=self.config['port'],
-            user=self.config['user'],
-            passwd=self.config['password'],
-            db=self.config['database'],
-            charset='utf8',
-            use_unicode=True,
-            ssl={}
-        )
-        self.cur = self.db.cursor()
 
 
     def json_params(self, params):
         json_params = []
 
         for param in params:
             if type(param) == datetime.date:
-                json_params.append(param.strftime('%Y-%M-%d'))
+                json_params.append(param.strftime('%Y-%m-%d'))
             elif type(param) == datetime.datetime:
-                json_params.append(param.strftime('%Y-%M-%d %H:%M:%S'))
+                json_params.append(param.strftime('%Y-%m-%d %H:%M:%S'))
             else:
                 json_params.append(param)
 
         return json_params
 
 
     def query(self, sql, params=[]):
         if 'DEBUG' in os.environ and os.environ['DEBUG'] == '1':
             print("SQL: %s" % (sql))
             print("PARAMS: %s" % (json.dumps(self.json_params(params),indent=4)))
 
-        self.cur.execute((sql), params)
+        result = self.driver.query(sql, params)
 
-        if sql[0:6].lower() == "select":
-            self.db.commit()
-            return self.build_rows(self.cur.fetchall())
+        if type(result) == list:
+            rows = []
 
-        self.db.commit()
+            for row in result:
+                rows.append(self.fix_dates(row))
 
-        if sql[0:6].lower() == "insert":
-            return self.cur.lastrowid
+            result = rows
 
-        return None
+        return result
 
 
-    def one(self, sql, params=[]):
-        rows = self.query(sql, params)
+    def fix_dates(self, row):
+        fixed_row = {}
 
-        if len(rows) >0:
-            return rows[0]
+        for key in row:
+            if type(row[key]) == str:
+                m = re.match(r'^([\d]{4})-([\d]{2})-([\d]{2})$', row[key])
 
-        return False
+                if m:
+                    fixed_row[key] = datetime.date(int(m.group(1)), int(m.group(2)), int(m.group(3)))
+                    continue
 
+                m = re.match(r'^([\d]{4})-([\d]{2})-([\d]{2}) ([\d]{2}):([\d]{2}):([\d]{2})$', row[key])
 
-    def build_row(self, data):
-        row = {}
+                if m:
+                    fixed_row[key] = datetime.datetime(int(m.group(1)), int(m.group(2)), int(m.group(3)), int(m.group(4)), int(m.group(5)), int(m.group(6)))
+                    continue
 
-        for i in range(0, len(self.cur.description)):
-            row[self.cur.description[i][0]] = data[i]
+            fixed_row[key] = row[key]
 
-        return row
+        return fixed_row
 
 
-    def build_rows(self, data):
-        rows = []
+    def one(self, sql, params=[]):
+        rows = self.query(sql, params)
 
-        for item in data:
-            rows.append(self.build_row(item))
+        if len(rows) >0:
+            return rows[0]
 
-        return rows
+        return False
 
 
     def find(self, table):
-        self.sel = '*'
         self.query_table = table
+        self.sel = []
         self.whereClauses = []
         self.whereParams = []
-        self.whereType = 'and'
-        self.orderBy = None
-        self.orderDir = None
+        self.andWhereClauses = []
+        self._orderBy = None
+        self._orderDir = None
         self._join = []
         self._leftJoin = []
+        self._groupBy = None
 
         return self
 
 
-    def select(self, select_str):
-        self.sel = select_str
+    def select(self, select):
+        self.sel.append(select)
 
         return self
 
 
-    def where(self, where, *whereParams):
+    def where(self, where, whereParams):
         self.whereClauses.append(where)
         self.whereParams += whereParams
 
         return self
 
 
-    def orderby(self, field, direction='asc'):
-        self.orderBy = field
-        self.orderDir = direction
+    def andWhere(self, where, whereParams):
+        self.andWhereClauses.append(where)
+        self.whereParams += whereParams
+
+        return self
+
+
+    def orderBy(self, field, direction='asc'):
+        self._orderBy = field
+        self._orderDir = direction
 
         return self
 
 
     def join(self, join_table, join_left_col, join_right_col=None):
         if join_right_col:
             self._join.append({
@@ -208,38 +138,49 @@
                 'table': join_table,
                 'clause': join_left_col
             })
 
         return self
 
 
-    def leftJoin(self, join_table, join_left_col, join_right_col=None):
-        if join_right_col:
-            self._leftJoin.append({
-                'table': join_table,
-                'join_left_col': join_left_col,
-                'join_right_col': join_right_col
-            })
-        else:
-            self._leftJoin.append({
-                'table': join_table,
-                'clause': join_left_col
-            })
+    def leftJoin(self, join_table, join_left_col, join_right_col, where=None):
+        self._leftJoin.append({
+            'table': join_table,
+            'join_left_col': join_left_col,
+            'join_right_col': join_right_col,
+            'where': where
+        })
 
         return self
 
 
     def orWhere(self, whereClause, whereParams=[]):
         self.whereType = 'or'
 
         return self.where(whereClause, whereParams)
 
 
+    def groupBy(self, groupBy):
+        self._groupBy = groupBy
+
+        return self
+
+
     def prepare(self):
-        sql = "select " + self.sel + " from `" + self.query_table + "`"
+        if self.sel == []:
+            select = '*'
+        else:
+            select = ''
+
+            for i in range(0, len(self.sel)):
+                if i >0:
+                    select += ','
+                select += f"{self.sel[i]}"
+
+        sql = "select " + select + " from `" + self.query_table + "`"
 
         for join in self._join:
             sql += " join `" + join['table'] + "` on "
 
             if 'clause' in join:
                 sql += join['clause']
             else:
@@ -249,27 +190,41 @@
             sql += " left join `" + join['table'] + "` on "
 
             if 'clause' in join:
                 sql += join['clause']
             else:
                 sql += join['join_left_col'] + " = " + join['join_right_col']
 
-        for i in range(0, len(self.whereClauses)):
-            if i >0:
-                sql += " " + self.whereType + " "
-            else:
-                sql += " where "
+        if len(self.whereClauses) >0:
+            sql += " where ("
+
+            for i in range(0, len(self.whereClauses)):
+                if i >0:
+                    sql += " or "
+                sql += self.whereClauses[i]
 
-            sql += self.whereClauses[i]
+            sql += ")"
 
-        if self.orderBy:
-            sql += " order by `" + self.orderBy + "`"
+            for i in range(0, len(self.andWhereClauses)):
+                sql += " and (" + self.andWhereClauses[i] + ") "
 
-        if self.orderDir:
-            sql += " " + self.orderDir
+        if self._groupBy:
+            sql += " group by " + self._groupBy
+
+        if self._orderBy:
+            sql += " order by "
+            order_by_fields = self._orderBy.split(',')
+
+            for i in range(0, len(order_by_fields)):
+                if i >0:
+                    sql += ","
+                sql += f" `{order_by_fields[i].strip()}`"
+
+        if self._orderDir:
+            sql += " " + self._orderDir
 
         return sql
 
 
     def getone(self):
         sql = self.prepare() + " limit 1"
 
@@ -295,36 +250,29 @@
 
         for i in range(0, len(sql)):
             if skip:
                 skip = False
                 continue
 
             if sql[i:i+2] == '%s':
-                raw_sql += "'" + self.whereParams[n] + "'"
+                if type(self.whereParams[n]) in [int,float]:
+                    raw_sql += str(self.whereParams[n])
+                else:
+                    raw_sql += "'" + str(self.whereParams[n]) + "'"
                 n += 1
                 skip = True
             else:
                 raw_sql += sql[i]
 
         return raw_sql
 
 
-    def get_columns(self, table):
-        columns = []
-
-        for row in self.query("select column_name from information_schema.columns where table_schema = %s and table_name = %s", [self.config['database'], table]):
-            if row['column_name'] != 'id':
-                columns.append(row['column_name'])
-
-        return columns
-
-
     def update(self, table, _id, data):
         if table not in self.columns:
-            self.columns[table] = self.get_columns(table)
+            self.columns[table] = self.driver.get_columns(table, exclude=['id'])
 
         sql = f"update `{table}` set"
         params = []
 
         for i in range(0, len(self.columns[table])):
             if i >0:
                 sql += ", "
@@ -336,15 +284,15 @@
         params.append(_id)
 
         self.query(sql, params)
 
 
     def create(self, table, data):
         if table not in self.columns:
-            self.columns[table] = self.get_columns(table)
+            self.columns[table] = self.driver.get_columns(table, exclude=['id'])
 
         sql = f"insert into `{table}` ("
         params = []
 
         for i in range(0, len(self.columns[table])):
             if i >0:
                 sql += ","
```

## monzo_utils/lib/monzo_api.py

```diff
@@ -10,768 +10,309 @@
 import pwd
 from pathlib import Path
 from monzo.authentication import Authentication
 import monzo.endpoints.account
 import monzo.endpoints.pot
 import monzo.endpoints.transaction
 from monzo.exceptions import MonzoAuthenticationError, MonzoServerError, MonzoHTTPError, MonzoPermissionsError
-from monzo_utils.lib.db import DB
-from monzo_utils.model.provider import Provider
-from monzo_utils.model.account import Account
-from monzo_utils.model.merchant import Merchant
-from monzo_utils.model.merchant_address import MerchantAddress
-from monzo_utils.model.pot import Pot
-from monzo_utils.model.transaction import Transaction
-from monzo_utils.model.counterparty import Counterparty
-from monzo_utils.model.transaction_metadata import TransactionMetadata
+from monzo_utils.lib.log import Log
+from monzo_utils.lib.config import Config
 
-PROVIDER = 'Monzo'
+class MonzoAPI:
 
-class Monzo:
-
-    def __init__(self, no_init=False):
+    def __init__(self, tmp=None):
         homedir = pwd.getpwuid(os.getuid()).pw_dir
-        monzo_dir = f"{homedir}/.monzo"
-
-        if not os.path.exists(monzo_dir):
-            os.mkdir(monzo_dir, 0o755)
-
-        self.config_file = f"{monzo_dir}/config.yaml"
-        self.token_file = f"{monzo_dir}/tokens"
-
-        if no_init:
-            return
-
-        if not os.path.exists(self.config_file):
-            sys.stderr.write(f"config file not found: {self.config_file}, run setup first.\n")
-            sys.exit(1)
+        self.monzo_dir = f"{homedir}/.monzo"
+        self.token_file = f"{self.monzo_dir}/tokens"
 
-        try:
-            self.config = yaml.safe_load(open(self.config_file).read())
-        except Exception as e:
-            sys.stderr.write(f"could not read config file: {self.config_file}, {str(e)}\n")
-            sys.exit(1)
-
-        self.db = DB(self.config['db'])
-
-        self.provider = self.get_provider()
-
-        self.load_tokens()
+        self.load_tokens(tmp)
 
         self.client = self.get_client()
 
 
-    def load_tokens(self):
+    def load_tokens(self, tmp=None):
         if os.path.exists(self.token_file):
             data = json.loads(open(self.token_file).read())
 
             self.access_token = data['access_token']
             self.access_token_expiry = data['expiry']
             self.refresh_token = data['refresh_token']
         else:
-            self.authenticate()
+            self.authenticate(tmp)
 
  
-    def setup(self):
-        print("\n========================")
-        print("Monzo Utils Setup Wizard")
-        print("========================\n")
-        print("Requirements:\n")
-        print("1) You must have created an OAuth client here: https://developers.monzo.com/apps/new")
-        print("   Note: confidentiality must be set to Confidential\n")
-        print("2) The MySQL database must be ready (see README.md)\n")
-        print("3) The machine we are running on must be reachable on a known port from the internet.")
-        print("   The webserver must be configured with the CGI script to capture the oauth tokens.")
-        print("   This is only required during setup for the initial oauth authentication flow.")
-        print("   Once this is complete and the tokens are stored this can be removed.\n")
-
-        self.prompt_continue()
-
-        if os.path.exists(self.config_file):
-            sys.stdout.write(f"\nWARNING! Config file already exists at: {self.config_file}\n\n")
-            sys.stdout.write("If we continue this will be erased.\n\n")
-
-            self.prompt_continue()
-
-        sys.stdout.write("\n")
-
-        mysql_host = self.prompt_input('MySQL host', '127.0.0.1')
-        mysql_port = self.prompt_input('MySQL port', '3306', False, 'int')
-        mysql_db = self.prompt_input('MySQL database', 'monzo')
-        mysql_user = self.prompt_input('MySQL username', 'monzo')
-        mysql_password = self.prompt_input('MySQL password', 'monzo')
-
-        db = {
-            'host': mysql_host,
-            'port': mysql_port,
-            'user': mysql_user,
-            'password': mysql_password,
-            'database': mysql_db
-        }
-
-        self.test_db_access(db)
-
-        sys.stdout.write("\n")
-
-        client_id = self.prompt_input('Monzo Client ID')
-        client_secret = self.prompt_input('Monzo Client Secret')
-        redirect_url = self.prompt_input('Monzo Client redirect URL')
-
-        sys.stdout.write("Enter the path where the CGI script will store the token file:\n")
-
-        token_path = self.prompt_input('Token path', '/var/www/monzo/token')
-
-        sys.stdout.write("\nIf the auth token expires or stops working the sync script can send\n")
-        sys.stdout.write("an email to notify you. Enter this email below or leave blank if not required.\n")
-
-        email = self.prompt_input('Email', None, True)
-
-        self.config = {
-            'oauth_token_file': token_path,
-            'db': db,
-            'client_id': client_id,
-            'client_secret': client_secret,
-            'redirect_url': redirect_url,
-            'email': email
-        }
-
-        self.save_config()
-
-        self.__init__()
-
-        self.scan_accounts()
-
-        sys.stdout.write("Performing initial transaction sync ...\n\n")
-        sys.stdout.flush()
-
-        self.sync()
-
-        sys.stdout.write("Setup complete!\n\n")
-
-
-    def save_config(self):
-        with open(self.config_file, 'w') as f:
-            f.write(yaml.dump(self.config))
-
-
-    def scan_accounts(self):
-        sys.stdout.write("\nFinding accounts...\n\n")
-
-        accounts = monzo.endpoints.account.Account.fetch(self.client)
-
-        found_accounts = []
-
-        for account in accounts:
-            if account.balance is None:
-                continue
-
-            if 'accounts' in self.config and account.account_id in self.config['accounts']:
-                continue
-
-            if 'Joint account between' in account.description:
-                account_type = 'Joint Current Account'
-            else:
-                account_type = account.account_type()
-
-            print(f"         id: {account.account_id}")
-            print(f"    balance: £{account.balance.balance/100:.2f}")
-            print(f"description: {account.description}")
-            print(f"       type: {account_type}")
-
-            sys.stdout.write("\n")
-
-            resp = self.prompt_continue('Sync this account? [y/N] ', True)
-
-            if resp == 'n':
-                continue
-
-            account_name = self.prompt_input('name for this account')
-
-            if 'accounts' not in self.config:
-                self.config['accounts'] = {}
-
-            self.config['accounts'][account.account_id] = {
-                'name': account_name
-            }
-
-            if account_type == 'Flex':
-                self.config['accounts'][account.account_id]['credit_limit'] = self.prompt_input('credit limit', None, False, 'int')
-            else:
-                self.config['accounts'][account.account_id]['sortcode'] = self.prompt_input('sort code')
-                self.config['accounts'][account.account_id]['account_no'] = self.prompt_input('account no')
-
-            sys.stdout.write("\n")
-
-            self.save_config()
-
-
-    def prompt_continue(self, prompt='Continue? [y/N] ', boolean=False):
-        while 1:
-            sys.stdout.write(prompt)
-            sys.stdout.flush()
-
-            resp = sys.stdin.readline().rstrip().lower()
-
-            if resp == 'n':
-                if boolean:
-                    return False
-
-                print("\nStopping at user request.\n")
-                sys.exit(0)
-
-            if resp == 'y':
-                break
-
-        return True
-
- 
-    def prompt_input(self, prompt, default=None, none_allowed=False, validation=None):
-        while 1:
-            if default is None:
-                sys.stdout.write(f"Enter {prompt}: ")
-            else:
-                sys.stdout.write(f"Enter {prompt} [{default}]: ")
-
-            sys.stdout.flush()
-
-            resp = sys.stdin.readline().rstrip()
-
-            if len(resp) == 0:
-                if default is None and none_allowed is False:
-                    continue
-
-                resp = default
-
-            if validation == 'int' and resp is not None:
-                try:
-                    resp = int(resp)
-                except:
-                    sys.stderr.write("\nerror: value must be an integer\n\n")
-                    sys.stderr.flush()
-                    continue
+    def authenticate(self, tmp=None):
+        client = Authentication(
+            client_id=Config().client_id,
+            client_secret=Config().client_secret,
+            redirect_url=Config().redirect_url
+        )
 
-            return resp
+        auth_required_file = f"{self.monzo_dir}/.auth_required"
 
+        if not sys.stdout.isatty():
+            if 'email' in Config().keys:
+                if not os.path.exists(auth_required_file):
+                    with open(auth_required_file,'w') as f:
+                        pass
 
-    def test_db_access(self, db_config):
-        try:
-            db = DB(db_config)
-        except:
-            print("failed")
+                    os.system("echo '%s'| mail -s 'Monzo auth required' '%s'" % (client.authentication_url, Config().email))
 
-        try:
-            resp = db.query("show tables")
-        except Exception as e:
-            sys.stderr.write(f"\nFailed to connect to the database: {str(e)}\n\n")
+            Log().error('Authentication required, unable to sync.')
             sys.exit(1)
 
+        if tmp:
+            with open(tmp + '.tmp','w') as f:
+                f.write(client.authentication_url)
 
-    def authenticate(self):
-        client = Authentication(
-            client_id=self.config['client_id'],
-            client_secret=self.config['client_secret'],
-            redirect_url=self.config['redirect_url']
-        )
-
-        if not sys.stdout.isatty():
-            if 'email' in self.config:
-                os.system("echo '%s'| mail -s 'Monzo auth required' '%s'" % (client.authentication_url, self.config['email']))
-            sys.stderr.write('Authentication required, unable to sync.\n')
-            sys.exit(1)
+            os.rename(tmp + '.tmp', tmp)
+        else:
+            print("\nAuthentication required, check email or visit:\n")
+            print(client.authentication_url)
 
-        print("\nAuthentication required, check email or visit:\n")
-        print(client.authentication_url)
+        if os.path.exists(Config().oauth_token_file):
+            os.remove(Config().oauth_token_file)
 
-        if os.path.exists(self.config['oauth_token_file']):
-            os.remove(self.config['oauth_token_file'])
+        if 'execute_before_auth' in Config().keys:
+            os.system(Config().execute_before_auth)
 
-        while not os.path.exists(self.config['oauth_token_file']):
+        while not os.path.exists(Config().oauth_token_file):
             time.sleep(1)
 
-        data = json.loads(open(self.config['oauth_token_file']).read().rstrip())
+        data = json.loads(open(Config().oauth_token_file).read().rstrip())
 
-        os.remove(self.config['oauth_token_file'])
+        os.remove(Config().oauth_token_file)
 
         try:
             client.authenticate(authorization_token=data['token'], state_token=data['state'])
         except MonzoAuthenticationError:
-            print('State code does not match')
+            Log().error('State code does not match')
             exit(1)
         except MonzoServerError:
-            print('Monzo Server Error')
+            Log().error('Monzo Server Error')
             exit(1)
 
-        with open(self.token_file,'w') as f:
-            f.write(json.dumps({
-                'access_token': client.access_token,
-                'expiry': client.access_token_expiry,
-                'refresh_token': client.refresh_token
-            }))
-
         self.access_token = client.access_token
         self.access_token_expiry = client.access_token_expiry
         self.refresh_token = client.refresh_token
 
+        self.save_tokens()
+
+        if os.path.exists(auth_required_file):
+            os.remove(auth_required_file)
+
+        if 'execute_after_auth' in Config().keys:
+            os.system(Config().execute_after_auth)
+
         self.client = self.get_client()
 
-        print("\n waiting for authorisation...")
+        print("\nwaiting for authorisation...")
 
         while 1:
             time.sleep(1)
 
             try:
                 self.accounts()
                 break
             except MonzoPermissionsError:
                 pass
 
 
+    def save_tokens(self):
+        self.set_file_contents(self.token_file, json.dumps({
+            'access_token': self.access_token,
+            'expiry': self.access_token_expiry,
+            'refresh_token': self.refresh_token
+        }))
+
+
+    def set_file_contents(self, path, content):
+        with open(path + ".new", 'w') as f:
+            f.write(content)
+
+        os.rename(path + ".new", path)
+
+
     def get_client(self):
         return Authentication(
-            client_id=self.config['client_id'],
-            client_secret=self.config['client_secret'],
-            redirect_url=self.config['redirect_url'],
+            client_id=Config().client_id,
+            client_secret=Config().client_secret,
+            redirect_url=Config().redirect_url,
             access_token=self.access_token,
             access_token_expiry=self.access_token_expiry,
             refresh_token=self.refresh_token
         )
 
 
     def account(self, account_id):
         return monzo.endpoints.account.Account.fetch(self.client, account_id=account_id)
 
 
-    def accounts(self, first=True):
-        try:
-            accounts = monzo.endpoints.account.Account.fetch(self.client)
-        except MonzoHTTPError:
-            if first:
-                if 'NO_AUTH' in os.environ:
-                    raise Exception("token expired")
+    def accounts(self, first=True, tmp=None):
+        for i in range(0, 3):
+            try:
+                accounts = monzo.endpoints.account.Account.fetch(self.client)
 
-                self.authenticate()
+                self.update_tokens()
 
-                return self.accounts(False)
+                return accounts
 
-            print("auth failed")
-            sys.exit(1)
-        except MonzoAuthenticationError:
-            if first:
-                self.authenticate()
+            except MonzoHTTPError:
+                if first:
+                    if 'NO_AUTH' in os.environ:
+                        raise Exception("token expired")
 
-                return self.accounts(False)
+                    self.authenticate(tmp)
 
-            print("auth failed")
-            sys.exit(1)
-        except MonzoServerError:
-            print("server error")
-            sys.exit(1)
-        except TimeoutError:
-            print("timeout")
-            sys.exit(1)
+                    return self.accounts(False)
+
+                Log().error('auth failed')
+                sys.exit(1)
+            except MonzoAuthenticationError:
+                if first:
+                    self.authenticate(tmp)
+
+                    return self.accounts(False)
+
+                Log().error("auth failed")
+                sys.exit(1)
+            except MonzoServerError:
+                Log().error("server error")
+
+                if i == 2:
+                    sys.exit(1)
 
-        self.update_tokens()
+                time.sleep(5)
 
-        return accounts
+            except TimeoutError:
+                Log().error("timeout")
+
+                if i == 2:
+                    sys.exit(1)
+
+                time.sleep(5)
+
+        raise Exception("failed to retrieve accounts after 3 attempts")
 
 
     def update_tokens(self):
         if self.access_token == self.client.access_token and \
             self.access_token_expiry == self.client.access_token_expiry and \
             self.refresh_token == self.client.refresh_token:
             return
 
         self.access_token = self.client.access_token
         self.access_token_expiry = self.client.access_token_expiry
         self.refresh_token = self.client.refresh_token
 
-        with open(self.token_file + '.new','w') as f:
-            f.write(json.dumps({
-                'access_token': self.client.access_token,
-                'expiry': self.client.access_token_expiry,
-                'refresh_token': self.client.refresh_token
-            }))
-
-        os.rename(self.token_file + '.new', self.token_file)
+        self.save_tokens()
 
 
-    def transactions(self, account_id):
+    def transactions(self, account_id, days=3):
         error = None
 
+        now = datetime.datetime.utcnow()
+        since = now - datetime.timedelta(days=days)
+
         for i in range(0, 3):
             try:
-                return monzo.endpoints.transaction.Transaction.fetch(self.client, account_id=account_id, expand=['merchant'])
+                return monzo.endpoints.transaction.Transaction.fetch(self.client, account_id=account_id, expand=['merchant'], since=since)
+            except MonzoPermissionsError as e:
+                raise e
             except Exception as e:
                 error = str(e)
 
                 if i != 2:
                     time.sleep(5)
+                else:
+                    raise e
 
-        print("failed to retrieve transactions: %s" % (error))
+        Log().error("failed to retrieve transactions: %s" % (error))
         sys.exit(1)
 
 
-    def pots(self, account_id, first=True):
+    def pots(self, account_id, first=True, tmp=None):
         try:
             pots = monzo.endpoints.pot.Pot.fetch(self.client, account_id=account_id)
         except MonzoHTTPError:
             if first:
                 if 'NO_AUTH' in os.environ:
                     raise Exception("token expired")
 
-                self.authenticate()
+                self.authenticate(tmp)
                 self.client = self.get_client()
 
                 return self.pots(account_id, False)
 
-            print("auth failed")
+            Log().error("auth failed")
             sys.exit(1)
         except MonzoAuthenticationError:
             if first:
-                self.authenticate()
+                self.authenticate(tmp)
                 self.client = self.get_client()
 
                 return self.pots(account_id, False)
 
-            print("auth failed")
+            Log().error("auth failed")
+            sys.exit(1)
+        except MonzoServerError:
+            Log().error("server error")
             sys.exit(1)
         except TimeoutError:
-            print("timeout")
+            Log().error("timeout")
             sys.exit(1)
 
         return pots
 
 
-    def get_or_create_merchant(self, mo_merchant):
-        if 'metadata' in mo_merchant and 'website' in mo_merchant['metadata']:
-            website = mo_merchant['metadata']['website']
-        else:
-            website = None
-
-        merchant_id = mo_merchant['id']
-
-        mo_merchant['merchant_id'] = mo_merchant['id']
-        mo_merchant.pop('id')
-        mo_address = mo_merchant.pop('address')
-
-        merchant = Merchant().find_by_merchant_id(merchant_id)
-
-        if not merchant:
-            merchant = Merchant()
-
-        merchant.update(mo_merchant)
-        merchant.save()
-
-        mo_address['merchant_id'] = merchant.id
-
-        address = MerchantAddress().find_by_merchant_id(merchant.id)
-
-        if not address:
-            address = MerchantAddress()
-
-        address.update(mo_address)
-        address.save()
-
-        return merchant
-
-
-    def sanitise(self, string):
-        return re.sub('[\s\t]+', ' ', string)
-
-
-    def add_transaction(self, account, mo_transaction, pot_account_ids, pot_id=None):
-        counterparty = None
-
-        if mo_transaction.counterparty:
-            counterparty = self.get_or_create_counterparty(mo_transaction.counterparty)
-
-            if counterparty.name != mo_transaction.description:
-                description = self.sanitise('%s %s' % (counterparty.name, mo_transaction.description))
-            else:
-                description = mo_transaction.description
-        else:
-            description = self.sanitise(mo_transaction.description)
-
-        amount = mo_transaction.amount
-
-        if amount >0:
-            money_in = amount / 100
-            money_out = None
-            verb = 'from'
-            _type = 'credit'
-        else:
-            money_in = None
-            money_out = 0 - (amount / 100)
-            verb = 'to'
-            _type = 'debit'
-
-        if pot_id:
-            where = [{
-                'clause': 'pot_id = %s',
-                'params': [pot_id]
-            }]
-        else:
-            where = [{
-                'clause': 'pot_id is null'
-            }]
-
-        transaction = Transaction().find_by_account_id_and_transaction_id(
-            account.id,
-            mo_transaction.transaction_id,
-            where=where
-        )
-
-        if not transaction:
-            transaction = Transaction()
-
-        if pot_id is None and mo_transaction.metadata and 'pot_account_id' in mo_transaction.metadata and mo_transaction.metadata['pot_account_id'] not in pot_account_ids:
-            pot_account_ids[mo_transaction.metadata['pot_account_id']] = mo_transaction.metadata['pot_id']
-
-        if mo_transaction.merchant:
-            merchant = self.get_or_create_merchant(mo_transaction.merchant)
-        else:
-            merchant = None
-
-        transaction.update({
-            'account_id': account.id,
-            'transaction_id': mo_transaction.transaction_id,
-            'date': mo_transaction.created.strftime('%Y-%m-%d'),
-            'type': _type,
-            'description': description,
-            'ref': mo_transaction.description,
-            'money_in': money_in,
-            'money_out': money_out,
-            'pending': mo_transaction.amount_is_pending,
-            'created_at': mo_transaction.created,
-            'updated_at': mo_transaction.updated,
-            'currency': mo_transaction.currency,
-            'local_currency': mo_transaction.local_currency,
-            'local_amount': mo_transaction.local_amount,
-            'merchant_id': merchant.id if merchant else None,
-            'notes': mo_transaction.notes,
-            'originator': mo_transaction.originator,
-            'scheme': mo_transaction.scheme,
-            'settled': mo_transaction.settled,
-            'declined': 1 if len(mo_transaction.decline_reason) >0 else 0,
-            'decline_reason': mo_transaction.decline_reason,
-            'counterparty_id': counterparty.id if counterparty else None,
-            'pot_id': pot_id
-        })
-
-        transaction.save()
-
-        metadata = {}
-
-        if type(mo_transaction.atm_fees_detailed) == dict:
-            for key in mo_transaction.atm_fees_detailed:
-                metadata['atm_fees_detailed_%s' % (key)] = mo_transaction.atm_fees_detailed[key]
-
-        if type(mo_transaction.categories) == dict:
-            for key in mo_transaction.categories:
-                metadata['categories_%s' % (key)] = mo_transaction.categories[key]
-
-        if type(mo_transaction.fees) == dict:
-            for key in mo_transaction.fees:
-                metadata['fees_%s' % (key)] = mo_transaction.fees[key]
-
-        if type(mo_transaction.metadata) == dict:
-            for key in mo_transaction.metadata:
-                metadata['metadata_%s' % (key)] = mo_transaction.metadata[key]
-
-        for key in metadata:
-            transaction_metadata = TransactionMetadata().find_by_transaction_id_and_key(transaction.id, key)
-
-            if not transaction_metadata:
-                transaction_metadata = TransactionMetadata()
-                transaction_metadata.transaction_id = transaction.id
-                transaction_metadata.key = key
-
-            transaction_metadata.value = metadata[key]
-
-            transaction_metadata.save()
-
-        for transaction_metadata in TransactionMetadata().find_all_by_transaction_id(transaction.id):
-            if transaction_metadata.key not in metadata:
-                transaction_metadata.delete()
-
-        return transaction
-
-
-    def get_or_create_counterparty(self, mo_counterparty):
-        counterparty = Counterparty().find_by_user_id(mo_counterparty['user_id'])
-
-        if not counterparty:
-            counterparty = Counterparty()
-
-        counterparty.update(mo_counterparty)
-
-        counterparty.save()
-
-        return counterparty
-
-
-    def get_provider(self):
-        provider = Provider().find_by_name(PROVIDER)
-
-        if not provider:
-            provider = Provider()
-            provider.name = PROVIDER
-            provider.save()
-
-        return provider
-
-
-    def sync(self):
-        mo_accounts = self.accounts()
-
-        accounts = []
-
-        for mo_account in mo_accounts:
-            if 'monzoflexbackingloan' in mo_account.description:
-                continue
-
-            account = self.get_or_create_account(mo_account, self.config['accounts'][mo_account.account_id])
-
-            try:
-                mo_transactions = self.transactions(account.account_id)
-            except MonzoPermissionsError:
-                continue
-            except MonzoServerError:
-                continue
-
-            mo_pots = self.pots(account_id=account.account_id)
-
-            pot_lookup = {}
-
-            for mo_pot in mo_pots:
-                pot = Pot().find_by_account_id_and_pot_id(account.id, mo_pot.pot_id)
-
-                if not pot:
-                    pot = Pot()
-
-                pot.account_id = account.id
-                pot.pot_id = mo_pot.pot_id
-                pot.name = mo_pot.name
-                pot.balance = mo_pot.balance / 100
-                pot.deleted = mo_pot.deleted
-
-                pot.save()
-
-                pot_lookup[pot.pot_id] = pot.id
-
-            seen = {}
-
-            pot_account_ids = {}
-
-            for mo_transaction in mo_transactions:
-                transaction = self.add_transaction(account, mo_transaction, pot_account_ids)
-
-                seen[transaction.id] = 1
-
-            seen = {}
-
-            for pot_account_id in pot_account_ids:
-                mo_pot_transactions = self.transactions(pot_account_id)
-
-                for mo_pot_transaction in mo_pot_transactions:
-                    transaction = self.add_transaction(account, mo_pot_transaction, pot_account_ids, pot_lookup[pot_account_ids[pot_account_id]])
-
-                    seen[transaction.id] = 1
-
-        if 'touch_file' in self.config:
-            Path(self.config['touch_file']).touch()
-
-
-    def get_or_create_account(self, mo_account, account_config):
-        account = Account().find_by_provider_id_and_account_id(self.provider.id, mo_account.account_id)
-
-        if not account:
-            account = Account()
-
-        account.provider_id = self.provider.id
-        account.name = account_config['name']
-        account.account_id = mo_account.account_id
-
-        if 'sortcode' in account_config:
-            account.type = 'bank'
-            account.balance = account.available = mo_account.balance.balance / 100
-            account.sortcode = account_config['sortcode']
-            account.account_no = account_config['account_no']
-        else:
-            account.type = 'credit'
-            account.balance = 0 - (mo_account.balance.balance / 100)
-            account.available = account_config['credit_limit'] - account.balance
-            account.credit_limit = account_config['credit_limit']
-
-        account.save()
-
-        return account
-
-
-    def withdraw_credit(self, account_id, pot, credit):
-        if os.path.exists(self.token_file):
-            data = json.loads(open(self.token_file).read())
-
-            self.access_token = data['access_token']
-            self.access_token_expiry = data['expiry']
-            self.refresh_token = data['refresh_token']
-        else:
-            raise Exception("need to abstract the auth library")
+    def withdraw_from_pot(self, account_id, pot, credit):
+        self.load_tokens()
 
         self.client = self.get_client()
 
-        pot = monzo.endpoints.pot.Pot.fetch_single(self.client, account_id=account_id, pot_id=pot['pot_id'])
+        pot = monzo.endpoints.pot.Pot.fetch_single(self.client, account_id=account_id, pot_id=pot.pot_id)
 
         dedupe_code = '%s_%s' % (
             pot.pot_id,
             datetime.datetime.now().strftime('%Y%m%d%H')
         )
 
         amount = round(credit * 100)
 
         for i in range(0, 3):
             try:
                 monzo.endpoints.pot.Pot.withdraw(self.client, pot=pot, account_id=account_id, amount=amount, dedupe_id=dedupe_code)
-                self.sync()
                 return True
             except Exception as e:
                 print("failed to withdraw pot money: %s" % (str(e)))
 
                 if i <2:
                     time.sleep(3)
 
         return False
 
 
     def deposit_to_pot(self, account_id, pot, shortfall):
-        if os.path.exists(self.token_file):
-            data = json.loads(open(self.token_file).read())
-
-            self.access_token = data['access_token']
-            self.access_token_expiry = data['expiry']
-            self.refresh_token = data['refresh_token']
-        else:
-            raise Exception("need to abstract the auth library")
+        self.load_tokens()
 
         self.client = self.get_client()
 
-        pot = monzo.endpoints.pot.Pot.fetch_single(self.client, account_id=account_id, pot_id=pot['pot_id'])
+        pot = monzo.endpoints.pot.Pot.fetch_single(self.client, account_id=account_id, pot_id=pot.pot_id)
 
         dedupe_code = '%s_%s' % (
             pot.pot_id,
             datetime.datetime.now().strftime('%Y%m%d%H')
         )
 
         amount = round(shortfall * 100)
 
         for i in range(0, 3):
             try:
                 monzo.endpoints.pot.Pot.deposit(self.client, pot=pot, account_id=account_id, amount=amount, dedupe_id=dedupe_code)
-                self.sync()
                 return True
             except Exception as e:
-                print("failed to withdraw pot money: %s" % (str(e)))
+                print("failed to deposit pot money: %s" % (str(e)))
 
                 if i <2:
                     time.sleep(3)
 
         return False
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## monzo_utils/model/account.py

```diff
@@ -1,36 +1,37 @@
 import sys
 from monzo_utils.model.base import BaseModel
+from monzo_utils.model.pot import Pot
 from monzo_utils.lib.db import DB
 
 class Account(BaseModel):
 
     DISPLAY_KEYS = ['name','sortcode','account_no','balance','available']
 
 
-    def __init__(self, attrs={}):
-        super().__init__(attrs)
-
-
     def transactions(self, orderby='created_at', orderdir='asc', limit=None):
         return super().related('Transaction', 'account_id', self.id, orderby, orderdir, limit)
 
 
     def pots(self, orderby='name', orderdir='asc', limit=None):
-        return super().related('Pot', 'account_id', self.id, orderby, orderdir, limit, deleted=0)
+        return self.related('Pot', 'account_id', self.id, orderby, orderdir, limit, deleted=0)
+
+
+    def get_pot(self, name):
+        return Pot.one("select * from pot where account_id = %s and name = %s and deleted = %s", [self.id, name, 0])
 
 
     @property
     def __dict__(self):
-        attrs = {'attrs': self.attrs}
+        attributes = {'attributes': self.attributes}
 
         for pot in self.pots(orderby='name'):
-            attrs['attrs'][pot.name] = pot.balance
+            attributes['attributes'][pot.name] = pot.balance
 
-        return attrs
+        return attributes
 
 
     @property
     def keys(self):
         keys = []
 
         for key in self.DISPLAY_KEYS.copy():
@@ -43,21 +44,31 @@
         for pot in self.pots(orderby='name'):
             if pot.name not in keys:
                 keys.append(pot.name)
 
         return keys
 
 
-    def last_salary_transaction(self, description, payment_day, salary_minimum):
-        return DB().find_transaction_by_account_id_and_declined_and_description(
-            self.id,
-            0,
-            description,
-            orderby='created_at',
-            orderdir='desc',
-            limit=1,
-            search=['description'],
-            where=[{
-                'clause': 'money_in >= %s',
-                'params': [salary_minimum]
-            }]
-        )
+    def last_salary_transaction(self, description, salary_minimum, salary_payment_day):
+        if type(description) == list:
+            salary_desc = description
+        else:
+            salary_desc = [description]
+
+        where = f"account_id = %s and declined = %s and money_in >= %s and ("
+        params = [self.id, 0, salary_minimum]
+
+        for i in range(0, len(salary_desc)):
+            if i >0:
+                where += ' or '
+            where += " description like %s"
+            params.append('%' + salary_desc[i] + '%')
+
+        where += ")"
+
+        for row in DB().query(f"select * from transaction where {where} order by created_at desc", params):
+            day = row['date'].day
+
+            if row['date'].day >= salary_payment_day - 4 and row['date'].day <= salary_payment_day:
+                return row
+
+        return None
```

## monzo_utils/model/base.py

```diff
@@ -1,77 +1,96 @@
 import re
+import sys
 import json
 import importlib
+import datetime
+import decimal
 from monzo_utils.lib.db import DB
 
 class BaseModel:
 
-    def __init__(self, attrs=None):
-        self.table = re.sub(r'(?<!^)(?=[A-Z])', '_', type(self).__name__).lower()
+    @classmethod
+    def one(cls, sql, params):
+        row = DB().one(sql, params)
 
-        if attrs:
-            self.attrs = attrs
-        else:
-            self.attrs = {}
+        if row:
+            table = re.sub(r'(?<!^)(?=[A-Z])', '_', cls.__name__).lower()
 
-        if 'id' not in self.attrs:
-            self.attrs['id'] = None
+            return getattr(importlib.import_module(f"monzo_utils.model.{table}"), cls.__name__)(row)
 
+        return None
 
-    def __getattr__(self, name):
-        if name in self.attrs:
-            return self.attrs[name]
 
-        match = re.match('^find_by_(.*?)$', name)
+    @classmethod
+    def find(cls, sql, params):
+        table = re.sub(r'(?<!^)(?=[A-Z])', '_', cls.__name__).lower()
+
+        data = DB().query(sql, params)
 
-        if match:
-            method_name = f"find_{self.table}_by_{match.group(1)}"
+        results = []
 
-            def find_object_by_fields(*args, **kwargs):
-                record = getattr(DB(), method_name)(*args, **kwargs)
+        for row in data:
+            results.append(getattr(importlib.import_module(f"monzo_utils.model.{table}"), cls.__name__)(row))
 
-                if record:
-                    return type(self)(record)
+        return results
 
-                return record
 
-            return find_object_by_fields
+    def __init__(self, attributes=None):
+        self.attributes = {}
+        self.factory_query = False
+        self.table = re.sub(r'(?<!^)(?=[A-Z])', '_', self.__class__.__name__).lower()
 
-        match = re.match('^find_all_by_(.*?)$', name)
+        if type(attributes) == dict:
+            self.attributes = attributes
 
-        if match:
-            method_name = f"find_all_{self.table}_by_{match.group(1)}"
 
-            def find_objects_by_fields(*args, **kwargs):
-                objects = []
+    def __getattr__(self, name):
+        try:
+            return self.attributes[name]
+        except:
+            pass
 
-                for record in getattr(DB(), method_name)(*args, **kwargs):
-                    objects.append(type(self)(record))
+        if name == 'id':
+            return None
 
-                return objects
+        raise AttributeError(f"'{type(self).__name__}' object has no attribute '{name}'")
 
-            return find_objects_by_fields
 
-        print("DB class method missing: %s" % (name))
-        sys.exit(1)
+    def __bool__(self):
+        return 'id' in self.__dict__.get('attributes', {})
 
 
     def __setattr__(self, name, value):
-        if name not in ['table','attrs']:
-            self.attrs[name] = value
+        if name not in ['table','attributes','factory_query']:
+            self.attributes[name] = value
         else:
             super().__setattr__(name, value)
 
 
     def __delattr__(self, name):
-        self.attrs.pop(name)
+        try:
+            self.attributes.pop(name)
+        except KeyError:
+            pass
 
 
     def __str__(self):
-        return json.dumps(self.attrs,indent=4)
+        for_display = {}
+
+        for key in self.attributes:
+            if type(self.attributes[key]) == datetime.date:
+                for_display[key] = self.attributes[key].strftime('%Y-%m-%d')
+            elif type(self.attributes[key]) == datetime.datetime:
+                for_display[key] = self.attributes[key].strftime('%Y-%m-%d %H:%M:%S')
+            elif type(self.attributes[key]) == decimal.Decimal:
+                for_display[key] = float(self.attributes[key])
+            else:
+                for_display[key] = self.attributes[key]
+
+        return json.dumps(for_display,indent=4)
 
 
     def related(self, model, key_field, parent_id, orderby, orderdir, limit, deleted=None):
         table = model.lower()
 
         sql = f"select * from `{table}` where {key_field} = %s"
         params = [parent_id]
@@ -89,23 +108,103 @@
         related = []
         for row in DB().query(sql, params):
             related.append(getattr(importlib.import_module(f"monzo_utils.model.{table}"), model)(row))
 
         return related
 
 
-    def update(self, attrs):
-        self.attrs.update(attrs)
+    def update(self, attributes):
+        self.attributes.update(attributes)
 
 
     def save(self):
         if self.id:
-            DB().update(self.table, self.id, self.attrs)
+            DB().update(self.table, self.id, self.attributes)
         else:
-            self.id = DB().create(self.table, self.attrs)
+            self.id = DB().create(self.table, self.attributes.copy())
 
 
     def delete(self):
         if self.id is None:
             raise Exception("Unable to delete record with null id")
 
         DB().query(f"delete from {self.table} where id = %s", [self.id])
+
+
+    def factory(self):
+        if self.factory_query is False:
+            DB().find(self.table)
+            self.factory_query = True
+
+
+    def select(self, select):
+        self.factory()
+
+        DB().select(select)
+
+        return self
+
+
+    def join(self, join_table):
+        if join_table not in self.RELATIONSHIPS:
+            raise Exception(f"no relationship defined between {self.table} and {join_table}")
+
+        self.factory()
+
+        DB().join(join_table, self.RELATIONSHIPS[join_table][0], self.RELATIONSHIPS[join_table][1])
+
+        return self
+
+
+    def leftJoin(self, join_table, where=None):
+        if join_table not in self.RELATIONSHIPS:
+            raise Exception(f"no relationship defined between {self.table} and {join_table}")
+
+        self.factory()
+
+        DB().leftJoin(join_table, self.RELATIONSHIPS[join_table][0], self.RELATIONSHIPS[join_table][1], where)
+
+        return self
+
+
+    def where(self, clause, params):
+        self.factory()
+
+        DB().where(clause, params)
+
+        return self
+
+
+    def andWhere(self, clause, params):
+        self.factory()
+
+        DB().andWhere(clause, params)
+
+        return self
+
+
+    def groupBy(self, group_by):
+        self.factory()
+
+        DB().groupBy(group_by)
+
+        return self
+
+
+    def orderBy(self, orderby, orderdir):
+        self.factory()
+
+        DB().orderBy(orderby, orderdir)
+
+        return self
+
+
+    def getall(self):
+        self.factory()
+
+        return DB().getall()        
+
+
+    def getone(self):
+        self.factory()
+
+        return DB().getone()
```

## monzo_utils/model/transaction.py

```diff
@@ -1,5 +1,10 @@
 from monzo_utils.model.base import BaseModel
 
 class Transaction(BaseModel):
 
     DISPLAY_KEYS = ['date','type','money_in','money_out','pending','description']
+    RELATIONSHIPS = {
+        'account': ['`transaction`.account_id', 'account.id'],
+        'transaction_metadata': ['`transaction`.id', 'transaction_metadata.transaction_id'],
+        'pot': ['`transaction`.pot_id', 'pot.id']
+    }
```

## Comparing `monzo_utils-0.0.9.data/scripts/monzo-payments` & `monzo_utils/lib/monzo_payments.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,769 +1,765 @@
-#!python
+#!/usr/bin/env python3
 
 import os
 import sys
 import datetime
 import yaml
 import calendar
 import json
 import time
 import requests
 import math
 import pwd
+import importlib
+import decimal
 from pushover import Client
-from monzo_utils.lib.monzo_api import Monzo
+from monzo_utils.lib.monzo_api import MonzoAPI
+from monzo_utils.lib.config import Config
 from monzo_utils.lib.db import DB
+from monzo_utils.lib.monzo_sync import MonzoSync
 from monzo_utils.model.provider import Provider
 from monzo_utils.model.account import Account
 from monzo_utils.model.pot import Pot
 from monzo_utils.model.transaction import Transaction
+from monzo_utils.model.flex_summary import FlexSummary
+from govuk_bank_holidays.bank_holidays import BankHolidays
+from calendar import monthrange
 
 PROVIDER = 'Monzo'
 
-class PaymentFundsCheck:
-    def __init__(self, account_name):
+class MonzoPayments:
+
+    def __init__(self, account_name, output_json=False, abbreviate=False):
         self.account_name = account_name
+        self.json = output_json
+        self.abbreviate = abbreviate
+        self.output = []
+        self.due = 0
+        self.total_this_month = 0
+        self.next_month = 0
+        self.next_month_bills_pot = 0
+
+        self.config = self.load_config()
+        self.validate_config()
+
+        self.db = self.get_db()
+
+        self.seen = []
+        self.exchange_rates = {}
+
+        self.provider = Provider.one("select * from provider where name = %s", [PROVIDER])
+        self.account = Account.one("select * from account where provider_id = %s and name = %s", [self.provider.id, self.account_name])
+
+        if not self.account:
+            sys.stderr.write(f"account {self.account_name} not found in the database\n")
+            sys.exit(1)
 
         homedir = pwd.getpwuid(os.getuid()).pw_dir
-        monzo_dir = f"{homedir}/.monzo"
+        self.credit_tracker = f"{homedir}/.monzo/{self.config['account']}.credit"
+        self.shortfall_tracker = f"{homedir}/.monzo/{self.config['account']}.shortfall"
+
+
+    def get_db(self):
+        try:
+            db = DB(None, self.config_path)
+        except Exception as e:
+            print(f"failed to connect to the database: {str(e)}")
+            sys.exit(1)
 
-        if not os.path.exists(monzo_dir):
-            os.mkdir(monzo_dir, 0o755)
+        return db
 
-        config_file = f"{monzo_dir}/config.yaml"
 
-        self.monzo_config = yaml.safe_load(open(config_file).read())
+    def load_config(self):
+        if os.path.exists(self.account_name):
+            account_config_file = self.account_name
+            self.config_path = os.path.dirname(account_config_file)
+        else:
+            homedir = pwd.getpwuid(os.getuid()).pw_dir
 
-        account_config_file = f"{monzo_dir}/{account_name}.yaml"
+            self.config_path = f"{homedir}/.monzo"
+
+            if not os.path.exists(self.config_path):
+                if not os.path.exists(self.config_path):
+                    os.mkdir(self.config_path, 0o755)
+
+            account_config_file = f"{self.config_path}/{self.account_name}.yaml"
 
         if not os.path.exists(account_config_file):
             sys.stderr.write(f"Cannot find account config file: {account_config_file}\n")
             sys.exit(1)
 
         try:
-            self.config = yaml.safe_load(open(account_config_file).read())
+            config = yaml.safe_load(open(account_config_file).read())
         except Exception as e:
             sys.stderr.write(f"Cannot read or parse account config file {account_config_file}: {str(e)}\n")
             sys.exit(1)
 
+        self.account_name = config['account']
+
+        return config
+
+
+    def validate_config(self):
         for required in ['payments','salary_description','salary_payment_day']:
             if required not in self.config or not self.config[required]:
                 sys.stderr.write(f"Missing config key: {required}\n")
                 sys.exit(1)
 
         if ('notify_shortfall' in self.config and self.config['notify_shortfall']) or ('notify_credit' in self.config and self.config['notify_credit']):
             for required in ['pushover_key','pushover_app']:
                 if required not in self.config or not self.config[required]:
                     sys.stderr.write(f"Push is enabled but push config key is missing: {required}\n")
                     sys.exit(1)
 
-        self.db = DB(self.monzo_config['db'])
 
-        self.seen = []
-        self.exchange_rates = {}
+    def main(self):
+        self.last_salary_date = self.get_last_salary_date()
+        self.next_salary_date = self.get_next_salary_date(self.last_salary_date)
+        self.following_salary_date = self.get_next_salary_date(self.next_salary_date)
+
+        if self.json is False:
+            self.widths = {
+                'Status': 9,
+                'Type': 15,
+                'Name': 25,
+                'Count': 5,
+                'Amount': 19,
+                'Left': 8,
+                'Last date': 12,
+                'Due date': 10
+            }
+            self.fields = ['Status','Type','Name','Count','Amount','Left','Last date','Due date']
+
+        payment_lists = {
+            'yearly': [],
+            'monthly': []
+        }
+
+        if 'payments' in self.config:
+            for payment_list in self.config['payments']:
+                if not payment_list['payments']:
+                    continue
 
-        self.provider = Provider().find_by_name(PROVIDER)
-        self.account = Account().find_by_provider_id_and_name(self.provider.id, self.account_name)
+                due, total_due_this_month, total_due_next_month, payments = self.process_payment_list(payment_list, True)
 
-        if not self.account:
-            sys.stderr.write(f"account {self.account_name} not found in the database\n")
-            sys.exit(1)
+                payment_lists['yearly'] += payments
 
+                self.due += due
+                self.total_this_month += total_due_this_month
+                self.next_month += total_due_next_month
 
-    def main(self):
-        last_salary_date = self.get_last_salary_date()
-        next_salary_date = self.get_next_salary_date(last_salary_date)
+            for payment_list in self.config['payments']:
+                if not payment_list['payments']:
+                    continue
 
-        due = 0
-        total = 0
-        next_month = 0
-        next_month_bills_pot = 0
+                due, total_due_this_month, total_due_next_month, payments = self.process_payment_list(payment_list, False)
 
-        now = datetime.datetime.now()
+                payment_lists['monthly'] += payments
 
-        flex_payments = []
+                self.due += due
+                self.total_this_month += total_due_this_month
+                self.next_month += total_due_next_month
+
+        if 'refunds_due' in self.config and self.config['refunds_due']:
+            self.display_payment_list({
+                'type': 'Refund',
+                'payments': self.config['refunds_due']
+            }, False)
 
-        for payment_list in self.config['payments']:
-            if payment_list['type'] == 'Flex':
-                flex_payments += payment_list['payments']
-                continue
+        if 'pot' in self.config:
+            pot = self.account.get_pot(self.config['pot'])
+        else:
+            pot = self.account
 
-            if not payment_list['payments']:
-                continue
+        shortfall = (self.due - (round(pot.balance * 100))) / 100
 
-            for payment in payment_list['payments']:
-                if payment_list['type'] == 'Amazon Payments':
-                    status, num_paid, remaining, last_amount, last_date, due_date = self.get_amazon_payment(payment, last_salary_date, next_salary_date, payment_list['payment_day'])
-
-                    self.display(status, 'Amazon Payments', payment['name'], last_amount, last_date, due_date, num_paid, payment['months'], remaining)
-
-                    if status == 'DUE':
-                        if last_amount >= remaining:
-                            due += last_amount * 100
-                            total += last_amount * 100
-                        else:
-                            due += remaining * 100
-                            total += remaining * 100
-
-                    elif status == 'PAID':
-                        total += last_amount * 100
-
-                    if remaining == 0:
-                        due_next_month = 0
-                    elif last_amount >= remaining:
-                        due_next_month = remaining
-                    else:
-                        due_next_month = last_amount
+        if self.json:
+            data = {
+                'balance': float(pot.balance),
+                'due': float(self.due) / 100,
+                'total_this_month': self.total_this_month / 100,
+                'total_next_month': self.next_month / 100,
+                'payments': self.sanitise(self.output)
+            }
+
+            if shortfall * 100 <0:
+                data['credit'] = (round(pot.balance * 100) - self.due) / 100
+                data['shortfall'] = 0
+            else:
+                data['shortfall'] = shortfall
+                data['credit'] = 0
 
-                    next_month_bills_pot += due_next_month * 100
-                    continue
+            print(json.dumps(data,indent=4))
+            return
 
-                last_date, last_amount = self.get_last_payment_date(payment_list['type'], payment)
+        self.adjust_column_widths(payment_lists)
 
-                if 'fixed' in payment and payment['fixed']:
-                    last_amount = payment['amount']
+        self.display_columns('yearly')
+        self.display_table(payment_lists['yearly'])
 
-                if str(payment['amount'])[0] == '$':
-                    rate = self.get_exchange_rate('usd')
+        self.display_spacer('monthly')
+        self.display_table(payment_lists['monthly'])
 
-                    dollar_value = float(str(payment['amount'])[1:])
+        sys.stdout.write("\n")
 
-                    last_amount = dollar_value / rate
+        indent = self.widths['Status'] + self.widths['Type'] + 2
+        width = self.widths['Name'] + self.widths['Count'] + 2
 
-                if last_amount is None:
-                    last_amount = payment['amount']
+        sys.stdout.write(" " * indent)
 
-                if 'last_amount_overrides' in self.config and payment['name'] in self.config['last_amount_overrides'] and last_salary_date in self.config['last_amount_overrides'][payment['name']]:
-                    last_amount = self.config['last_amount_overrides'][payment['name']][last_salary_date]
+        sys.stdout.write("TOTAL THIS MONTH:".ljust(width))
+        print("£%.2f" % (self.total_this_month / 100))
 
-                if 'last_date_overrides' in self.config and payment['name'] in self.config['last_date_overrides'] and last_date in self.config['last_date_overrides'][payment['name']]:
-                    last_date = self.config['last_date_overrides'][payment['name']][last_date]
+        if 'exclude_yearly_from_bills' in self.config and self.config['exclude_yearly_from_bills']:
+            sys.stdout.write("\n")
 
-                could_be_due = True
+        sys.stdout.write(" " * indent)
+        sys.stdout.write("TOTAL NEXT MONTH:".ljust(width))
+        print("£%.2f" % (self.next_month / 100))
+
+        credit = (round(pot.balance * 100) - self.due) / 100
+
+        if round(shortfall * 100) <0:
+            sys.stdout.write(" " * indent)
+            sys.stdout.write("LESS CREDIT BALANCE:".ljust(width))
+            print("£%.2f" % ((self.next_month / 100) - credit))
 
-                due_date = last_date
+        if 'exclude_yearly_from_bills' in self.config and self.config['exclude_yearly_from_bills']:
+            sys.stdout.write(" " * indent)
+            sys.stdout.write("Bills pot payment:".ljust(width))
+            print("£%.2f" % (self.next_month_bills_pot / 100))
 
-                if 'yearly_month' in payment:
-                    could_be_due = self.is_yearly_payment_due_this_month(payment, last_salary_date)
+        sync_required = False
 
-                    today = datetime.datetime.now()
+        if round(shortfall * 100) >0:
+            print("      due: £%.2f" % (self.due / 100))
+            print("  balance: £%.2f" % (pot.balance))
+            print("shortfall: £%.2f" % (shortfall))
 
-                    while today.month != payment['yearly_month'] or today.day != payment['yearly_day']:
-                        today += datetime.timedelta(days=1)
+            sync_required = self.handle_shortfall(pot, shortfall)
 
-                    due_date = datetime.date(today.year, today.month, today.day)
+        else:
 
-                else:
-                    if 'renew_date' in payment:
-                        due_date = payment['renew_date']
-                    elif due_date:
-                        if due_date.month == 12:
-                            due_date = datetime.date(due_date.year+1, 1, due_date.day)
-                        else:
-                            due_date = datetime.date(due_date.year, due_date.month+1, due_date.day)
-
-                # payment period not started yet
-                if 'start_date' in payment:
-                    if payment['start_date'] >= next_salary_date:
-                        could_be_due = False
-                        due_date = payment['start_date']
-
-                # excluded months (council tax)
-                if 'exclude_months' in payment:
-                    if last_date is None:
-                        if 'start_date' in payment:
-                            next_payment_month = payment['start_date'].month + 1
-                        else:
-                            next_payment_month = None
-                    else:
-                        next_payment_month = last_date.month + 1
+            if os.path.exists(self.shortfall_tracker):
+                os.remove(self.shortfall_tracker)
 
-                    if next_payment_month:
-                        if next_payment_month >12:
-                            next_payment_month = 1
-
-                        if next_payment_month in payment['exclude_months']:
-                            could_be_due = False
-
-                if could_be_due and (last_date is None or last_date < last_salary_date):
-                    status = 'DUE'
-                    due += round(last_amount * 100)
-                    total += round(last_amount * 100)
-                else:
-                    if could_be_due:
-                        status = 'PAID'
-                        total += round(last_amount * 100)
-                    else:
-                        status = 'SKIPPED'
+            print("    due: £%.2f" % (self.due / 100))
+            print("balance: £%.2f" % (pot.balance))
 
-                num_paid = None
-                num_total = None
-                remaining = None
+            if round(credit * 100) == 0:
+                credit = 0
 
-                if payment_list['type'] == 'Finance':
-                    if 'months' not in payment:
-                        raise Exception('finance entries must have key: months')
-                    if 'start_date' not in payment:
-                        raise Exception('finance entries must have key: start_date')
+                if os.path.exists(self.credit_tracker):
+                    os.remove(self.credit_tracker)
 
-                    num_paid = self.get_num_payments_made(payment)
-                    num_total = payment['months']
+            else:
+                print(" credit: £%.2f" % (credit))
 
-                    total_paid = num_paid * payment['amount']
-                    remaining = (num_total - num_paid) * payment['amount']
+                sync_required = self.handle_credit(pot, credit)
 
-                self.display(status, payment_list['type'], payment['name'], last_amount, last_date, due_date, num_paid, num_total, remaining)
+        today = datetime.datetime.now()
 
-                # determine if due next month
-                if 'yearly_month' in payment:
-                    date_from = next_salary_date
-                    date_to = self.get_next_salary_date(next_salary_date)
+        if today.strftime('%Y%m%d') == self.last_salary_date.strftime('%Y%m%d'):
+            if self.check_pot_payments():
+                sync_required = True
+
+        if sync_required:
+            ms = MonzoSync()
+            ms.sync(3, self.account)
 
-                    if due_date >= date_from and due_date <= date_to:
-                        next_month += round(last_amount * 100)
 
-                        if 'exclude_yearly_from_bills' not in self.config or self.config['exclude_yearly_from_bills'] is False:
-                            next_month_bills_pot += round(last_amount * 100)
-                else:
-                    end_of_next_salary_period = self.get_next_salary_date(next_salary_date)
+    def display_columns(self, title):
+        for i in range(0, len(self.fields)):
+            if i > 0:
+                sys.stdout.write(" ")
+            if self.fields[i] == 'Count':
+                sys.stdout.write(''.ljust(self.widths[self.fields[i]]))
+            else:
+                sys.stdout.write(self.fields[i].ljust(self.widths[self.fields[i]]))
 
-                    if 'start_date' not in payment or payment['start_date'] < end_of_next_salary_period:
-                        if 'renew_date' not in payment or payment['renew_date'] < end_of_next_salary_period:
-                            next_month += round(last_amount * 100)
-
-                            if 'exclude_from_bills' not in self.config or ('exclude_from_bills' in self.config and payment['name'] not in self.config['exclude_from_bills']):
-                                next_month_bills_pot += round(last_amount * 100)
-
-        flex_this_month = 0
-        flex_due = []
-        flex_status = 'DONE'
-
-        total_remaining = 0
-
-        for payment in flex_payments:
-            status, date, amount, payment_num = self.flex_payment_due(payment, next_salary_date)
-
-            if status == 'DUE':
-                due += round(amount * 100)
-                total += round(amount * 100)
-                flex_this_month += amount
-                remaining = max([0, payment['amount'] - (payment_num * amount)])
-                total_remaining += remaining
-
-                flex_due.append({
-                    'status': status,
-                    'date': date,
-                    'amount': amount,
-                    'name': payment['name'],
-                    'num_paid': payment_num,
-                    'num_total': payment['months'],
-                    'remaining': remaining
-                })
-
-                next_month_bills_pot += round(amount * 100)
-                next_month += round(amount * 100)
-
-                if flex_status in ['DONE','SKIPPED']:
-                    flex_status = status
-
-            elif status == 'SKIPPED':
-                flex_this_month += amount
-                remaining = max([0, payment['amount'] - (payment_num * amount)])
-                total_remaining += remaining
-
-                flex_due.append({
-                    'status': status,
-                    'date': date,
-                    'amount': amount,
-                    'name': payment['name'],
-                    'num_paid': payment_num,
-                    'num_total': payment['months'],
-                    'remaining': remaining
-                })
-                next_month_bills_pot += round(amount * 100)
-                next_month += round(amount * 100)
-
-                if flex_status in ['DONE']:
-                    flex_status = status
-
-        if flex_status != 'DONE':
-            self.display(flex_status, 'Flex', 'Flex payment', flex_this_month, None, date, None, None, total_remaining)
-
-            for flex_payment in flex_due:
-                self.display(
-                    flex_payment['status'],
-                    'Flex',
-                    '- ' + flex_payment['name'],
-                    flex_payment['amount'],
-                    None,
-                    flex_payment['date'],
-                    flex_payment['num_paid'],
-                    flex_payment['num_total'],
-                    flex_payment['remaining']
-                )
+        sys.stdout.write("\n")
 
-        if 'pot' in self.config:
-            pot = Pot().find_by_account_id_and_name(self.account.id, self.config['pot'])
-        else:
-            pot = self.account
+        if self.json is False:
+            self.display_spacer(title)
 
-        shortfall = (due - (round(pot.balance * 100))) / 100
 
-        sys.stdout.write("\n")
+    def display_spacer(self, title):
+        sys.stdout.write("-" * (sum(self.widths.values()) - 2))
+        sys.stdout.write(title.ljust(9,'-') + "\n")
 
-        sys.stdout.write(" " * 25)
-        sys.stdout.write(" TOTAL THIS MONTH:".ljust(31))
-        print("£%.2f" % (total / 100))
 
-        if 'exclude_yearly_from_bills' in self.config and self.config['exclude_yearly_from_bills']:
-            sys.stdout.write("\n")
+    def prompt_action(self, prompt):
+        while 1:
+            sys.stdout.write(prompt)
+            sys.stdout.flush()
 
-        sys.stdout.write(" " * 25)
-        sys.stdout.write(" TOTAL NEXT MONTH:".ljust(31))
-        print("£%.2f" % (next_month / 100))
+            i = sys.stdin.readline().rstrip().lower()
 
-        if 'exclude_yearly_from_bills' in self.config and self.config['exclude_yearly_from_bills']:
-            sys.stdout.write(" " * 25)
-            sys.stdout.write("Bills pot payment:".ljust(31))
-            print("£%.2f" % (next_month_bills_pot / 100))
+            if i in ['y','n']:
+                break
 
-        if round(shortfall * 100) >0:
-            print("      due: £%.2f" % (due / 100))
-            print("  balance: £%.2f" % (pot.balance))
-            print("shortfall: £%.2f" % (shortfall))
+        return i == 'y'
 
-            if 'pot' in self.config:
-                deposit = False
-                notify = False
-
-                if 'pot' in self.config and 'auto_deposit' in self.config and self.config['auto_deposit']:
-                    deposit = True
-                elif not sys.stdout.isatty():
-                    if 'notify_shortfall' in self.config and self.config['notify_shortfall']:
-                        notify = True
-                else:
-                    if 'pot' in self.config and 'prompt_deposit' in self.config and self.config['prompt_deposit']:
-                        while 1:
-                            sys.stdout.write("\ndeposit shortfall? [y/N] ")
-                            sys.stdout.flush()
-
-                            i = sys.stdin.readline().rstrip().lower()
-
-                            if i in ['y','n']:
-                                break
-
-                        deposit = (i == 'y')
-                    elif 'notify_shortfall' in self.config and self.config['notify_shortfall']:
-                        notify = True
-
-                if deposit:
-                    m = Monzo()
-
-                    result = m.deposit_to_pot(self.account.account_id, pot, shortfall)
-
-                    if 'notify_deposit' in self.config and self.config['notify_deposit']:
-                        self.notify(
-                            '%s - pot topped up' % (self.account.name),
-                            "£%.2f\n£%.2f due, £%.2f available" % (
-                                shortfall,
-                                due / 100,
-                                pot.balance
-                            )
-                        )
  
-                elif notify:
-                    self.notify(
-                        '%s - shortfall' % (self.account.name),
-                        "£%.2f\n£%.2f due, £%.2f available" % (
-                            shortfall,
-                            due / 100,
-                            pot.balance
-                        )
-                    )
+    def process_payment_list(self, payment_list, annual):
+        payments = self.get_payments(payment_list, annual)
 
-        else:
-            credit = (round(pot.balance * 100) - due) / 100
+        summary = None
+        due = 0
+        total_due_this_month = 0
+        total_due_next_month = 0
 
-            print("    due: £%.2f" % (due / 100))
-            print("balance: £%.2f" % (pot.balance))
+        output = []
 
-            if round(credit * 100) == 0:
-                credit = 0
+        if payment_list['type'] == 'Flex' and annual is False:
+            total_this_month = 0
+            total_next_month = 0
+            today = datetime.datetime.now()
+            today = datetime.date(today.year, today.month, today.day)
+
+            for payment in payments:
+                total_this_month += payment.amount_for_period(self.last_salary_date, self.next_salary_date)
+                total_next_month += payment.amount_for_period(self.next_salary_date, self.following_salary_date)
+
+            flex_remaining = 0
+
+            for payment in payments:
+                flex_remaining += payment.remaining
+
+            summary = FlexSummary(self.config, self.account, total_this_month, total_next_month, flex_remaining, self.last_salary_date, self.next_salary_date, self.following_salary_date)
+
+            if self.json:
+                self.output.append(summary.data(self.abbreviate))
             else:
-                print(" credit: £%.2f" % (credit))
+                output.append(summary.display_output())
 
-                withdraw = False
-                notify = False
+        for payment in payments:
+            if summary:
+                payment.last_flex_payment = summary.last_payment
 
-                if 'pot' in self.config and 'auto_withdraw' in self.config and self.config['auto_withdraw']:
-                    withdraw = True
-                elif not sys.stdout.isatty():
-                    if 'notify_credit' in self.config and self.config['notify_credit']:
-                        notify = True
-                else:
-                    if 'pot' in self.config and 'prompt_withdraw' in self.config and self.config['prompt_withdraw']:
-                        while 1:
-                            sys.stdout.write("\nwithdraw credit? [y/N] ")
-                            sys.stdout.flush()
-
-                            i = sys.stdin.readline().rstrip().lower()
-
-                            if i in ['y','n']:
-                                break
-
-                        withdraw = (i == 'y')
-                    elif 'notify_credit' in self.config and self.config['notify_credit']:
-                        notify = True
-
-                if withdraw:
-                    m = Monzo()
-
-                    if not m.withdraw_credit(self.account.account_id, pot, credit):
-                        sys.stderr.write("ERROR: failed to withdraw credit\n")
-
-                    if 'notify_withdraw' in self.config and self.config['notify_withdraw']:
-                        self.notify(
-                            '%s - pot credit withdrawn' % (self.account.name),
-                            "£%.2f\n£%.2f due, £%.2f available" % (
-                                credit,
-                                due / 100,
-                                pot.balance
-                            )
-                        )
- 
-                elif notify:
-                    self.notify(
-                        '%s - credit' % (self.account.name),
-                        "£%.2f\n£%.2f due, £%.2f available" % (
-                            credit,
-                            due / 100,
-                            pot.balance
-                        )
-                    )
+            if payment.status in ['DUE','PAID']:
+                total_due_this_month += payment.display_amount * 100
 
+            if payment.status == 'DUE':
+                due += payment.display_amount * 100
 
-    def display(self, status, payment_type, payment_name, amount, last_date, due_date, num_paid=None, num_total=None, remaining=None):
-        if num_paid is not None:
-            suffix = '%d/%d' % (
-                num_paid,
-                num_total
-            )
-        else:
-            suffix = ''
+            if payment.due_next_month:
+                if payment.status == 'SKIPPED' or payment_list['type'] != 'Refund':
+                    total_due_next_month += payment.next_month_amount * 100
 
-        if remaining is not None:
-            remaining = '£%.2f' % (remaining)
-        else:
-            remaining = ''
+                    if 'exclude_yearly_from_bills' not in self.config or self.config['exclude_yearly_from_bills'] is False or 'yearly_month' not in payment_config:
+                        self.next_month_bills_pot += payment.next_month_amount * 100
 
-        print("%s: %s %s %s %s %s %s %s" % (
-            status.rjust(7),
-            payment_type.ljust(15),
-            payment_name.ljust(25),
-            suffix.ljust(4),
-            ('£%.2f' % (amount)).ljust(8),
-            remaining.ljust(8),
-            last_date.strftime('%Y-%m-%d').ljust(12) if last_date else ''.ljust(12),
-            due_date.strftime('%Y-%m-%d').ljust(10) if due_date else ''
-        ))
+            if self.json:
+                self.output.append(payment.data(self.abbreviate))
+            else:
+                output.append(payment.display_output())
 
+        return due, total_due_this_month, total_due_next_month, output
 
-    def flex_payment_due(self, payment, next_salary_date):
-        date = payment['start_date']
-        today = datetime.datetime.now()
-        today = datetime.date(today.year, today.month, today.day)
 
-        due = False
-        total_paid = 0
-        for i in range(0, payment['months']):
-            amount = int(math.ceil(payment['amount'] / payment['months']))
-
-            if total_paid + amount > payment['amount']:
-                amount = payment['amount'] - total_paid
-
-            while date.day != self.config['flex_payment_date']:
-                date += datetime.timedelta(days=1)
-
-            if date >= today:
-                due = True
-                payment_num = i
-                break
+    def get_payments(self, payment_list, annual):
+        payments = {}
 
-            date += datetime.timedelta(days=1)
+        for payment_config in payment_list['payments']:
+            payment_list_type_library = payment_list['type'].lower().replace(' ','_')
+            payment_list_type = payment_list['type'].title().replace(' ','')
 
-            total_paid += amount
+            if annual and ('is_yearly' not in payment_config or payment_config['is_yearly'] is False) and ('yearly_month' not in payment_config or 'yearly_day' not in payment_config):
+                continue
 
-        if not due:
-            status = 'DONE'
-        elif date <= next_salary_date:
-            status = 'DUE'
-        else:
-            status = 'SKIPPED'
+            if not annual and (('yearly_month' in payment_config and 'yearly_day' in payment_config) or ('is_yearly' in payment_config and payment_config['is_yearly'])):
+                continue
+
+            payment = getattr(importlib.import_module(f"monzo_utils.model.{payment_list_type_library}"), payment_list_type)(
+                self.config,
+                self.account,
+                payment_list,
+                payment_config,
+                self.last_salary_date,
+                self.next_salary_date,
+                self.following_salary_date
+            )
+
+            if payment.due_date not in payments:
+                payments[payment.due_date] = []
+
+            payments[payment.due_date].append(payment)
 
-        return status, date, amount, payment_num
+        sorted_payments = []
+
+        if None in payments:
+            for payment in payments[None]:
+                sorted_payments.append(payment)
+
+            payments.pop(None)
+
+        for due_date in sorted(payments):
+            for payment in payments[due_date]:
+                sorted_payments.append(payment)
+
+        return sorted_payments
 
 
     def notify(self, event, message):
         pushover = Client(self.config['pushover_key'], api_token=self.config['pushover_app'])
         pushover.send_message(message, title=event)
 
 
+    def abbreviate_string(self, string):
+        abbreviated = ''
+        
+        for i in range(0, len(string)):
+            if string[i].isupper():
+                abbreviated += string[i]
+
+        return abbreviated
+
+
     def get_last_salary_date(self):
         if 'salary_account' in self.config and self.config['salary_account'] != self.account_name:
-            account = Account().find_by_provider_id_and_name(self.provider.id, self.config['salary_account'])
+            account = Account.one("select * from account where provider_id = %s and name = %s", [self.provider.id, self.config['salary_account']])
         else:
             account = self.account
 
         last_salary_transaction = account.last_salary_transaction(
             description=self.config['salary_description'],
-            payment_day=self.config['salary_payment_day'],
-            salary_minimum=self.config['salary_minimum'] if 'salary_minimum' in self.config else 1000
+            salary_minimum=self.config['salary_minimum'] if 'salary_minimum' in self.config else 1000,
+            salary_payment_day=self.config['salary_payment_day']
         )
 
         if not last_salary_transaction:
             sys.stderr.write("failed to find last salary transaction.\n")
-            sys.stderr.write(f"SQL: {sql}\n")
-            sys.stderr.write(f"params: {json.dumps(params,indent=4)}\n")
             sys.exit(1)
 
         last_salary_date = last_salary_transaction['date']
 
-        while last_salary_date.day <self.config['salary_payment_day']:
-            last_salary_date = datetime.date(last_salary_date.year, last_salary_date.month, last_salary_date.day+1)
-
         return last_salary_date
 
 
     def get_next_salary_date(self, last_salary_date):
+        while last_salary_date.day != self.config['salary_payment_day']:
+            try:
+                last_salary_date = datetime.date(last_salary_date.year, last_salary_date.month, last_salary_date.day+1)
+            except:
+                last_salary_date = datetime.date(last_salary_date.year, last_salary_date.month+1, 1)
+
         next_salary_date = datetime.date(last_salary_date.year, last_salary_date.month, last_salary_date.day+1)
 
-        while next_salary_date.day != 15:
+        while next_salary_date.day != self.config['salary_payment_day']:
             try:
                 next_salary_date = datetime.date(next_salary_date.year, next_salary_date.month, next_salary_date.day+1)
             except:
-                next_salary_date = datetime.date(next_salary_date.year, next_salary_date.month+1, 1)
+                if next_salary_date.month == 12:
+                    next_salary_date = datetime.date(next_salary_date.year+1, 1, 1)
+                else:
+                    next_salary_date = datetime.date(next_salary_date.year, next_salary_date.month+1, 1)
 
         while next_salary_date.weekday() in [5,6]:
-            next_salary_date = datetime.date(next_salary_date.year, next_salary_date.month, next_salary_date.day-1)
+            if next_salary_date.day == 1:
+                if next_salary_date.month == 1:
+                    next_salary_date = datetime.date(next_salary_date.year-1, 12, 31)
+                else:
+                    next_salary_date = datetime.date(next_salary_date.year, next_salary_date.month-1, monthrange(next_salary_date.year, next_salary_date.month-1)[1])
+            else:
+                next_salary_date = datetime.date(next_salary_date.year, next_salary_date.month, next_salary_date.day-1)
+
+        if 'uk_bank_holidays' in self.config and self.config['uk_bank_holidays']:
+            bank_holidays = BankHolidays()
+
+            while bank_holidays.is_holiday(next_salary_date) or next_salary_date == datetime.date(2024,4,1) or next_salary_date.weekday() in [5,6]:
+                if next_salary_date.day == 1:
+                    if next_salary_date.month == 1:
+                        next_salary_date = datetime.date(next_salary_date.year-1, 12, 31)
+                    else:
+                        next_salary_date = datetime.date(next_salary_date.year, next_salary_date.month-1, monthrange(next_salary_date.year, next_salary_date.month-1)[1])
+                else:
+                    next_salary_date = datetime.date(next_salary_date.year, next_salary_date.month, next_salary_date.day-1)
 
         return next_salary_date
 
 
-    def get_last_payment_date(self, payment_type, payment):
-        if payment_type != 'Standing Order' and 'fixed' in payment and payment['fixed']:
-            transactions = Transaction().find_all_by_declined_and_money_out_and_description(
-                0,
-                payment['amount'],
-                payment['desc'],
-                orderby='created_at',
-                orderdir='desc',
-                search=['description']
-            )
+    def handle_shortfall(self, pot, shortfall):
+        deposit = False
+        notify = False
+
+        if 'pot' in self.config and 'auto_deposit' in self.config and self.config['auto_deposit'] and not sys.stdout.isatty() and not self.abbreviate:
+            if 'auto_deposit_delay_mins' in self.config:
+                deposit = self.handle_deposit_delay(shortfall)
+            else:
+                deposit = True
 
+        elif not sys.stdout.isatty():
+            if 'notify_shortfall' in self.config and self.config['notify_shortfall'] and not self.abbreviate:
+                notify = True
         else:
-            transactions = Transaction().find_all_by_declined_and_description(
-                0,
-                payment['desc'],
-                orderby='created_at',
-                orderdir='desc',
-                search=['description']
+            if 'pot' in self.config and 'prompt_deposit' in self.config and self.config['prompt_deposit']:
+                deposit = self.prompt_action("\ndeposit shortfall? [y/N] ")
+
+            elif 'notify_shortfall' in self.config and self.config['notify_shortfall']:
+                notify = True
+
+        if deposit:
+            m = MonzoAPI()
+
+            if not m.deposit_to_pot(self.account.account_id, pot, shortfall):
+                sys.stderr.write("ERROR: failed to deposit funds\n")
+
+                if 'notify_deposit' in self.config and self.config['notify_deposit']:
+                    self.notify(
+                        '%s - pot deposit failed' % (self.account.name),
+                        "£%.2f\n£%.2f due, £%.2f available" % (
+                            credit,
+                            self.due / 100,
+                            pot.balance
+                        )
+                    )
+            else:
+                if os.path.exists(self.shortfall_tracker):
+                    os.remove(self.shortfall_tracker)
+
+                if 'notify_deposit' in self.config and self.config['notify_deposit']:
+                    self.notify(
+                        '%s - pot topped up' % (self.account.name),
+                        "£%.2f\n£%.2f due, £%.2f available" % (
+                            shortfall,
+                            self.due / 100,
+                            pot.balance
+                        )
+                    )
+
+                return True
+
+        elif notify:
+            self.notify(
+                '%s - shortfall' % (self.account.name),
+                "£%.2f\n£%.2f due, £%.2f available" % (
+                    shortfall,
+                    self.due / 100,
+                    pot.balance
+                )
             )
 
-        for transaction in transactions:
-            if transaction.id not in self.seen:
-                self.seen.append(transaction.id)
+        return False
 
-                return transaction.date, transaction.money_out
 
-        return None, None
+    def handle_credit(self, pot, credit):
+        withdraw = False
+        notify = False
 
+        if 'pot' in self.config and 'auto_withdraw' in self.config and self.config['auto_withdraw'] and not sys.stdout.isatty() and not self.abbreviate:
+            if 'auto_withdraw_delay_mins' in self.config:
+                withdraw = self.handle_withdrawal_delay(credit)
+            else:
+                withdraw = True
+        elif not sys.stdout.isatty():
+            if 'notify_credit' in self.config and self.config['notify_credit'] and not self.abbreviate:
+                notify = True
+        else:
+            if 'pot' in self.config and 'prompt_withdraw' in self.config and self.config['prompt_withdraw']:
+                withdraw = self.prompt_action("\nwithdraw credit? [y/N] ")
 
-    def days_in_month(self, year, month):
-        return calendar.monthrange(year, month)[1]
+            elif 'notify_credit' in self.config and self.config['notify_credit']:
+                notify = True
 
+        if withdraw:
+            m = MonzoAPI()
 
-    def is_yearly_payment_due_this_month(self, payment, last_salary_date):
-        date_from = last_salary_date.strftime('%Y-%m-%d')
-        date = last_salary_date
+            if not m.withdraw_from_pot(self.account.account_id, pot, credit):
+                sys.stderr.write("ERROR: failed to withdraw credit\n")
 
-        while date.day <= 15:
-            date += datetime.timedelta(days=1)
+                if 'notify_withdraw' in self.config and self.config['notify_withdraw']:
+                    self.notify(
+                        '%s - pot credit withdraw failed' % (self.account.name),
+                        "£%.2f\n£%.2f due, £%.2f available" % (
+                            credit,
+                            self.due / 100,
+                            pot.balance
+                        )
+                    )
+            else:
+                if os.path.exists(self.credit_tracker):
+                    os.remove(self.credit_tracker)
 
-        while date.day != 15:
-            date += datetime.timedelta(days=1)
+                if 'notify_withdraw' in self.config and self.config['notify_withdraw']:
+                    self.notify(
+                        '%s - pot credit withdrawn' % (self.account.name),
+                        "£%.2f\n£%.2f due, £%.2f available" % (
+                            credit,
+                            self.due / 100,
+                            pot.balance
+                        )
+                    )
 
-        date_to = date.strftime('%Y-%m-%d')
+                return True
 
-        due_date = str(last_salary_date.year) + '-' + (str(payment['yearly_month']).rjust(2,'0')) + '-' + (str(payment['yearly_day']).rjust(2,'0'))
+        elif notify:
+            self.notify(
+                '%s - credit' % (self.account.name),
+                "£%.2f\n£%.2f due, £%.2f available" % (
+                    credit,
+                    self.due / 100,
+                    pot.balance
+                )
+            )
 
-        return due_date >= date_from and due_date <= date_to
+        return False
 
 
-    def get_exchange_rate(self, currency):
-        if currency in self.exchange_rates:
-            return self.exchange_rates[currency]
+    def handle_withdrawal_delay(self, credit):
+        credit_s = str(int(credit * 100))
 
-        if os.path.exists(self.monzo_config['exchange_rate_files'][currency]):
-            mtime = os.stat(self.monzo_config['exchange_rate_files'][currency]).st_mtime
+        if not os.path.exists(self.credit_tracker) or self.get_file_contents(self.credit_tracker).rstrip() != credit_s:
+            with open(self.credit_tracker,'w') as f:
+                f.write(credit_s)
 
-            dt = datetime.datetime.fromtimestamp(mtime)
+            return False
 
-            if dt.strftime('%Y%m%d') == datetime.datetime.now().strftime('%Y%m%d'):
-                self.exchange_rates[currency] = float(open(self.monzo_config['exchange_rate_files'][currency]).read())
+        elapsed = time.time() - os.stat(self.credit_tracker).st_mtime
 
-                return self.exchange_rates[currency]
+        return elapsed >= self.config['auto_withdraw_delay_mins'] * 60
 
-        resp = requests.get('https://raw.githubusercontent.com/TheArmagan/currency/main/api/GBP-to-%s.txt' % (currency.upper()))
-        rate = float(resp.text)
 
-        with open(self.monzo_config['exchange_rate_files'][currency], 'w') as f:
-            f.write(resp.text)
+    def get_file_contents(self, path):
+        return open(path).read()
 
-        self.exchange_rates[currency] = rate
 
-        return rate
+    def handle_deposit_delay(self, shortfall):
+        homedir = pwd.getpwuid(os.getuid()).pw_dir
 
+        shortfall_s = str(int(shortfall * 100))
 
-    def handle_amazon_payments(self, payment_day, payment, last_salary_date, next_salary_date):
-        amazon_due = 0
-        amazon_total = 0
-        amazon_next_month_bills_pot = 0
-        first = True
+        if not os.path.exists(self.shortfall_tracker) or self.get_file_contents(self.shortfall_tracker).rstrip() != shortfall_s:
+            with open(self.shortfall_tracker,'w') as f:
+                f.write(shortfall_s)
 
-        status, num_paid, remaining, last_amount, last_date, due_date = self.get_amazon_payment(payment, last_salary_date, next_salary_date, payment_day)
+            return False
 
-        self.display(status, 'Amazon Payments', payment['name'], last_amount, last_date, due_date, num_paid, payment['months'], remaining)
+        elapsed = time.time() - os.stat(self.shortfall_tracker).st_mtime
 
-        return amazon_due, amazon_total, amazon_next_month_bills_pot
+        return elapsed >= self.config['auto_deposit_delay_mins'] * 60
 
 
-    def get_amazon_payment(self, payment_spec, last_salary_date, next_salary_date, payment_day):
-        date_from = payment_spec['start_date']
+    def sanitise(self, output):
+        new_output = []
 
-        payments = []
+        for item in output:
+            obj = {}
+            
+            for key in item:
+                if type(item[key]) == datetime.date:
+                    obj[key] = item[key].strftime('%Y-%m-%d')
+                elif type(item[key]) == datetime.datetime:
+                    obj[key] = item[key].strftime('%Y-%m-%d %H:%M:%S')
+                elif type(item[key]) == decimal.Decimal:
+                    obj[key] = float(item[key])
+                else:
+                    obj[key] = item[key]
 
-        initial_amount = int(math.ceil(int(payment_spec['amount'] * 100) / payment_spec['months'])) / 100
-        final_amount = payment_spec['amount'] - (initial_amount * (payment_spec['months']-1))
+            new_output.append(obj)
 
-        payments = Transaction().find_all_by_provider_id_and_declined_and_description(
-            self.provider.id,
-            0,
-            payment_spec['desc'],
-            orderby='created_at',
-            orderdir='asc',
-            search=['description'],
-            where=[{
-                'clause': '`date` >= %s',
-                'params': [payment_spec['start_date']]
-            },{
-                'clause': '(money_out = %s or money_out = %s)',
-                'params': [initial_amount, final_amount]
-            }]
-        )
+        return new_output
 
-        num_paid = len(payments)
-        remaining = payment_spec['amount']
 
-        for payment in payments:
-            remaining -= payment.money_out
+    def check_pot_payments(self):
+        m = None
+        sync_required = False
 
-        if len(payments) >0:
-            last_amount = payments[-1].money_out
-            last_date = payments[-1].date
-        else:
-            last_amount = initial_amount
-            last_date = None
+        if 'payments_to_pots' not in self.config or type(self.config['payments_to_pots']) != list:
+            return sync_required
 
-        if num_paid < payment_spec['months']:
-            if last_date:
-                due_date = last_date + datetime.timedelta(months=1)
-            else:
-                due_date = datetime.datetime.now() + datetime.timedelta(days=1)
+        for payment in self.config['payments_to_pots']:
+            pot = Pot.one("select * from pot where name = %s and deleted = %s", [payment['name'], 0])
 
-                while due_date.day != payment_day:
-                    due_date += datetime.timedelta(days=1)
-        else:
-            due_date = None
+            if not pot:
+                continue
 
-        # if paid since last salary then status is PAID
-        if len(payments) >0 and payments[-1].date >= last_salary_date:
-            status = 'PAID'
+            if pot.last_monthly_transfer_date != self.last_salary_date:
+                amount_to_transfer = self.get_transfer_amount(pot, payment)
 
-        else:
-            # determine if the payment date falls before the next salary date
-            # if it does then this payment is DUE
-            now = datetime.datetime.now() + datetime.timedelta(days=1)
-            due = False
-
-            while 1:
-                if datetime.date(now.year, now.month, now.day) == next_salary_date:
-                    break
-
-                if now.day == payment_day:
-                    due = True
-                    break
+                if amount_to_transfer == 0:
+                    continue
 
-                now += datetime.timedelta(days=1)
+                if not m:
+                    m = MonzoAPI()
+                    sys.stdout.write("\n")
 
-            if due:
-                status = 'DUE'
-            else:
-                status = 'SKIPPED'
+                sys.stdout.write("Transferring £%.2f to pot: %s ... " % (amount_to_transfer / 100, pot.name))
+                sys.stdout.flush()
 
-        return status, num_paid, remaining, last_amount, last_date, due_date
+                if m.deposit_to_pot(self.account.account_id, pot, amount_to_transfer / 100):
+                    sys.stdout.write("OK\n")
 
+                    pot.last_monthly_transfer_date = self.last_salary_date
+                    pot.save()
 
-    def get_next_amazon_payment(self, i, payment_spec, payment, amount):
-        date_from = self.add_month(payment.date) - datetime.timedelta(days=7)
-        date_to = self.add_month(payment.date) + datetime.timedelta(days=7)
-
-        return Transaction().find_by_provider_id_and_declined_and_description_and_money_out(
-            self.provider['id'],
-            0,
-            payment_spec['desc'],
-            amount,
-            where=[{
-                'clause': '(`date` >= %s and `date` <= %s)',
-                'params': [date_from, date_to]
-            }]
-        )
+                    sync_required = True
+                else:
+                    sys.stdout.write("FAILED\n\n")
 
+                    sys.stderr.write("ERROR: failed to transfer £%.2f to pot: %s\n" % (amount_to_transfer / 100, pot.name))
 
-    def add_month(self, date):
-        if date.month == 12:
-            day = date.day
-            month = 1
-            year = date.year + 1
+        return sync_required
+
+
+    def get_transfer_amount(self, pot, payment):
+        amount = round(payment['amount'] * 100)
+
+        if 'topup' in payment and payment['topup']:
+            pot_balance = round(pot.balance * 100)
+            to_transfer = max([0, amount - pot_balance])
         else:
-            day = date.day
-            month = date.month + 1
-            year = date.year
+            to_transfer = amount
 
-        while 1:
-            try:
-                new_date = datetime.date(year, month, day)
-                break
-            except ValueError:
-                day -= 1
+        return to_transfer
 
-        return new_date
 
+    def adjust_column_widths(self, payment_lists):
+        for list_type in payment_lists:
+            for item in payment_lists[list_type]:
+                for key in item:
+                    if len(item[key]) > self.widths[key]:
+                        self.widths[key] = len(item[key])
+
+
+    def display_table(self, data):
+        for item in data:
+            for key in self.fields:
+                if key in ['Status']:
+                    sys.stdout.write(item[key].rjust(self.widths[key]))
+                else:
+                    sys.stdout.write(item[key].ljust(self.widths[key]))
+                sys.stdout.write(" ")
+
+            sys.stdout.write("\n")
+
+
+if __name__ == '__main__':
+    if len(sys.argv) <2:
+        print("usage: %s [-o json] <account_name>" % (sys.argv[0].split('/')[-1]))
+        sys.exit(1)
+
+    output_json = False
+    account = None
+    abbreviate = False
+
+    for i in range(1, len(sys.argv)):
+        if sys.argv[i] == '-o' and i+1 < len(sys.argv) and sys.argv[i+1] == 'json':
+            output_json = True
+            continue
+        else:
+            if sys.argv[i] == '-a':
+                abbreviate = True
+                continue
+
+            if sys.argv[i-1] == '-o':
+                continue
+
+            account = sys.argv[i]
 
-    def get_num_payments_made(self, payment):
-        return len(Transaction().find_all_by_declined_and_money_out_and_description(
-            0,
-            payment['amount'],
-            payment['desc'],
-            where=[{
-                'clause': '`date` >= %s',
-                'params': [payment['start_date']]
-            }]
-        ))
-
-
-if len(sys.argv) <2:
-    print("usage: %s <account_name>" % (sys.argv[0].split('/')[-1]))
-    sys.exit(1)
+    if account is None:
+        print("usage: %s [-o json] [-a] <account_name>" % (sys.argv[0].split('/')[-1]))
+        sys.exit(1)
 
-p = PaymentFundsCheck(sys.argv[1])
-p.main()
+    p = MonzoPayments(account, output_json, abbreviate)
+    p.main()
```

## Comparing `monzo_utils-0.0.9.data/scripts/monzo-search` & `monzo_utils-0.0.90.data/scripts/monzo-search`

 * *Files 5% similar despite different names*

```diff
@@ -7,40 +7,32 @@
 import re
 import datetime
 import yaml
 import pwd
 import warnings
 import dateparser
 import calendar
+from monzo_utils.lib.config import Config
 from monzo_utils.lib.db import DB
+from monzo_utils.model.transaction import Transaction
 
 # Ignore dateparser warnings regarding pytz
 warnings.filterwarnings(
     "ignore",
     message="The localize method is no longer necessary, as this time zone supports the fold attribute",
 )
 
 FIELD_MAP = {
     'date': 'created_at'
 }
 
 class Monzo:
 
     def __init__(self, args):
-        homedir = pwd.getpwuid(os.getuid()).pw_dir
-        monzo_dir = f"{homedir}/.monzo"
-
-        if not os.path.exists(monzo_dir):
-            os.mkdir(monzo_dir, 0o755)
-
-        config_file = f"{monzo_dir}/config.yaml"
-
-        self.config = yaml.safe_load(open(config_file).read())
-
-        self.db = DB(self.config['db'])
+        self.db = DB()
 
         include_pots = False
         show_declined = False
 
         on_date = None
         date_range = False
         date_from = datetime.datetime.now() - datetime.timedelta(days=365)
@@ -137,74 +129,78 @@
                     continue
                 except Exception as e:
                     sys.stderr.write("unparseable date format '%s': %s\n" % (args[i+1], str(e)))
                     sys.exit(1)
  
             query_args.append(args[i])
 
-        sql = "select transaction.*, account.name as account, pot.name as pot, transaction_metadata.value as mastercard_lifecycle_id from transaction join account on transaction.account_id = account.id left join transaction_metadata on transaction_metadata.transaction_id = transaction.id and transaction_metadata.`key` = %s left join pot on transaction.pot_id = pot.id where declined = %s and ((money_in >0 or money_out >0)"
-        params = [
-            'metadata_mastercard_lifecycle_id',
-            1 if show_declined else 0
-        ]
+        query = Transaction() \
+            .select('`transaction`.*') \
+            .select('transaction_metadata.value as mastercard_lifecycle_id') \
+            .select('account.name as account') \
+            .select('pot.name as pot') \
+            .join('account') \
+            .leftJoin('transaction_metadata', where=['key', 'metadata_mastercard_lifecycle_id']) \
+            .leftJoin('pot') \
+            .where('declined = %s', [1 if show_declined else 0]) \
+            .andWhere('money_in > %s or money_out > %s', [0,0])
+
+        if 'exclude_accounts' in Config().keys:
+            for exclude_account in Config().exclude_accounts:
+                query.andWhere('account.name != %s', [exclude_account])
 
         if len(query_args) >0:
             query_string = (' '.join(query_args))
+            query_param = '%' + query_string + '%'
 
-            query = '%' + query_string + '%'
-
-            sql += " and description like %s"
-            params.append(query)
+            clause = 'description like %s'
+            params = [query_param]
 
             if query_string.replace('.','').isdigit():
                 # integer value is queried as a range <n>.00 - <n>.99
                 if query_string.isdigit():
                     money_from = '%s.00' % (query_string)
                     money_to = '%s.99' % (query_string)
 
-                    sql += " or (money_in >0 and money_in >= %s and money_in <= %s) or (money_out >0 and money_out >= %s and money_out <= %s)"
+                    clause += " or (money_in >0 and money_in >= %s and money_in <= %s) or (money_out >0 and money_out >= %s and money_out <= %s)"
                     params += [money_from, money_to, money_from, money_to]
+
                 # query for specific value, eg 10.99
                 else:
                     while len(query_string.split('.')[1]) <2:
                         query_string += '0'
 
-                    sql += "or (money_in >0 and money_in = %s) or (money_out >0 and money_out = %s)"
-
+                    clause += "or (money_in >0 and money_in = %s) or (money_out >0 and money_out = %s)"
                     params += [query_string, query_string]
 
-        sql += ")"
+            query.andWhere(clause, params)
 
         if include_pots is False:
-            sql += " and description not like %s"
-            params.append('pot_0000%')
+            query.andWhere('description not like %s', ['pot_0000%'])
 
         if on_date:
-            sql += " and transaction.date = %s"
-            params.append(on_date)
+            query.andWhere('`transaction`.`date` = %s', [on_date])
         else:
             if date_from:
-                sql += " and transaction.date >= %s"
-                params.append(date_from)
+                query.andWhere('`transaction`.`date` >= %s', [date_from])
             if date_to:
-                sql += " and transaction.date <= %s"
-                params.append(date_to)
-
-        sql += " group by id order by date, created_at"
+                query.andWhere('`transaction`.`date` <= %s', [date_to])
 
-        rows = self.db.query(sql, params)
+        transactions = query.groupBy('`transaction`.id') \
+            .orderBy('date, created_at', 'asc') \
+            .getall()
 
-        rows = self.process_pending_refunds(rows)
+        transactions = self.process_pending_refunds(transactions)
 
         display_columns = ['account','pot','date','money_in','money_out','description']
 
         if show_declined:
             display_columns.append('decline_reason')
 
-        self.display(rows, display_columns)
+        self.display(transactions, display_columns)
 
 
     def help(self):
         cmd = sys.argv[0].split('/')[-1]
 
         print("usage:\n")
         print("%s [-p] [-d] [search string]\n" % (cmd))
@@ -240,25 +236,31 @@
             widths[key] = len(key)
 
         last_date = None
 
         today = datetime.datetime.now()
 
         for i in range(0, len(data)):
+            if type(data[i]) != dict:
+                data[i] = data[i].__dict__
+
             for key in columns:
                 if key in FIELD_MAP:
                     if data[i][FIELD_MAP[key]]:
                         data[i][key] = data[i][FIELD_MAP[key]]
 
                 if key == 'date':
                     data[i][key] = self.adjust_timestamp(data[i][key])
 
-                if key == 'money_out' and data[i]['pending'] and type(data[i]['money_out']) != str:
+                if key == 'money_out' and data[i]['pending'] and data[i]['money_out'] is not None:
                     data[i]['money_out'] = '*' + str(data[i]['money_out']) + '*'
 
+                if key == 'money_in' and data[i]['pending'] and data[i]['money_in'] is not None:
+                    data[i]['money_in'] = '*' + str(data[i]['money_in']) + '*'
+
                 if key == 'date':
                     pattern = '%d/%m' if data[i][key].year == today.year else '%d/%m/%y'
 
                     this_date = data[i][key].strftime(pattern)
 
                     if this_date == last_date:
                         data[i][key] = data[i][key].strftime('%H:%M')
```

## Comparing `monzo_utils-0.0.9.data/scripts/monzo-status` & `monzo_utils-0.0.90.data/scripts/monzo-status`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import sys
 import time
 import json
 import datetime
 import yaml
 import pwd
+from monzo_utils.lib.config import Config
 from monzo_utils.lib.db import DB
 from monzo_utils.model.provider import Provider
 from monzo_utils.model.account import Account
 from monzo_utils.model.pot import Pot
 from monzo_utils.model.transaction import Transaction
 
 PROVIDER = 'Monzo'
@@ -19,40 +20,26 @@
     'date': 'created_at'
 }
 
 class Monzo:
 
     widths = {}
 
-    def __init__(self):
-        homedir = pwd.getpwuid(os.getuid()).pw_dir
-        monzo_dir = f"{homedir}/.monzo"
-
-        if not os.path.exists(monzo_dir):
-            os.mkdir(monzo_dir, 0o755)
-
-        config_file = f"{monzo_dir}/config.yaml"
-
-        self.config = yaml.safe_load(open(config_file).read())
-
-        self.db = DB(self.config['db'])
-
-
     def accounts(self, first=True):
         transactions = False
         n = 10
 
         for i in range(0, len(sys.argv)):
             if sys.argv[i] == '-t':
                 transactions = True
                 if i+1 < len(sys.argv) and sys.argv[i+1].isdigit():
                     n = int(sys.argv[i+1])
 
-        provider = Provider().find_by_name(PROVIDER)
-        accounts = provider.accounts(order=self.config['account_order'] if 'account_order' in self.config else None)
+        provider = Provider.one("select * from provider where name = %s", [PROVIDER])
+        accounts = provider.accounts(order=Config().account_order if 'account_order' in Config().keys else None)
 
         count = 0
         for account in accounts:
             self.display([account], account.keys, show_headers=(count == 0 or transactions))
 
             if transactions:
                 sys.stdout.write("\n")
@@ -73,15 +60,15 @@
                     self.widths[key] = 8
             else:
                 if key not in self.widths or self.widths[key] < len(key):
                     self.widths[key] = len(key)
 
         for i in range(0, len(data)):
             if type(data[i]) != dict:
-                obj = data[i].__dict__['attrs']
+                obj = data[i].__dict__['attributes']
             else:
                 obj = data[i]
 
             for key in columns:
                 if key in FIELD_MAP:
                     obj[key] = obj[FIELD_MAP[key]]
 
@@ -105,15 +92,15 @@
 
             for key in columns:
                 sys.stdout.write('-' * (self.widths[key]+2))
             sys.stdout.write("\n")
 
         for i in range(0, len(data)):
             if type(data[i]) != dict:
-                obj = data[i].__dict__['attrs']
+                obj = data[i].__dict__['attributes']
             else:
                 obj = data[i]
 
             for key in columns:
                 sys.stdout.write(str(obj[key]).ljust(self.widths[key]+2))
 
             sys.stdout.write("\n")
```

## Comparing `monzo_utils-0.0.9.dist-info/LICENSE` & `monzo_utils-0.0.90.dist-info/LICENSE`

 * *Files identical despite different names*

