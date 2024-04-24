# Comparing `tmp/minidb-2.0.7.tar.gz` & `tmp/minidb-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidb-2.0.7.tar", last modified: Fri Sep 16 18:41:57 2022, max compression
+gzip compressed data, was "minidb-2.0.8.tar", last modified: Wed Apr 24 19:00:37 2024, max compression
```

## Comparing `minidb-2.0.7.tar` & `minidb-2.0.8.tar`

### file list

```diff
@@ -1,7 +1,14 @@
-drwxr-xr-x   0 thp       (1000) thp       (1000)        0 2022-09-16 18:41:57.046341 minidb-2.0.7/
--rw-r--r--   0 thp       (1000) thp       (1000)      300 2022-09-16 18:41:57.046341 minidb-2.0.7/PKG-INFO
--rw-r--r--   0 thp       (1000) thp       (1000)    32094 2022-09-16 18:41:32.398203 minidb-2.0.7/minidb.py
--rw-r--r--   0 thp       (1000) thp       (1000)      224 2021-06-06 10:46:33.866839 minidb-2.0.7/setup.cfg
--rw-r--r--   0 thp       (1000) thp       (1000)      602 2021-06-06 10:46:33.866839 minidb-2.0.7/setup.py
-drwxr-xr-x   0 thp       (1000) thp       (1000)        0 2022-09-16 18:41:57.046341 minidb-2.0.7/test/
--rw-r--r--   0 thp       (1000) thp       (1000)    19505 2022-09-12 08:30:09.615189 minidb-2.0.7/test/test_minidb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:00:37.366820 minidb-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-24 19:00:31.000000 minidb-2.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-24 19:00:37.366820 minidb-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-04-24 19:00:31.000000 minidb-2.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:00:37.366820 minidb-2.0.8/minidb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-24 19:00:37.000000 minidb-2.0.8/minidb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-24 19:00:37.000000 minidb-2.0.8/minidb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:00:37.000000 minidb-2.0.8/minidb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 19:00:37.000000 minidb-2.0.8/minidb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    32106 2024-04-24 19:00:31.000000 minidb-2.0.8/minidb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-24 19:00:37.366820 minidb-2.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-24 19:00:31.000000 minidb-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:00:37.366820 minidb-2.0.8/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    20312 2024-04-24 19:00:31.000000 minidb-2.0.8/test/test_minidb.py
```

### Comparing `minidb-2.0.7/minidb.py` & `minidb-2.0.8/minidb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #           _      _    _ _
 #     _ __ (_)_ _ (_)__| | |__
 #    | '  \| | ' \| / _` | '_ \
 #    |_|_|_|_|_||_|_\__,_|_.__/
 #    simple python object store
 #
-# Copyright 2009-2010, 2014-2022 Thomas Perl <thp.io>. All rights reserved.
+# Copyright 2009-2010, 2014-2022, 2024 Thomas Perl <thp.io>. All rights reserved.
 #
 # Permission to use, copy, modify, and/or distribute this software for any
 # purpose with or without fee is hereby granted, provided that the above
 # copyright notice and this permission notice appear in all copies.
 #
 # THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
@@ -32,15 +32,15 @@
 import sys
 import json
 import datetime
 import logging
 
 
 __author__ = 'Thomas Perl <m@thp.io>'
