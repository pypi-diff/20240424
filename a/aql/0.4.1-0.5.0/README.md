# Comparing `tmp/aql-0.4.1.tar.gz` & `tmp/aql-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aql-0.4.1.tar", last modified: Sat Oct 31 03:40:41 2020, max compression
+gzip compressed data, was "aql-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aql-0.4.1.tar` & `aql-0.5.0.tar`

### file list

```diff
@@ -1,53 +1,50 @@
--rw-r--r--   0        0        0     1219 2020-07-16 04:27:33.217662 aql-0.4.1/.gitignore
--rw-r--r--   0        0        0    16971 2019-10-26 20:06:10.952704 aql-0.4.1/.pylint
--rw-r--r--   0        0        0       75 2019-07-25 02:34:50.852871 aql-0.4.1/.pyup.yml
--rw-r--r--   0        0        0      156 2020-07-16 05:06:10.151219 aql-0.4.1/.readthedocs.yml
--rw-r--r--   0        0        0     1288 2020-10-31 03:25:43.004155 aql-0.4.1/CHANGELOG.md
--rw-r--r--   0        0        0     3212 2019-07-25 02:34:50.853174 aql-0.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      755 2020-07-16 04:55:57.964527 aql-0.4.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1067 2019-07-25 02:34:50.853490 aql-0.4.1/LICENSE
--rw-r--r--   0        0        0       26 2019-07-25 02:34:50.853629 aql-0.4.1/MANIFEST.in
--rw-r--r--   0        0        0     2057 2020-07-16 04:52:13.090214 aql-0.4.1/README.md
--rw-r--r--   0        0        0      473 2020-10-31 03:35:11.718761 aql-0.4.1/aql/__init__.py
--rw-r--r--   0        0        0       22 2020-10-31 03:35:09.471767 aql-0.4.1/aql/__version__.py
--rw-r--r--   0        0        0     3774 2020-10-31 03:35:09.773110 aql-0.4.1/aql/column.py
--rw-r--r--   0        0        0      837 2020-10-31 03:35:09.552127 aql-0.4.1/aql/connector.py
--rw-r--r--   0        0        0      225 2020-10-31 03:35:10.882761 aql-0.4.1/aql/engines/__init__.py
--rw-r--r--   0        0        0     9054 2020-10-31 03:35:11.329141 aql-0.4.1/aql/engines/base.py
--rw-r--r--   0        0        0     2923 2020-10-31 03:35:11.397323 aql-0.4.1/aql/engines/mysql.py
--rw-r--r--   0        0        0     6652 2020-10-31 03:35:11.135766 aql-0.4.1/aql/engines/sql.py
--rw-r--r--   0        0        0     2944 2020-10-31 03:35:10.957413 aql-0.4.1/aql/engines/sqlite.py
--rw-r--r--   0        0        0      436 2020-10-31 03:35:09.679309 aql-0.4.1/aql/errors.py
--rw-r--r--   0        0        0        0 2020-10-31 01:49:20.589587 aql-0.4.1/aql/py.typed
--rw-r--r--   0        0        0     7549 2020-10-31 03:35:09.459443 aql-0.4.1/aql/query.py
--rw-r--r--   0        0        0     4950 2020-10-31 03:35:09.667694 aql-0.4.1/aql/table.py
--rw-r--r--   0        0        0      240 2020-10-31 03:35:09.991048 aql-0.4.1/aql/tests/__init__.py
--rw-r--r--   0        0        0      177 2020-10-31 03:35:10.187394 aql-0.4.1/aql/tests/__main__.py
--rw-r--r--   0        0        0     4429 2020-10-31 03:35:10.321625 aql-0.4.1/aql/tests/column.py
--rw-r--r--   0        0        0      709 2020-10-31 03:35:10.020864 aql-0.4.1/aql/tests/connector.py
--rw-r--r--   0        0        0      250 2020-10-31 03:35:10.327372 aql-0.4.1/aql/tests/engines/__init__.py
--rw-r--r--   0        0        0     1290 2020-10-31 03:35:10.805036 aql-0.4.1/aql/tests/engines/base.py
--rw-r--r--   0        0        0     2671 2020-10-31 03:35:10.470356 aql-0.4.1/aql/tests/engines/integration.py
--rw-r--r--   0        0        0     3424 2020-10-31 03:35:10.877287 aql-0.4.1/aql/tests/engines/mysql.py
--rw-r--r--   0        0        0    14259 2020-10-31 03:35:10.770642 aql-0.4.1/aql/tests/engines/sql.py
--rw-r--r--   0        0        0     3239 2020-10-31 03:35:10.400881 aql-0.4.1/aql/tests/engines/sqlite.py
--rw-r--r--   0        0        0     6573 2020-10-31 03:35:09.985118 aql-0.4.1/aql/tests/query.py
--rw-r--r--   0        0        0     5295 2020-10-31 03:35:10.182123 aql-0.4.1/aql/tests/table.py
--rw-r--r--   0        0        0      387 2020-10-31 03:35:10.003773 aql-0.4.1/aql/tests/types.py
--rw-r--r--   0        0        0     2037 2020-10-31 03:35:09.532911 aql-0.4.1/aql/types.py
--rw-r--r--   0        0        0      284 2020-07-16 04:07:42.111871 aql-0.4.1/docs/_static/custom.css
--rw-r--r--   0        0        0      342 2020-07-16 04:07:42.110586 aql-0.4.1/docs/_templates/badges.html
--rw-r--r--   0        0        0      934 2020-07-16 04:07:42.110841 aql-0.4.1/docs/_templates/omnilib.html
--rw-r--r--   0        0        0      503 2020-07-16 04:22:55.963904 aql-0.4.1/docs/api.rst
--rw-r--r--   0        0        0       70 2020-07-16 04:07:42.112158 aql-0.4.1/docs/changelog.rst
--rw-r--r--   0        0        0     2751 2020-07-16 04:09:37.214833 aql-0.4.1/docs/conf.py
--rw-r--r--   0        0        0       79 2020-07-16 04:07:42.110041 aql-0.4.1/docs/contributing.rst
--rw-r--r--   0        0        0      171 2020-07-16 04:50:25.911251 aql-0.4.1/docs/index.rst
--rw-r--r--   0        0        0      244 2020-07-16 04:49:42.817225 aql-0.4.1/docs/roadmap.rst
--rw-r--r--   0        0        0      752 2020-10-14 04:54:31.682829 aql-0.4.1/makefile
--rw-r--r--   0        0        0       57 2020-07-16 01:55:50.797982 aql-0.4.1/mypy.ini
--rw-r--r--   0        0        0     1104 2020-07-16 04:32:47.500440 aql-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      237 2020-10-31 01:48:47.383615 aql-0.4.1/requirements-dev.txt
--rw-r--r--   0        0        0       13 2020-10-14 04:51:19.310400 aql-0.4.1/requirements.txt
--rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 aql-0.4.1/setup.py
--rw-r--r--   0        0        0      174 1970-01-01 00:00:00.000000 aql-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      180 2024-04-23 09:00:35.952692 aql-0.5.0/.flake8
+-rw-r--r--   0        0        0     1219 2024-04-23 08:18:44.926862 aql-0.5.0/.gitignore
+-rw-r--r--   0        0        0       50 2024-04-23 08:18:44.926955 aql-0.5.0/.mailmap
+-rw-r--r--   0        0        0      209 2024-04-23 08:47:22.132518 aql-0.5.0/.readthedocs.yml
+-rw-r--r--   0        0        0     1867 2024-04-24 02:12:43.358752 aql-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3216 2024-04-23 08:18:44.927241 aql-0.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      743 2024-04-24 01:52:19.443703 aql-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1071 2024-04-23 08:18:44.927434 aql-0.5.0/LICENSE
+-rw-r--r--   0        0        0       26 2024-04-23 08:18:44.927522 aql-0.5.0/MANIFEST.in
+-rw-r--r--   0        0        0     2060 2024-04-24 01:52:19.443838 aql-0.5.0/README.md
+-rw-r--r--   0        0        0      481 2024-04-24 01:41:43.846773 aql-0.5.0/aql/__init__.py
+-rw-r--r--   0        0        0      156 2024-04-24 02:12:43.368088 aql-0.5.0/aql/__version__.py
+-rw-r--r--   0        0        0     3712 2024-04-24 01:52:19.444077 aql-0.5.0/aql/column.py
+-rw-r--r--   0        0        0      841 2024-04-24 01:41:43.790413 aql-0.5.0/aql/connector.py
+-rw-r--r--   0        0        0      229 2024-04-24 01:41:43.852145 aql-0.5.0/aql/engines/__init__.py
+-rw-r--r--   0        0        0     9099 2024-04-24 01:52:19.444340 aql-0.5.0/aql/engines/base.py
+-rw-r--r--   0        0        0     2927 2024-04-24 01:41:43.833349 aql-0.5.0/aql/engines/mysql.py
+-rw-r--r--   0        0        0     6656 2024-04-24 01:41:43.849015 aql-0.5.0/aql/engines/sql.py
+-rw-r--r--   0        0        0     2948 2024-04-24 01:41:43.813026 aql-0.5.0/aql/engines/sqlite.py
+-rw-r--r--   0        0        0      440 2024-04-24 01:41:43.830740 aql-0.5.0/aql/errors.py
+-rw-r--r--   0        0        0        0 2024-04-23 08:18:44.928891 aql-0.5.0/aql/py.typed
+-rw-r--r--   0        0        0     7563 2024-04-24 01:52:19.444603 aql-0.5.0/aql/query.py
+-rw-r--r--   0        0        0     5005 2024-04-24 01:52:19.444772 aql-0.5.0/aql/table.py
+-rw-r--r--   0        0        0      258 2024-04-24 01:41:43.835067 aql-0.5.0/aql/tests/__init__.py
+-rw-r--r--   0        0        0      181 2024-04-24 01:41:43.846772 aql-0.5.0/aql/tests/__main__.py
+-rw-r--r--   0        0        0     4433 2024-04-24 01:41:43.869283 aql-0.5.0/aql/tests/column.py
+-rw-r--r--   0        0        0      713 2024-04-24 01:41:43.844606 aql-0.5.0/aql/tests/connector.py
+-rw-r--r--   0        0        0      254 2024-04-24 01:41:43.792430 aql-0.5.0/aql/tests/engines/__init__.py
+-rw-r--r--   0        0        0     1294 2024-04-24 01:41:43.854880 aql-0.5.0/aql/tests/engines/base.py
+-rw-r--r--   0        0        0     2675 2024-04-24 01:41:43.815125 aql-0.5.0/aql/tests/engines/integration.py
+-rw-r--r--   0        0        0     3428 2024-04-24 01:41:43.852138 aql-0.5.0/aql/tests/engines/mysql.py
+-rw-r--r--   0        0        0    14263 2024-04-24 01:41:43.805317 aql-0.5.0/aql/tests/engines/sql.py
+-rw-r--r--   0        0        0     3243 2024-04-24 01:41:43.863810 aql-0.5.0/aql/tests/engines/sqlite.py
+-rw-r--r--   0        0        0     6568 2024-04-24 01:41:43.873815 aql-0.5.0/aql/tests/query.py
+-rw-r--r--   0        0        0     5299 2024-04-24 01:41:43.844707 aql-0.5.0/aql/tests/table.py
+-rw-r--r--   0        0        0      391 2024-04-24 01:41:43.818280 aql-0.5.0/aql/tests/types.py
+-rw-r--r--   0        0        0     2041 2024-04-24 01:41:43.860328 aql-0.5.0/aql/types.py
+-rw-r--r--   0        0        0      284 2024-04-23 08:18:44.931061 aql-0.5.0/docs/_static/custom.css
+-rw-r--r--   0        0        0      342 2024-04-23 08:18:44.931220 aql-0.5.0/docs/_templates/badges.html
+-rw-r--r--   0        0        0      934 2024-04-23 08:18:44.931313 aql-0.5.0/docs/_templates/omnilib.html
+-rw-r--r--   0        0        0      503 2024-04-23 08:18:44.931412 aql-0.5.0/docs/api.rst
+-rw-r--r--   0        0        0       70 2024-04-23 08:18:44.931502 aql-0.5.0/docs/changelog.rst
+-rw-r--r--   0        0        0     2806 2024-04-23 08:18:44.931604 aql-0.5.0/docs/conf.py
+-rw-r--r--   0        0        0       79 2024-04-23 08:18:44.931684 aql-0.5.0/docs/contributing.rst
+-rw-r--r--   0        0        0      171 2024-04-23 08:18:44.931781 aql-0.5.0/docs/index.rst
+-rw-r--r--   0        0        0      244 2024-04-23 08:18:44.931884 aql-0.5.0/docs/roadmap.rst
+-rw-r--r--   0        0        0      751 2024-04-23 08:47:22.133337 aql-0.5.0/makefile
+-rw-r--r--   0        0        0       57 2024-04-23 08:18:44.932070 aql-0.5.0/mypy.ini
+-rw-r--r--   0        0        0     1442 2024-04-24 02:07:53.047406 aql-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3581 1970-01-01 00:00:00.000000 aql-0.5.0/PKG-INFO
```

### Comparing `aql-0.4.1/.gitignore` & `aql-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aql-0.4.1/CODE_OF_CONDUCT.md` & `aql-0.5.0/CODE_OF_CONDUCT.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 ## Scope
 
 This Code of Conduct applies both within project spaces and in public spaces when an individual is representing the project or its community. Examples of representing a project or community include using an official project e-mail address, posting via an official social media account, or acting as an appointed representative at an online or offline event. Representation of a project may be further defined and clarified by project maintainers.
 
 ## Enforcement
 
-Instances of abusive, harassing, or otherwise unacceptable behavior may be reported by contacting the project team at john@noswap.com. The project team will review and investigate all complaints, and will respond in a way that it deems appropriate to the circumstances. The project team is obligated to maintain confidentiality with regard to the reporter of an incident. Further details of specific enforcement policies may be posted separately.
+Instances of abusive, harassing, or otherwise unacceptable behavior may be reported by contacting the project team at contact@omnilib.dev. The project team will review and investigate all complaints, and will respond in a way that it deems appropriate to the circumstances. The project team is obligated to maintain confidentiality with regard to the reporter of an incident. Further details of specific enforcement policies may be posted separately.
 
 Project maintainers who do not follow or enforce the Code of Conduct in good faith may face temporary or permanent repercussions as determined by other members of the project's leadership.
 
 ## Attribution
 
 This Code of Conduct is adapted from the [Contributor Covenant][homepage], version 1.4, available at [http://contributor-covenant.org/version/1/4][version]
```

### Comparing `aql-0.4.1/CONTRIBUTING.md` & `aql-0.5.0/CONTRIBUTING.md`

 * *Files 23% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 
 ## Preparation
 
 You'll need to have Python 3.6 or newer available for testing
 
 You can do this with [pyenv][]:
 
-    $ pyenv install 3.6.x
-    $ pyenv shell 3.6.x
-
+```sh
+pyenv install 3.6.x
+pyenv shell 3.6.x
+```
 
 ## Setup
 
 Once in your development environment, install the
 appropriate linting tools and dependencies:
 
-    $ cd <path/to/aql>
-    $ make venv
-    $ source .venv/bin/activate
-
+```sh
+cd <path/to/aql>
+make venv
+source .venv/bin/activate
+```
 
 ## Submitting
 
 Before submitting a pull request, please ensure
 that you have done the following:
 
 * Documented changes or features in `README.md` and/or `docs/`
```

### Comparing `aql-0.4.1/LICENSE` & `aql-0.5.0/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018 John Reese
+Copyright (c) 2022 Amethyst Reese
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `aql-0.4.1/README.md` & `aql-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 [![build status](https://github.com/omnilib/aql/workflows/Build/badge.svg)](https://github.com/omnilib/aql/actions)
 [![code coverage](https://img.shields.io/codecov/c/gh/omnilib/aql)](https://codecov.io/gh/omnilib/aql)
 [![version](https://img.shields.io/pypi/v/aql.svg)](https://pypi.org/project/aql)
 [![license](https://img.shields.io/pypi/l/aql.svg)](https://github.com/omnilib/aql/blob/main/LICENSE)
 [![code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
-
 Highlights
 ----------
 
 aql is a simple, modern, and composable query builder, with support for asynchronous
 execution of queries against multiple database backends using a unified API.
 aql uses modern, type annotated data structures for both table definitions and queries.
 
@@ -59,15 +58,14 @@
 async with connect(...) as db:
     rows = await db.get(Object, Object.id == 100)
     rows[0].description += "updated"
 
     await db.modify(Object, rows)
 ```
 
-
 License
 -------
 
-aql is copyright [John Reese](https://jreese.sh), and licensed under
+aql is copyright [Amethyst Reese](https://noswap.com), and licensed under
 the MIT license.  I am providing code in this repository to you under an open
 source license.  This is my personal repository; the license you receive to
 my code is from me and not from my employer. See the `LICENSE` file for details.
```

### Comparing `aql-0.4.1/aql/column.py` & `aql-0.5.0/aql/column.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 from typing import Any, Generic, Optional, Sequence, Type, TypeVar, Union
 
 from attr import dataclass
 
 from .errors import InvalidColumnType
@@ -24,18 +24,15 @@
         if name is not None:
             self._name = name
         else:
             names = [self._AUTO_PREFIX] + list(columns)
             self._name = "_".join(names)
 
     def __eq__(self, other):
-        return (
-            type(self) == type(other)  # pylint:disable=unidiomatic-typecheck
-            and self._columns == other._columns
-        )
+        return type(self) is type(other) and self._columns == other._columns
 
 
 class Unique(Index[T]):
     _AUTO_PREFIX = "unq"
 
 
 class Primary(Index[T]):
@@ -83,15 +80,15 @@
         return ctype
 
 
 class Column:
     def __init__(
         self,
         name: str,
-        ctype: Type = None,
+        ctype: Optional[Type] = None,
         default: Any = NO_DEFAULT,
         table_name: str = "",
     ) -> None:
         self.name = name
         self.ctype = ctype
         self.default = default
         self.table_name = table_name
```

### Comparing `aql-0.4.1/aql/connector.py` & `aql-0.5.0/aql/connector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 import re
 from typing import Any, Pattern, Union
 
 from .engines.base import Connection
 from .errors import InvalidURI
```

### Comparing `aql-0.4.1/aql/engines/base.py` & `aql-0.5.0/aql/engines/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 import logging
 from typing import (
     Any,
     AsyncIterator,
     Dict,
@@ -196,15 +196,15 @@
         return self._cursor.rowcount
 
     @property
     def last_id(self) -> Optional[int]:
         """ID of last modified row, or None if not available."""
         raise self._cursor.lastrowid
 
-    def convert(self, row) -> T:
+    def convert(self, row) -> T:  # type: ignore[type-var]
         """Convert from the cursor's native data type to the query object type."""
         if self._query:
             return self._query.table(row)
         else:
             return row
 
     async def close(self) -> None:
@@ -295,18 +295,18 @@
         prepared = self.connection.engine.prepare(self.query)
         await self._cursor.execute(prepared.sql, prepared.parameters)
         return self._cursor
 
     async def row(self) -> Optional[T]:
         cursor = await self.run()
         row = await cursor.fetchone()
-        if self.factory:
+        if row and self.factory:
             return self.factory(*row)
         return None
 
     async def rows(self) -> Sequence[T]:
         cursor = await self.run()
         rows = await cursor.fetchall()
         if self.factory:
-            return [self.factory(*row) for row in rows]
+            return [self.factory(*row) for row in rows if row]
         else:
             return rows
```

### Comparing `aql-0.4.1/aql/engines/mysql.py` & `aql-0.5.0/aql/engines/mysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# Copyright 2020 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 from typing import Any, List
 
 from ..column import NO_DEFAULT, Primary, Unique
 from ..errors import BuildError, NoConnection
 from ..query import PreparedQuery, Query
 from .base import Connection, MissingConnector
-from .sql import SqlEngine, T, q
+from .sql import q, SqlEngine, T
 
 try:
     import aiomysql
 except ModuleNotFoundError as e:  # pragma:nocover
     aiomysql = MissingConnector(e)
```

### Comparing `aql-0.4.1/aql/engines/sql.py` & `aql-0.5.0/aql/engines/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 from datetime import date, datetime
 from itertools import chain
 from typing import Any, List
 
 from attr import astuple
@@ -19,15 +19,15 @@
     Operator,
     Or,
     Select,
     SqlParams,
     TableJoin,
     Text,
 )
-from .base import Engine, T, q
+from .base import Engine, q, T
 
 
 class SqlEngine(Engine, name="sql"):
     """Generic SQL engine for generating standardized queries."""
 
     PLACEHOLDER = "?"
```

### Comparing `aql-0.4.1/aql/engines/sqlite.py` & `aql-0.5.0/aql/engines/sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Copyright 2020 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 import logging
 from typing import Any, List, TypeVar
 
 from ..column import NO_DEFAULT, Primary, Unique
 from ..errors import BuildError
 from ..query import PreparedQuery, Query
 from .base import Connection, MissingConnector
-from .sql import SqlEngine, q
+from .sql import q, SqlEngine
 
 try:
     import aiosqlite
 except ModuleNotFoundError as e:  # pragma:nocover
     aiosqlite = MissingConnector(e)  # type:ignore
 
 LOG = logging.getLogger(__name__)
```

### Comparing `aql-0.4.1/aql/query.py` & `aql-0.5.0/aql/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Copyright 2020 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 from typing import (
-    TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Generic,
     List,
     Optional,
     Sequence,
     Tuple,
     Type,
+    TYPE_CHECKING,
     TypeVar,
     Union,
 )
 
 from attr import make_class
 
 from .column import Column
@@ -197,15 +197,15 @@
             else:
                 order = Order.asc
                 remaining = remaining[1:]
             self._order.append((col, order))
         return self
 
     @only()
-    def limit(self, n: int, offset: int = None) -> "Query[T]":
+    def limit(self, n: int, offset: Optional[int] = None) -> "Query[T]":
         self._limit = n
         self._offset = offset
         return self
 
     @only()
     def offset(self, n: int) -> "Query[T]":
         self._offset = n
```

### Comparing `aql-0.4.1/aql/table.py` & `aql-0.5.0/aql/table.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,44 @@
-# Copyright 2020 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 from typing import (
     Any,
     Callable,
     Dict,
     Generic,
+    get_type_hints,
     Iterable,
     List,
     Optional,
+    overload,
     Set,
     Type,
     TypeVar,
     Union,
-    get_type_hints,
-    overload,
 )
 
-from attr import NOTHING, dataclass, fields_dict
+from attr import dataclass, fields_dict, NOTHING
 
-from .column import NO_DEFAULT, Column, ColumnType, Index
+from .column import Column, ColumnType, Index, NO_DEFAULT
 from .errors import AqlError, DuplicateColumnName
 from .query import Query
 from .types import Comparison
 
 T = TypeVar("T")
 
 
 class Table(Generic[T]):
     """Table specification using custom columns and a source type."""
 
     def __init__(
-        self, name: str, cons: Iterable[Union[Column, Index]], source: Type[T] = None
+        self,
+        name: str,
+        cons: Iterable[Union[Column, Index]],
+        source: Optional[Type[T]] = None,
     ) -> None:
         self._name = name
         self._columns: List[Column] = []
         self._column_names: Set[str] = set()
         self._column_types: Dict[Column, ColumnType] = {}
         self._indexes: List[Index] = []
         self._source: Optional[Type[T]] = source
@@ -102,26 +105,27 @@
 
     def delete(self) -> Query:
         """Shortcut for Query(<table>).delete()"""
         return Query(self).delete()
 
 
 @overload
-def table(cls_or_name: Type[T], *args: Index) -> Table[T]:
-    ...  # pragma: no cover
+def table(cls_or_name: Type[T], *args: Index) -> Table[T]: ...  # pragma: no cover
 
 
 @overload
-def table(cls_or_name: str, *args: Index) -> Callable[[Type[T]], Table[T]]:
-    ...  # pragma: no cover
+def table(
+    cls_or_name: str, *args: Index
+) -> Callable[[Type[T]], Table[T]]: ...  # pragma: no cover
 
 
 @overload
-def table(cls_or_name: Index, *args: Index) -> Callable[[Type[T]], Table[T]]:
-    ...  # pragma: no cover
+def table(
+    cls_or_name: Index, *args: Index
+) -> Callable[[Type[T]], Table[T]]: ...  # pragma: no cover
 
 
 def table(cls_or_name, *args: Index):
     """Simple decorator to generate table spec from annotated class def."""
 
     table_name: Optional[str] = None
     if isinstance(cls_or_name, str):
@@ -139,15 +143,15 @@
 
         cons: List[Union[Column, Index]] = list(args)
         if issubclass(cls, tuple):
             defaults = getattr(cls, "_field_defaults", {})
         else:
             defaults = {
                 k: (NO_DEFAULT if a.default == NOTHING else a.default)
-                for k, a in fields_dict(cls).items()
+                for k, a in fields_dict(cls).items()  # type: ignore
             }
         for key, value in get_type_hints(cls).items():
             cons.append(
                 Column(
                     key,
                     ctype=value,
                     table_name=name,
```

### Comparing `aql-0.4.1/aql/tests/column.py` & `aql-0.5.0/aql/tests/column.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 from typing import List, Optional, Union
 from unittest import TestCase
 
 from aql.column import AutoIncrement, Column, ColumnType, Index, Primary, Unique
 from aql.errors import InvalidColumnType
```

### Comparing `aql-0.4.1/aql/tests/connector.py` & `aql-0.5.0/aql/tests/connector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 from unittest import TestCase
 
 from aql.connector import connect
 from aql.engines.sql import SqlEngine
 from aql.engines.sqlite import SqliteConnection
```

### Comparing `aql-0.4.1/aql/tests/engines/base.py` & `aql-0.5.0/aql/tests/engines/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 from unittest import TestCase
 from unittest.mock import patch
 
 from aql.column import Column
 from aql.engines.base import Engine
```

### Comparing `aql-0.4.1/aql/tests/engines/integration.py` & `aql-0.5.0/aql/tests/engines/integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 from sqlite3 import OperationalError
 
 from aiounittest import AsyncTestCase
 
 import aql
```

### Comparing `aql-0.4.1/aql/tests/engines/mysql.py` & `aql-0.5.0/aql/tests/engines/mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 from datetime import date
 from typing import Optional
 from unittest import TestCase
 
 from aql.column import AutoIncrement, Column, Index, Primary, Unique
```

### Comparing `aql-0.4.1/aql/tests/engines/sql.py` & `aql-0.5.0/aql/tests/engines/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 from unittest import TestCase
 
 from aql.engines.sql import SqlEngine
 from aql.errors import BuildError, UnsafeQuery
 from aql.query import PreparedQuery
```

### Comparing `aql-0.4.1/aql/tests/engines/sqlite.py` & `aql-0.5.0/aql/tests/engines/sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 from datetime import date
 from typing import Optional
 from unittest import TestCase
 
 from aql.column import AutoIncrement, Column, Index, Primary, Unique
```

### Comparing `aql-0.4.1/aql/tests/query.py` & `aql-0.5.0/aql/tests/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 from unittest import TestCase
 
 from aql.column import Column
 from aql.errors import BuildError
 from aql.query import PreparedQuery, Query
@@ -177,15 +177,15 @@
 
         query = Query(Foo).select(Foo.a)
         factory = query.factory()
         self.assertNotEqual(factory, Foo._source)
         self.assertEqual(factory(1), factory(1))
         self.assertEqual(factory(1).a, 1)
         with self.assertRaises(AttributeError):
-            _value = factory(1).b
+            factory(1).b
 
         query = Query(one).select()
         factory = query.factory()
         self.assertEqual(factory(1, 2), factory(1, 2))
         self.assertEqual(factory(1, 2).a, 1)
         self.assertEqual(factory(1, 2).b, 2)
```

### Comparing `aql-0.4.1/aql/tests/table.py` & `aql-0.5.0/aql/tests/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# Copyright 2020 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 from typing import NamedTuple
 from unittest import TestCase
 
 from aql.column import (
-    NO_DEFAULT,
     AutoIncrement,
     Column,
     ColumnType,
     Index,
+    NO_DEFAULT,
     Primary,
     Unique,
 )
 from aql.errors import AqlError, DuplicateColumnName
 from aql.query import Query
 from aql.table import Table, table
 from aql.types import Comparison, Operator, QueryAction
```

### Comparing `aql-0.4.1/aql/types.py` & `aql-0.5.0/aql/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# Copyright 2020 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
-from enum import Enum, IntEnum, auto
+from enum import auto, Enum, IntEnum
 from typing import (
-    TYPE_CHECKING,
     Any,
     Generic,
     List,
     NewType,
     Optional,
     Tuple,
+    TYPE_CHECKING,
     TypeVar,
     Union,
 )
 
-from attr import Factory, dataclass
+from attr import dataclass, Factory
 
 if TYPE_CHECKING:  # pragma: no cover
     from .column import Column
     from .table import Table
 
 T = TypeVar("T")
```

### Comparing `aql-0.4.1/docs/_templates/omnilib.html` & `aql-0.5.0/docs/_templates/omnilib.html`

 * *Files identical despite different names*

### Comparing `aql-0.4.1/docs/conf.py` & `aql-0.5.0/docs/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 
 
 # -- Project information -----------------------------------------------------
 
 import datetime
 
 project = "aql"
-copyright = f"{datetime.date.today().year}, John Reese"
-author = "John Reese"
+copyright = f"{datetime.date.today().year}, Amethyst Reese"
+author = "Amethyst Reese"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    "m2r",
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
+    "sphinx_mdinclude",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
@@ -45,14 +45,15 @@
 
 autodoc_default_options = {
     "show-inheritance": True,
     "members": True,
     "undoc-members": True,
 }
 autodoc_member_order = "groupwise"
+autodoc_typehints = "description"
 
 highlight_language = "python3"
 intersphinx_mapping = {"python": ("https://docs.python.org/3", None)}
 master_doc = "index"
 
 # -- Options for HTML output -------------------------------------------------
```

### Comparing `aql-0.4.1/pyproject.toml` & `aql-0.5.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,54 @@
 [build-system]
 requires = ["flit_core >=2,<4"]
 build-backend = "flit_core.buildapi"
 
-[tool.flit.metadata]
-module = "aql"
-author = "John Reese"
-author-email = "john@noswap.com"
-description-file = "README.md"
-home-page = "https://github.com/omnilib/aql"
-requires = ["attrs"]
-requires-python = ">=3.6"
+[project]
+name = "aql"
+authors = [
+    {name = "Amethyst Reese", email="amethyst@n7.gg"},
+]
+readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: AsyncIO",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development :: Libraries",
 ]
+dynamic = ["version", "description"]
+requires-python = ">=3.8"
+dependencies = [
+    "attrs >= 22",
+]
 
-[tool.flit.metadata.requires-extra]
+[project.optional-dependencies]
 all = ["aiomysql", "aiosqlite"]
 sqlite = ["aiosqlite"]
 mysql = ["aiomysql"]
+dev = [
+    "aiomysql==0.2.0",
+    "aiosqlite==0.20.0",
+    "aiounittest==1.4.2",
+    "attribution==1.7.1",
+    "attrs==23.2.0",
+    "black==24.4.0",
+    "coverage==7.5.0",
+    "flake8==7",
+    "flake8-bugbear==24.4.21",
+    "flit==3.9.0",
+    "mypy==1.9.0",
+    "usort==1.0.8.post1",
+]
+docs = [
+    "sphinx==7.3.7",
+    "sphinx-mdinclude==0.6.0",
+]
 
-[tool.flit.metadata.urls]
+[project.urls]
 Documentation = "https://aql.omnilib.dev/en/latest/"
 Github = "https://github.com/omnilib/aql"
 
 [tool.flit.sdist]
 exclude = [
     ".github/",
 ]
@@ -39,13 +60,13 @@
 
 [tool.coverage.report]
 fail_under = 93
 precision = 1
 show_missing = true
 skip_covered = true
 
-[tool.isort]
-line_length = 88
-multi_line_output = 3
-force_grid_wrap = false
-include_trailing_comma = true
-use_parentheses = true
+[tool.attribution]
+name = "aql"
+package = "aql"
+signed_tags = true
+version_file = true
+ignored_authors = ["dependabot", "pyup.io"]
```