-__version__ = '2.0.7'
+__version__ = '2.0.8'
 __url__ = 'http://thp.io/2010/minidb/'
 __license__ = 'ISC'
 
 
 __all__ = [
     # Main classes
     'Store', 'Model', 'JSON',
@@ -408,15 +408,15 @@
             columns = [d[0] for d in result.description]
 
             def _decode(row, columns):
                 for name, value in zip(columns, row):
                     type_ = attr_to_type.get(name, None)
                     yield (self.deserialize(value, type_) if type_ is not None else value)
 
-            return (RowProxy(tuple(_decode(row, columns)), columns) for row in result)
+            return (RowProxy(tuple(_decode(row, columns)), columns) for row in list(result))
 
     def load(self, class_, *args, **kwargs):
         with self.lock:
             query = kwargs.get('__query__', None)
             if '__query__' in kwargs:
                 del kwargs['__query__']
```

### Comparing `minidb-2.0.7/setup.py` & `minidb-2.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # Setup script for
 'minidb'
 # by Thomas Perl <thp.io>
 
 import os
 import re
-from distutils.core import setup
+from setuptools import setup
 
 dirname = os.path.dirname(os.path.abspath(__file__))
 src = open(os.path.join(dirname, '{}.py'.format(__doc__))).read()
 docstrings = re.findall('"""(.*)"""', src)
 m = dict(re.findall(r"__([a-z_]+)__\s*=\s*'([^']+)'", src))
 m['name'] = __doc__
 m['author'], m['author_email'] = re.match(r'(.*) <(.*)>', m['author']).groups()
```

### Comparing `minidb-2.0.7/test/test_minidb.py` & `minidb-2.0.8/test/test_minidb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import concurrent.futures
 import minidb
 import pytest
 import datetime
 
 
 class FieldTest(minidb.Model):
     CONSTANT = 123
@@ -260,18 +261,18 @@
     class FloatModel(minidb.Model):
         value = float
 
     with minidb.Store(debug=True) as db:
         db.register(FloatModel)
         float_id = FloatModel(value=3.1415).save(db).id
         get_value = FloatModel.get(db, id=float_id).value
-        assert type(get_value) == float
+        assert isinstance(get_value, float)
         assert get_value == 3.1415
         query_value = next(FloatModel.c.value.query(db, where=lambda c: c.id == float_id)).value
-        assert type(query_value) == float
+        assert isinstance(query_value, float)
         assert query_value == 3.1415
 
 
 def test_storing_and_retrieving_bytes():
     # http://probablyprogramming.com/2009/03/15/the-tiniest-gif-ever
     BLOB = (b'GIF89a\x01\x00\x01\x00\x80\x01\x00\xff\xff\xff\x00\x00\x00' +
             b'!\xf9\x04\x01\n\x00\x01\x00,\x00\x00\x00\x00\x01\x00\x01' +
@@ -280,18 +281,18 @@
     class BytesModel(minidb.Model):
         value = bytes
 
     with minidb.Store(debug=True) as db:
         db.register(BytesModel)
         bytes_id = BytesModel(value=BLOB).save(db).id
         get_value = BytesModel.get(db, id=bytes_id).value
-        assert type(get_value) == bytes
+        assert isinstance(get_value, bytes)
         assert get_value == BLOB
         query_value = next(BytesModel.c.value.query(db, where=lambda c: c.id == bytes_id)).value
-        assert type(query_value) == bytes
+        assert isinstance(query_value, bytes)
         assert query_value == BLOB
 
 
 def test_get_with_multiple_value_raises_exception():
     with pytest.raises(ValueError):
         class Mod(minidb.Model):
             mod = str
@@ -586,27 +587,27 @@
         da = datetime.date
         tm = datetime.time
 
     with minidb.Store(debug=True) as db:
         db.register(DateTimeModel)
         datetime_id = DateTimeModel(dt=DT_NOW, da=D_TODAY, tm=T_NOW).save(db).id
         get_value = DateTimeModel.get(db, id=datetime_id)
-        assert type(get_value.dt) == datetime.datetime
+        assert isinstance(get_value.dt, datetime.datetime)
         assert get_value.dt == DT_NOW
-        assert type(get_value.da) == datetime.date
+        assert isinstance(get_value.da, datetime.date)
         assert get_value.da == D_TODAY
-        assert type(get_value.tm) == datetime.time
+        assert isinstance(get_value.tm, datetime.time)
         assert get_value.tm == T_NOW
         query_value = next(DateTimeModel.query(db, lambda c: c.dt // c.da // c.tm,
                                                where=lambda c: c.id == datetime_id))
-        assert type(query_value.dt) == datetime.datetime
+        assert isinstance(query_value.dt, datetime.datetime)
         assert query_value.dt == DT_NOW
-        assert type(query_value.da) == datetime.date
+        assert isinstance(query_value.da, datetime.date)
         assert query_value.da == D_TODAY
-        assert type(query_value.tm) == datetime.time
+        assert isinstance(query_value.tm, datetime.time)
         assert query_value.tm == T_NOW
 
 
 def test_query_with_datetime():
     DT_NOW = datetime.datetime.now()
 
     class DateTimeModel(minidb.Model):
@@ -636,19 +637,19 @@
         position = Point
 
     with minidb.Store(debug=True) as db:
         db.register(Player)
         p = Point(1.12, 5.99)
         player_id = Player(name='Foo', position=p).save(db).id
         get_value = Player.get(db, id=player_id)
-        assert type(get_value.position) == Point
+        assert isinstance(get_value.position, Point)
         assert (get_value.position.x, get_value.position.y) == (p.x, p.y)
         query_value = next(Player.query(db, lambda c: c.position,
                                         where=lambda c: c.id == player_id))
-        assert type(query_value.position) == Point
+        assert isinstance(query_value.position, Point)
         assert (query_value.position.x, query_value.position.y) == (p.x, p.y)
 
 
 def test_delete_all():
     class Thing(minidb.Model):
         bla = str
         blubb = int
@@ -658,7 +659,34 @@
 
         db.save(Thing(bla='a', blubb=123))
         db.save(Thing(bla='c', blubb=456))
         assert db.count_rows(Thing) == 2
 
         db.delete_all(Thing)
         assert db.count_rows(Thing) == 0
+
+
+def test_threaded_query():
+    class Thing(minidb.Model):
+        s = str
+        i = int
+
+    with minidb.Store(debug=True, vacuum_on_close=False) as db:
+        db.register(Thing)
+
+        for i in range(100):
+            db.save(Thing(s=str(i), i=i))
+
+        def query(i):
+            things = list(Thing.query(db, Thing.c.s // Thing.c.i, where=Thing.c.i == i))
+            assert len(things) == 1
+
+            thing = things[0]
+            assert thing is not None
+            assert thing.s == str(i)
+            assert thing.i == i
+
+            return i
+
+        executor = concurrent.futures.ThreadPoolExecutor(max_workers=10)
+        # Wrap in list to resolve all the futures
+        list(executor.map(query, range(100)))
```

