# Comparing `tmp/sqldatamodel-0.3.9.tar.gz` & `tmp/sqldatamodel-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqldatamodel-0.3.9.tar", last modified: Sat Apr 13 23:09:09 2024, max compression
+gzip compressed data, was "sqldatamodel-0.4.0.tar", last modified: Tue Apr 23 22:06:52 2024, max compression
```

## Comparing `sqldatamodel-0.3.9.tar` & `sqldatamodel-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 23:09:09.971355 sqldatamodel-0.3.9/
--rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 sqldatamodel-0.3.9/LICENSE
--rw-rw-rw-   0        0        0    27267 2024-04-13 23:09:09.961354 sqldatamodel-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0    25395 2024-04-12 01:46:49.000000 sqldatamodel-0.3.9/README.md
--rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 sqldatamodel-0.3.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-13 23:09:09.973357 sqldatamodel-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0     2400 2024-04-13 23:07:32.000000 sqldatamodel-0.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-13 23:09:08.454230 sqldatamodel-0.3.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-13 23:09:09.643783 sqldatamodel-0.3.9/src/SQLDataModel/
--rw-rw-rw-   0        0        0     6899 2024-03-19 22:34:49.000000 sqldatamodel-0.3.9/src/SQLDataModel/ANSIColor.py
--rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 sqldatamodel-0.3.9/src/SQLDataModel/HTMLParser.py
--rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 sqldatamodel-0.3.9/src/SQLDataModel/JSONEncoder.py
--rw-rw-rw-   0        0        0   589857 2024-04-13 23:07:34.000000 sqldatamodel-0.3.9/src/SQLDataModel/SQLDataModel.py
--rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 sqldatamodel-0.3.9/src/SQLDataModel/StandardDeviation.py
--rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 sqldatamodel-0.3.9/src/SQLDataModel/__init__.py
--rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 sqldatamodel-0.3.9/src/SQLDataModel/converters.py
--rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 sqldatamodel-0.3.9/src/SQLDataModel/demo.py
--rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 sqldatamodel-0.3.9/src/SQLDataModel/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-13 23:09:09.862411 sqldatamodel-0.3.9/src/SQLDataModel/extensions/
--rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 sqldatamodel-0.3.9/src/SQLDataModel/extensions/__init__.py
--rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 sqldatamodel-0.3.9/src/SQLDataModel/extensions/str_utils.c
-drwxrwxrwx   0        0        0        0 2024-04-13 23:09:09.953354 sqldatamodel-0.3.9/src/SQLDataModel.egg-info/
--rw-rw-rw-   0        0        0    27267 2024-04-13 23:09:08.000000 sqldatamodel-0.3.9/src/SQLDataModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2024-04-13 23:09:08.000000 sqldatamodel-0.3.9/src/SQLDataModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 23:09:08.000000 sqldatamodel-0.3.9/src/SQLDataModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-13 23:09:08.000000 sqldatamodel-0.3.9/src/SQLDataModel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-13 23:09:09.880410 sqldatamodel-0.3.9/tests/
--rw-rw-rw-   0        0        0    59486 2024-04-13 23:06:52.000000 sqldatamodel-0.3.9/tests/test_Future.py
--rw-rw-rw-   0        0        0    59489 2024-04-13 23:06:53.000000 sqldatamodel-0.3.9/tests/test_SQLDataModel.py
+drwxrwxrwx   0        0        0        0 2024-04-23 22:06:52.990235 sqldatamodel-0.4.0/
+-rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 sqldatamodel-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0    27204 2024-04-23 22:06:52.977437 sqldatamodel-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    25304 2024-04-18 17:59:54.000000 sqldatamodel-0.4.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 sqldatamodel-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 22:06:52.991235 sqldatamodel-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2432 2024-04-23 20:12:46.000000 sqldatamodel-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 22:06:51.583553 sqldatamodel-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-23 22:06:52.758817 sqldatamodel-0.4.0/src/SQLDataModel/
+-rw-rw-rw-   0        0        0     6899 2024-03-19 22:34:49.000000 sqldatamodel-0.4.0/src/SQLDataModel/ANSIColor.py
+-rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 sqldatamodel-0.4.0/src/SQLDataModel/HTMLParser.py
+-rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 sqldatamodel-0.4.0/src/SQLDataModel/JSONEncoder.py
+-rw-rw-rw-   0        0        0   600424 2024-04-23 22:06:16.000000 sqldatamodel-0.4.0/src/SQLDataModel/SQLDataModel.py
+-rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 sqldatamodel-0.4.0/src/SQLDataModel/StandardDeviation.py
+-rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 sqldatamodel-0.4.0/src/SQLDataModel/__init__.py
+-rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 sqldatamodel-0.4.0/src/SQLDataModel/converters.py
+-rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 sqldatamodel-0.4.0/src/SQLDataModel/demo.py
+-rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 sqldatamodel-0.4.0/src/SQLDataModel/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-23 22:06:52.905454 sqldatamodel-0.4.0/src/SQLDataModel/extensions/
+-rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 sqldatamodel-0.4.0/src/SQLDataModel/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 sqldatamodel-0.4.0/src/SQLDataModel/extensions/str_utils.c
+drwxrwxrwx   0        0        0        0 2024-04-23 22:06:52.976028 sqldatamodel-0.4.0/src/SQLDataModel.egg-info/
+-rw-rw-rw-   0        0        0    27204 2024-04-23 22:06:50.000000 sqldatamodel-0.4.0/src/SQLDataModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2024-04-23 22:06:51.000000 sqldatamodel-0.4.0/src/SQLDataModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 22:06:51.000000 sqldatamodel-0.4.0/src/SQLDataModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-23 22:06:51.000000 sqldatamodel-0.4.0/src/SQLDataModel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 22:06:52.920156 sqldatamodel-0.4.0/tests/
+-rw-rw-rw-   0        0        0    59564 2024-04-23 20:10:21.000000 sqldatamodel-0.4.0/tests/test_Future.py
+-rw-rw-rw-   0        0        0    59567 2024-04-23 20:10:35.000000 sqldatamodel-0.4.0/tests/test_SQLDataModel.py
```

### Comparing `sqldatamodel-0.3.9/LICENSE` & `sqldatamodel-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.3.9/PKG-INFO` & `sqldatamodel-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.3.9
+Version: 0.4.0
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
-Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package
+Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package,polars2pandas,pandas2polars
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -262,16 +262,16 @@
 
 # Filter to only 'Future' missions
 sdm = sdm[sdm['Status'] == 'Future']
 
 # Create new column with today's date so it ages better!
 sdm['Updated'] = datetime.date.today()
 
-# Send our table to a new html file, this time without the index
-saturn_html = sdm.to_html('Future-Saturn.html', include_index=False)
+# Create a new html file with our table
+sdm.to_html('Future-Saturn.html', index=False)
 ```
 Here's a snippet from the `Future-Saturn.html` file generated by the `to_html()` method:
 ```html
 <!-- Metadata Removed -->
 <table>
     <tr>
         <th>Mission</th>
@@ -531,15 +531,15 @@
 
   * [`ANSIColor`](https://sqldatamodel.readthedocs.io/en/latest/SQLDataModel.html#SQLDataModel.ANSIColor.ANSIColor) for terminal styling.
   * [`HTMLParser`](https://sqldatamodel.readthedocs.io/en/latest/SQLDataModel.html#SQLDataModel.HTMLParser.HTMLParser) for parsing tabular data from the web.
   * [`JSONEncoder`](https://sqldatamodel.readthedocs.io/en/latest/SQLDataModel.html#SQLDataModel.JSONEncoder.DataTypesEncoder) for type casting and encoding JSON data.
   * [`SQLDataModel`](https://sqldatamodel.readthedocs.io/en/latest/SQLDataModel.html#SQLDataModel.SQLDataModel.SQLDataModel) for wrapping it all up.
 
 
-However, to skip over the less relevant modules and jump straight to the meat of the package, the ``SQLDataModel`` module, click [here](https://sqldatamodel.readthedocs.io/en/latest/SQLDataModel.html#SQLDataModel.SQLDataModel.SQLDataModel). 
+However, to skip over the less relevant modules and jump straight to the meat of the package, the ``SQLDataModel`` module, click [here](https://sqldatamodel.readthedocs.io/en/latest/modules.html). 
 
 ---
 
 ### Motivation
 
 While there are packages/dependencies out there that can accomplish some of the same tasks as `SQLDataModel`, they're either missing key features or end up being overkill for common tasks like grabbing and converting tables from source A to destination B, or they don't quite handle the full process and require additional dependencies to make it all work. When you find yourself doing the same thing over and over again, eventually you sit down and write a package to do it for you.
```

### Comparing `sqldatamodel-0.3.9/README.md` & `sqldatamodel-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -237,16 +237,16 @@
 
 # Filter to only 'Future' missions
 sdm = sdm[sdm['Status'] == 'Future']
 
 # Create new column with today's date so it ages better!
 sdm['Updated'] = datetime.date.today()
 
-# Send our table to a new html file, this time without the index
-saturn_html = sdm.to_html('Future-Saturn.html', include_index=False)
+# Create a new html file with our table
+sdm.to_html('Future-Saturn.html', index=False)
 ```
 Here's a snippet from the `Future-Saturn.html` file generated by the `to_html()` method:
 ```html
 <!-- Metadata Removed -->
 <table>
     <tr>
         <th>Mission</th>
@@ -506,15 +506,15 @@
 
   * [`ANSIColor`](https://sqldatamodel.readthedocs.io/en/latest/SQLDataModel.html#SQLDataModel.ANSIColor.ANSIColor) for terminal styling.
   * [`HTMLParser`](https://sqldatamodel.readthedocs.io/en/latest/SQLDataModel.html#SQLDataModel.HTMLParser.HTMLParser) for parsing tabular data from the web.
   * [`JSONEncoder`](https://sqldatamodel.readthedocs.io/en/latest/SQLDataModel.html#SQLDataModel.JSONEncoder.DataTypesEncoder) for type casting and encoding JSON data.
   * [`SQLDataModel`](https://sqldatamodel.readthedocs.io/en/latest/SQLDataModel.html#SQLDataModel.SQLDataModel.SQLDataModel) for wrapping it all up.
 
 
-However, to skip over the less relevant modules and jump straight to the meat of the package, the ``SQLDataModel`` module, click [here](https://sqldatamodel.readthedocs.io/en/latest/SQLDataModel.html#SQLDataModel.SQLDataModel.SQLDataModel). 
+However, to skip over the less relevant modules and jump straight to the meat of the package, the ``SQLDataModel`` module, click [here](https://sqldatamodel.readthedocs.io/en/latest/modules.html). 
 
 ---
 
 ### Motivation
 
 While there are packages/dependencies out there that can accomplish some of the same tasks as `SQLDataModel`, they're either missing key features or end up being overkill for common tasks like grabbing and converting tables from source A to destination B, or they don't quite handle the full process and require additional dependencies to make it all work. When you find yourself doing the same thing over and over again, eventually you sit down and write a package to do it for you.
```

### Comparing `sqldatamodel-0.3.9/setup.py` & `sqldatamodel-0.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='SQLDataModel',  
-     version='0.3.9',
+     version='0.4.0',
      scripts=['src/SQLDataModel/SQLDataModel.py'] ,
      author='Ante Tonkovic-Capin',
      author_email='antetc@icloud.com',
      description='SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.',
-     keywords=['SQL','ETL','dataframe','terminal tables','pretty print tables','sql2sql','data analysis','data science','data model','extract','transform','load','web scraping tables','data mining','html','html table parsing','apache arrow','pyarrow','pyarrow conversion','pyarrow to table','pyarrow to sql','pyarrow to csv','parquet file parsing','csv','csv parsing','markdown','markdown table parsing','latex','latex table parsing','delimited','delimited data parsing','file conversion','format conversion','terminal styling','table styling','from sqlite','to sqlite','from postgresql','to postgresql','sql to sql','excel','xlsx file','excel to sql','DataFrame package'],
+     keywords=['SQL','ETL','dataframe','terminal tables','pretty print tables','sql2sql','data analysis','data science','data model','extract','transform','load','web scraping tables','data mining','html','html table parsing','apache arrow','pyarrow','pyarrow conversion','pyarrow to table','pyarrow to sql','pyarrow to csv','parquet file parsing','csv','csv parsing','markdown','markdown table parsing','latex','latex table parsing','delimited','delimited data parsing','file conversion','format conversion','terminal styling','table styling','from sqlite','to sqlite','from postgresql','to postgresql','sql to sql','excel','xlsx file','excel to sql','DataFrame package','polars2pandas','pandas2polars'],
      license_file='LICENSE',
      long_description=long_description,
      long_description_content_type='text/markdown',
      url='https://github.com/AnteT/SQLDataModel',
      project_urls = {
         'Documentation':'https://sqldatamodel.readthedocs.io/en/latest/',
         'Source': 'https://github.com/AnteT/SQLDataModel.git'
```

### Comparing `sqldatamodel-0.3.9/src/SQLDataModel/ANSIColor.py` & `sqldatamodel-0.4.0/src/SQLDataModel/ANSIColor.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.3.9/src/SQLDataModel/HTMLParser.py` & `sqldatamodel-0.4.0/src/SQLDataModel/HTMLParser.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.3.9/src/SQLDataModel/JSONEncoder.py` & `sqldatamodel-0.4.0/src/SQLDataModel/JSONEncoder.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.3.9/src/SQLDataModel/SQLDataModel.py` & `sqldatamodel-0.4.0/src/SQLDataModel/SQLDataModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
-import sqlite3, os, csv, sys, datetime, pickle, re, shutil, datetime, json, random
+import sqlite3, os, csv, sys, datetime, pickle, re, shutil, datetime, json, random, urllib.request
 from collections.abc import Generator, Callable, Iterator
 from collections import namedtuple
 from typing import Literal, Any
 from ast import literal_eval
-import urllib.request
+from io import StringIO
 
 from .exceptions import DimensionError, SQLProgrammingError
-from .ANSIColor import ANSIColor
 from .StandardDeviation import StandardDeviation
 from .JSONEncoder import DataTypesEncoder
 from .HTMLParser import HTMLParser
+from .ANSIColor import ANSIColor
 
 try:
     from dateutil.parser import parse as dateparser
     _has_dateutil = True
 except ModuleNotFoundError:
     _has_dateutil = False
     
@@ -263,30 +263,31 @@
         - No additional dependencies are installed with this package, however you will obviously need to have pandas or numpy to create pandas or numpy objects.
         - Use :meth:`SQLDataModel.set_display_color()` to modify the terminal color of the table, by default no color styling is applied.
         - Use :meth:`SQLDataModel.get_supported_sql_connections()` to view supported SQL connection packages, please reach out with any issues or questions, thanks!
 
     """
     __slots__ = ('sql_idx','sql_model','display_max_rows','min_column_width','max_column_width','column_alignment','display_color','display_index','row_count','headers','column_count','static_py_to_sql_map_dict','static_sql_to_py_map_dict','sql_db_conn','display_float_precision','header_master','indicies','dtypes','shape','table_style')
     
-    def __init__(self, data:list[list]=None, headers:list[str]=None, dtypes:dict[str,str]=None, display_max_rows:int=None, min_column_width:int=3, max_column_width:int=38, column_alignment:Literal['dynamic','left','center','right']='dynamic', display_color:str=None, display_index:bool=True, display_float_precision:int=2, infer_types:bool=False, table_style:Literal['ascii','bare','dash','default','double','markdown','outline','pandas','polars','postgresql','round','thick']='default'):
+    def __init__(self, data:list[list]=None, headers:list[str]=None, dtypes:dict[str,str]=None, display_max_rows:int=None, min_column_width:int=3, max_column_width:int=38, column_alignment:Literal['dynamic','left','center','right']='dynamic', display_color:str=None, display_index:bool=True, display_float_precision:int=2, infer_types:bool=False, table_style:Literal['ascii','bare','dash','default','double','list','markdown','outline','pandas','polars','postgresql','round']='default'):
         """
         Initializes a new instance of ``SQLDataModel``.
 
         Parameters:
-            ``data`` (list[list]): The data to populate the model. Should be a list of lists or a list of tuples.
+            ``data`` (list[list]): The data to populate the model. Should be a list of lists or a list of tuples or a dictionary orientated by rows or columns.
             ``headers`` (list[str]): The column headers for the model. If not provided, default headers will be used.
             ``dtypes`` (dict): A dictionary specifying the data types for each column. Format: {'column': 'dtype'}.
             ``display_max_rows`` (int): The maximum number of rows to display. If not provided, all rows will be displayed.
             ``min_column_width`` (int): The minimum width for each column. Default is 3.
             ``max_column_width`` (int): The maximum width for each column. Default is 38.
-            ``column_alignment`` (str): The alignment for columns ('dynamic', 'left', 'center', 'right'). Default is 'dynamic'.
+            ``column_alignment`` (str): The alignment for columns, must be 'dynamic', 'left', 'center' or 'right'). Default is 'dynamic'.
             ``display_color`` (str|tuple|None): The color for display as hex code string or rgb tuple.
             ``display_index`` (bool): Whether to display row indices. Default is True.
             ``display_float_precision`` (int): The number of decimal places to display for float values. Default is 2.
             ``infer_types`` (bool): Whether to infer the data types based on a randomly selected sample. Default is False, using first row to derive the corresponding type.
+            ``table_style`` (str): The styling to use when representing the table, must be 'ascii', 'bare', 'dash', 'default', 'double', 'list', 'markdown', 'outline', 'pandas', 'polars', 'postgresql' or 'round'. Default is 'default'.
 
         Raises:
             ``ValueError``: If ``data`` and ``headers`` are not provided, or if ``data`` is of insufficient length.
             ``TypeError``: If ``data`` or ``headers`` is not a valid type (list or tuple), or if ``dtypes`` is not a dictionary.
             ``DimensionError``: If the length of ``headers`` does not match the implied column count from the data.
             ``SQLProgrammingError``: If there's an issue with executing SQL statements during initialization.
 
@@ -294,15 +295,15 @@
 
             from SQLDataModel import SQLDataModel
 
             # Create sample data
             data = [('Alice', 20, 'F'), ('Bob', 25, 'M'), ('Gerald', 30, 'M')]
 
             # Create the model with custom headers
-            sdm = SQLDataModel(data,headers=['Name','Age','Sex'])
+            sdm = SQLDataModel(data, headers=['Name','Age','Sex'])
             
             # Display the model
             print(model)
 
         ```shell
             ┌────────┬──────┬──────┐
             │ Name   │  Age │ Sex  │
@@ -320,24 +321,24 @@
             - If ``dtypes`` is provided, it must be a dictionary with column names as keys and Python data types as string values, e.g., `{'first_name': 'str', 'weight': 'float'}`
             - If ``infer_types = True`` and ``dtypes`` are provided, the order will be resolved by first inferring the types, then overriding the inferred types for each ``{col:type}`` provided in the ``dtypes`` argument. If one is not provided, then the inferred type will be used as a fallback.
         """
         if data is None:
             if headers is None:
                 if dtypes is None:
                     raise ValueError(
-                        SQLDataModel.ErrorFormat(f"ValueError: insufficient data, an empty header-less model cannot be created, to create a model with zero rows a ``headers`` or ``dtypes`` argument is required")
+                        SQLDataModel.ErrorFormat(f"ValueError: insufficient data, an empty header-less model cannot be created, to create a model with zero rows a `headers` or `dtypes` argument is required")
                     )
                 else:
                     if not isinstance(dtypes,dict):
                         raise TypeError(
-                            SQLDataModel.ErrorFormat(f"TypeError: invalid type '{type(dtypes).__name__}', ``dtypes`` must be of type 'dict' with format of `{{'column':'dtype'}}` where 'dtype' must be a string representing a valid python datatype")
+                            SQLDataModel.ErrorFormat(f"TypeError: invalid type '{type(dtypes).__name__}', `dtypes` must be of type 'dict' with format of `{{'column':'dtype'}}` where 'dtype' must be a string representing a valid python datatype")
                         )
                     headers = list(dtypes.keys())
-            had_data = False
             data = [tuple(None for _ in range(len(headers)))]
+            had_data = False
         else:
             had_data = True
         if not isinstance(data, (list,tuple,dict)) and had_data:  
             raise TypeError(
                 SQLDataModel.ErrorFormat(f"TypeError: type mismatch, '{type(data).__name__}' is not a valid type for data, which must be of type list, tuple or dict")
                 )
         if len(data) < 1 and had_data:
@@ -357,25 +358,19 @@
                         headers = ['idx',*headers]
                     data = [tuple([k,*v]) for k,v in data.items()]
                 else:
                     first_key_val = data[next(iter(data))]
                     if isinstance(first_key_val, dict):
                         inferred_headers = list(data.keys())
                         data = [[data[col][val] for col in inferred_headers] for val in data.keys()]
-                    elif isinstance(first_key_val, (list,tuple)):
-                        inferred_headers = [k for k in data.keys()]
-                        column_count = len(inferred_headers)
-                        row_count = len(first_key_val)
-                        data = [x for x in data.values()]
-                        data = [tuple([data[j][row] for j in range(column_count)]) for row in range(row_count)]
-                        if headers is None:
-                            headers = inferred_headers
-                        else:
-                            if len(headers) + 1 == column_count:
-                                headers = ['idx',*headers]
+                    elif isinstance(first_key_val, (list, tuple)):
+                        inferred_headers = list(data.keys())
+                        data = list(data.values())
+                        data = [tuple(data[j][i] for j in range(len(inferred_headers))) for i in range(len(first_key_val))]
+                        headers = inferred_headers if headers is None else ['idx', *headers] if len(headers) + 1 == len(inferred_headers) else headers
                     else:
                         raise TypeError(
                             SQLDataModel.ErrorFormat(f"TypeError: invalid dict values, received type '{type(first_key_val).__name__}' but expected dict values as one of type 'list', 'tuple' or 'dict'")
                         )
             try:
                 _ = data[0]
             except Exception as e:
@@ -451,15 +446,15 @@
         self.display_color = ANSIColor(display_color) if isinstance(display_color, (str,tuple)) else display_color if isinstance(display_color,ANSIColor) else None
         """``ANSIColor``: The display color to use for string representations of the model. Default is ``None``, using the standard terminal color."""
         self.static_py_to_sql_map_dict = {'None': 'TEXT','int': 'INTEGER','float': 'REAL','str': 'TEXT','bytes': 'BLOB', 'date': 'DATE', 'datetime': 'TIMESTAMP', 'NoneType':'TEXT', 'bool':'INTEGER'}
         """``dict``: The data type mapping to use when converting python types to SQL column types."""
         self.static_sql_to_py_map_dict = {'NULL': 'None','INTEGER': 'int','REAL': 'float','TEXT': 'str','BLOB': 'bytes', 'DATE': 'date', 'TIMESTAMP': 'datetime','':'str'}
         """``dict``: The data type mapping to use when converting SQL column types to python types."""
         self.table_style = table_style
-        """``str``: The table style used for string representations of the model. Available styles are ``'ascii'``, ``'bare'``, ``'dash'``, ``'default'``, ``'double'``, ``'markdown'``, ``'outline'``, ``'pandas'``, ``'polars'``, ``'postgresql'``, ``'round'`` or ``'thick'``. Defaults to ``'default'`` table style."""
+        """``str``: The table style used for string representations of the model. Available styles are ``'ascii'``, ``'bare'``, ``'dash'``, ``'default'``, ``'double'``, ``'list'``, ``'markdown'``, ``'outline'``, ``'pandas'``, ``'polars'``, ``'postgresql'`` or ``'round'``. Defaults to ``'default'`` table style."""
         if infer_types and self.row_count > 0:
             inferred_dtypes = SQLDataModel.infer_types_from_data(input_data=random.sample(data, min(self.row_count, 16)))
             headers_to_py_dtypes_dict = {self.headers[i]:inferred_dtypes[i+dyn_idx_offset] for i in range(self.column_count)}
         else:
             headers_to_py_dtypes_dict = {self.headers[i]:type(data[0][i+dyn_idx_offset]).__name__ for i in range(self.column_count)}        
         if dtypes is not None:
             [(headers_to_py_dtypes_dict.__setitem__(col,dtype)) for col,dtype in dtypes.items() if col in self.headers and dtype in self.static_py_to_sql_map_dict]
@@ -2321,32 +2316,32 @@
                 else:
                     fill_value = ''
         else:
             fill_value = None
         return cls([[fill_value for _ in range(n_cols)] for _ in range(n_rows)])
         
     @classmethod
-    def from_csv(cls, csv_source:str, infer_types:bool=True, encoding:str = "Latin1", delimiters:str = ', \t;|:', quotechar:str = '"', headers:list[str] = None, **kwargs) -> SQLDataModel:
+    def from_csv(cls, csv_source:str, infer_types:bool=True, encoding:str = 'Latin1', delimiter:str = ',', quotechar:str = '"', headers:list[str] = None, **kwargs) -> SQLDataModel:
         """
         Returns a new ``SQLDataModel`` generated from the provided CSV source, which can be either a file path or a raw delimited string.
 
         Parameters:
             ``csv_source`` (str): The path to the CSV file or a raw delimited string.
-            ``infer_types`` (bool, optional): Infer column types based on random subset of data. Default is True, when False, all columns are str type.
-            ``encoding`` (str, optional): The encoding used to decode the CSV source if it is a file. Default is 'Latin1'.
-            ``delimiters`` (str, optional): Possible delimiters. Default is ``\\s``, ``\\t``, ``;``, ``|``, ``:`` or ``,`` (space, tab, semicolon, pipe, colon or comma).
-            ``quotechar`` (str, optional): The character used for quoting fields. Default is ``"``.
+            ``infer_types`` (bool, optional): Infer column types based on random subset of data. Default is ``True``, when False, all columns are str type.
+            ``encoding`` (str, optional): The encoding used to decode the CSV source if it is a file. Default is ``'Latin1'``.
+            ``delimiter`` (str, optional): The delimiter to use when parsing CSV source. Default is ``','``.
+            ``quotechar`` (str, optional): The character used for quoting fields. Default is ``'"'``.
             ``headers`` (List[str], optional): List of column headers. If None, the first row of the CSV source is assumed to contain headers.
             ``**kwargs``: Additional keyword arguments to be passed to the SQLDataModel constructor.
 
         Returns:
             ``SQLDataModel``: The SQLDataModel object created from the provided CSV source.
 
         Raises:
-            ``ValueError``: If no delimiter is found in ``csv_source`` or if parsing with delimiter does not yield valid tabular data.
+            ``ValueError``: If no delimited data is found in ``csv_source`` or if parsing with delimiter does not yield valid tabular data.
             ``Exception``: If an error occurs while attempting to read from or process the provided CSV source.
 
         Examples:
 
         From CSV File
         -------------
 
@@ -2355,26 +2350,27 @@
 
             # CSV file path or raw CSV string
             csv_source = "/path/to/data.csv"
 
             # Create the model using the CSV file, providing custom headers
             sdm = SQLDataModel.from_csv(csv_source, headers=['ID', 'Name', 'Value'])
         ```
-        From Delimited Source
-        ---------------------
+
+        From CSV Literal
+        ----------------
 
         ```python
             from SQLDataModel import SQLDataModel
 
-            # Space delimited data
+            # CSV data
             data = '''
-            A B C
-            1a 1b 1c
-            2a 2b 2c
-            3a 3b 3c
+            A, B, C
+            1a, 1b, 1c
+            2a, 2b, 2c
+            3a, 3b, 3c
             '''
 
             # Create the model
             sdm = SQLDataModel.from_csv(data)
 
             # View result
             print(sdm)
@@ -2389,42 +2385,38 @@
             │ 1a   │ 1b   │ 1c   │
             │ 2a   │ 2b   │ 2c   │
             │ 3a   │ 3b   │ 3c   │
             └──────┴──────┴──────┘
             [3 rows x 3 columns]
         ```
 
+        Change Log:
+            - Version 0.4.0 (2024-04-23):
+                - Modifed to only parse CSV files and removed all delimiter sniffing with introduction of new method :meth:`SQLDataModel.from_delimited()` to handle other delimiters.
+                - Renamed ``delimiters`` parameter to ``delimiter`` with ``,`` set as new default to reflect revised focus on CSV files only.
+
         Note:
-            - If ``csv_source`` is delimited by characters other than those specified, provide the delimiter to ``delimiters``.
+            - If ``csv_source`` is delimited by characters other than those specified, use :meth:`SQLDataModel.from_delimited()` and provide delimiter to ``delimiters``.
             - If ``headers`` are provided, the first row parsed from source will be the first row in the table and not discarded.
-            - This method is called by :meth:`SQLDataModel.from_text()` when source data appears to be delimited instead of SQLDataModel's ``__repr__()``
             - The ``infer_types`` argument can be used to infer the appropriate data type for each column:
+            
                 - If ``infer_types = True``, a random subset of the data will be used to infer the correct type and cast values accordingly
                 - If ``infer_types = False``, values from the first row only will be used to assign types, almost always 'str' when reading from CSV.
         """
         if os.path.exists(csv_source):
             try:
                 with open(csv_source, encoding=encoding) as csvfile:
-                    dialect = csv.Sniffer().sniff(csvfile.read(1024), delimiters=delimiters)
-                    csvfile.seek(0)
-                    delimiter = dialect.delimiter
                     tmp_all_rows = list(csv.reader(csvfile, delimiter=delimiter, quotechar=quotechar))
             except Exception as e:
                 raise Exception(
                     SQLDataModel.ErrorFormat(f"{type(e).__name__}: {e} encountered when trying to open and read from provided `csv_source`")
                 ) from None
         else:
             csv_source = csv_source.strip()
             try:
-                dialect = csv.Sniffer().sniff(csv_source, delimiters=delimiters)
-                delimiter = dialect.delimiter
-                if delimiter is None:
-                    raise ValueError(
-                        SQLDataModel.ErrorFormat(f"ValueError: delimiter not found, ensure `csv_source` contains tabular data delimited by one of ` `, `\t`, `;`, `|`, `:` or `,`" )
-                    )
                 tmp_all_rows = list(csv.reader(csv_source.splitlines(), delimiter=delimiter, quotechar=quotechar))
             except ValueError as e:
                 raise ValueError(
                     SQLDataModel.ErrorFormat(f"{e}") # using existing formatting from validation
                 ) from None
             except Exception as e:
                 raise Exception(
@@ -2531,15 +2523,15 @@
             ,'.html': cls.from_html
             ,'.json': cls.from_json
             ,'.md': cls.from_markdown
             ,'.parquet': cls.from_parquet
             ,'.pkl': cls.from_pickle
             ,'.sdm': cls.from_pickle
             ,'.tex': cls.from_latex
-            ,'.tsv': cls.from_csv
+            ,'.tsv': cls.from_delimited
             ,'.txt': cls.from_text
             ,'.xlsx': cls.from_excel
         }
         if isinstance(data, dict):
             if all(value in ('None','int','float','str','bytes','date','datetime','NoneType','bool') for value in data.values()):
                 return cls(dtypes=data, **kwargs)
             else:
@@ -2602,14 +2594,124 @@
                 return cls.from_pyarrow(data, **kwargs)
             else:
                 raise TypeError(
                     SQLDataModel.ErrorFormat(f"TypeError: unsupported type '{arg_type}', current supported external types are 'numpy.ndarray' or 'pandas.DataFrame' objects")
                 )
     
     @classmethod
+    def from_delimited(cls, source:str, infer_types:bool=True, encoding:str='Latin1', delimiters:str=', \t;|:', quotechar:str='"', headers:list[str]=None, **kwargs) -> SQLDataModel:
+        """
+        Returns a new ``SQLDataModel`` generated from the provided delimited source, which can be either a file path or a raw delimited string.
+
+        Parameters:
+            ``source`` (str): The path to the delimited file or a raw delimited string.
+            ``infer_types`` (bool, optional): Infer column types based on random subset of data. Default is True, when False, all columns are str type.
+            ``encoding`` (str, optional): The encoding used to decode the source if it is a file. Default is ``'Latin1'``.
+            ``delimiters`` (str, optional): Possible delimiters. Default is ``\\s``, ``\\t``, ``;``, ``|``, ``:`` or ``,`` (space, tab, semicolon, pipe, colon or comma).
+            ``quotechar`` (str, optional): The character used for quoting fields. Default is ``'"'``.
+            ``headers`` (list[str], optional): List of column headers. If None, the first row of the delimited source is assumed to be the header row.
+            ``**kwargs``: Additional keyword arguments to be passed to the SQLDataModel constructor.
+
+        Returns:
+            ``SQLDataModel``: The SQLDataModel object created from the provided CSV source.
+
+        Raises:
+            ``ValueError``: If no delimiter is found in ``source`` or if parsing with delimiter does not yield valid tabular data.
+            ``Exception``: If an error occurs while attempting to read from or process the provided CSV source.
+
+        Example:
+
+        From Delimited Literal
+        ----------------------
+
+        ```python            
+            from SQLDataModel import SQLDataModel
+
+            # Space delimited literal
+            source_data = '''
+            Name Age Height
+            Beth 27 172.4
+            Kate 28 162.0
+            John 30 175.3
+            Will 35 185.8'''
+
+            # Create the model
+            sdm = SQLDataModel.from_delimited(source_data)
+
+            # View output
+            print(sdm)
+        ```
+
+        This will output:
+
+        ```shell
+            ┌──────┬─────┬─────────┐
+            │ Name │ Age │  Height │
+            ├──────┼─────┼─────────┤
+            │ Beth │  27 │  172.40 │
+            │ Kate │  28 │  162.00 │
+            │ John │  30 │  175.30 │
+            │ Will │  35 │  185.80 │
+            └──────┴─────┴─────────┘
+            [4 rows x 3 columns]
+        ```
+
+        From Delimited File
+        -------------------
+
+        ```python            
+            from SQLDataModel import SQLDataModel
+
+            # Tab separated file
+            tsv_file = 'persons.tsv'
+
+            # Create the model
+            sdm = SQLDataModel.from_delimited(tsv_file)
+        ```
+
+        Note:
+            - Use :meth:`SQLDataModel.from_csv()` if delimiter in source is already known and available as this method requires more compute to determine a plausible delimiter.
+            - Use :meth:`SQLDataModel.from_text()` if data is not delimited but is a string representation such as an ASCII table or the output from another ``SQLDataModel`` instance.
+            - If file is delimited by delimiters other than the default targets ``\\s``, ``\\t``, ``;``, ``|``, ``:`` or ``,`` (space, tab, semicolon, pipe, colon or comma) make sure they are provided as single character values to ``delimiters``.
+        """
+        if os.path.exists(source):
+            try:
+                with open(source, 'r', encoding=encoding) as f:
+                    source = f.read()
+            except Exception as e:
+                raise Exception (
+                    SQLDataModel.ErrorFormat(f"{type(e).__name__}: {e} encountered when trying to open and read from provided `source`")
+                ) from None   
+        else:
+            source = source.strip()
+        try:
+            dialect = csv.Sniffer().sniff(source, delimiters=delimiters)
+            delimiter = dialect.delimiter
+            if delimiter is None:
+                raise ValueError(
+                    SQLDataModel.ErrorFormat(f"ValueError: delimiter not found, ensure `source` contains data delimited by one of ` `, `\\t`, `;`, `|`, `:` or `,` or provide additional delimiters to search for" )
+                )
+            tmp_all_rows = list(csv.reader(source.splitlines(), delimiter=delimiter, quotechar=quotechar, skipinitialspace=True))
+        except ValueError as e:
+            raise ValueError(
+                SQLDataModel.ErrorFormat(f"{e}") # using existing formatting from validation
+            ) from None
+        except Exception as e:
+            raise Exception(
+                SQLDataModel.ErrorFormat(f"{type(e).__name__}: {e} encountered when trying to parse the provided delimited string literal")
+            ) from None
+        if not tmp_all_rows:
+            raise ValueError(
+                SQLDataModel.ErrorFormat(f"ValueError: no delimited tabular data found in provided `source`, ensure content contains delimited tabular data")
+            )
+        if headers is None:
+            headers = tmp_all_rows.pop(0)
+        return cls(data=tmp_all_rows, headers=headers, infer_types=infer_types, **kwargs)          
+
+    @classmethod
     def from_dict(cls, data:dict|list, **kwargs) -> SQLDataModel:
         """
         Create a new ``SQLDataModel`` instance from the provided dictionary.
 
         Parameters:
             ``data`` (dict): The dictionary or list of dictionaries to convert to SQLDataModel. If keys are of type int, they will be used as row indexes; otherwise, keys will be used as headers.
             ``**kwargs``: Additional arguments to be passed to the SQLDataModel constructor.
@@ -4144,16 +4246,17 @@
             text_source = "/path/to/tabular_data.txt"
 
             # Create the model using the text source
             sdm = SQLDataModel.from_text(text_source, table_identifier=2)
 
         Note:
             - This method is made for parsing ``SQLDataModel`` formatted text, such as the kind generated with ``print(sdm)`` or the output created by the inverse method :meth:`SQLDataModel.to_text()`
-            - For parsing other delimited tabular data, this method calls the related :meth:`SQLDataModel.from_csv()` method, which parses tabular data constructed with common delimiters.
-
+            - For parsing delimited tabular data, this method calls :meth:`SQLDataModel.from_delimited()` method, which parses tabular data constructed with common delimiters.
+            - For parsing delimited tabular data when the delimiter is known, use :meth:`SQLDataModel.from_csv()` and provide the delimiter to use for parsing output.
+            - See :meth:`SQLDataModel.to_text()` for converting ``SQLDataModel`` to textual representation or for styling output.
         """
         if not isinstance(text_source, str):
             raise TypeError(
                 SQLDataModel.ErrorFormat(f"TypeError: invalid type '{type(text_source).__name__}', expected `text_source` to be of type 'str', representing a tabular data filepath or tabular string literal")
             )
         if not isinstance(table_identifier, int):
             raise TypeError(
@@ -4170,15 +4273,15 @@
             except Exception as e:
                 raise Exception (
                     SQLDataModel.ErrorFormat(f"{type(e).__name__}: {e} encountered when trying to open and read from provided `text_source`")
                 ) from None                  
         tables = re.findall(r'┌.*?┘', text_source, re.DOTALL)
         if not tables:
             try:
-                return SQLDataModel.from_csv(text_source,headers=headers, **kwargs)
+                return SQLDataModel.from_delimited(text_source, headers=headers, **kwargs)
             except Exception:
                 raise ValueError(
                     SQLDataModel.ErrorFormat("ValueError: no tabular data found in `text_source`, confirm correct filepath or that provided content contains valid tabular data")
                 )
         if table_identifier > len(tables):
             raise IndexError(
                 SQLDataModel.ErrorFormat(f"IndexError: found '{len(tables)}' tables in `text_source`, however none were found at provided `table_identifier` index '{table_identifier}'")
@@ -4326,24 +4429,25 @@
         data = res.fetchall()
         if (len(data) == 1) and (not include_headers): # if only single row
             data = data[0]
         if len(data) == 1: # if only single cell
             data = data[0]
         return [tuple(x[0] for x in res.description),*data] if include_headers else data
 
-    def to_csv(self, filename:str=None, delimiter:str=',', quotechar:str='"', lineterminator:str='\r\n', index:bool=False, **kwargs) -> str|None:
+    def to_csv(self, filename:str=None, delimiter:str=',', quotechar:str='"', lineterminator:str='\r\n', na_rep:str='None', index:bool=False, **kwargs) -> str|None:
         """
         Writes ``SQLDataModel`` to the specified file if ``filename`` argument if provided, otherwise returns the model directly as a CSV formatted string literal.
 
         Parameters:
-            ``filename`` (str): The name of the CSV file to which the data will be written. Default is None, returning as raw literal.
-            ``delimiter`` (str, optional): The delimiter to use for separating values. Default is ','.
-            ``quotechar`` (str, optional): The character used to quote fields. Default is '"'.
-            ``lineterminator`` (str, optional): The character used to terminate the row and move to a new line. Default is '\\r\\n'.
-            ``index`` (bool, optional): If True, includes the index in the CSV file; if False, excludes the index. Default is False.
+            ``filename`` (str): The name of the CSV file to which the data will be written. Default is ``None``, returning as raw literal.
+            ``delimiter`` (str, optional): The delimiter to use for separating values. Default is ``','``.
+            ``quotechar`` (str, optional): The character used to quote fields. Default is ``'"'``.
+            ``lineterminator`` (str, optional): The character used to terminate the row and move to a new line. Default is ``'\\r\\n'``.
+            ``na_rep`` (str, optional): String representation to use for null or missing values. Default is ``'None'``.
+            ``index`` (bool, optional): If True, includes the index in the CSV file; if False, excludes the index. Default is ``False``.
             ``**kwargs``: Additional arguments to be passed to the ``csv.writer`` constructor.
 
         Returns:
             ``str`` | ``None``: If ``filename`` is None, returns the model as a delimited string literal, ``None`` if ``filename`` is provided, writing the model to the specified file as a CSV file.
 
         Example:
 
@@ -4375,14 +4479,15 @@
 
         ```shell
             Name    Age     Height
             John    30      175.3
             Alice   28      162.0
             Travis  35      185.8
         ```
+
         Write to File
         -------------
 
         ```python            
             from SQLDataModel import SQLDataModel
 
             # Sample data
@@ -4398,42 +4503,53 @@
 
             # CSV filename
             csv_file = 'persons.csv'
 
             # Write to the file, keeping the index
             sdm.to_csv(filename=csv_file, index=True)
         ```
-        Contents of ``persons.csv``
+
+        Contents of ``persons.csv``:
 
         ```shell
             idx,Name,Age,Height
             0,John,30,175.3
             1,Alice,28,162.0
             2,Travis,35,185.8
         ```
         
         Change Log:
+            - Version 0.4.0 (2024-04-23):
+                - Modified quoting behavior to avoid redundant quoting and to closely mimic csv module from standard library.
+                - Added ``na_rep`` to fill null or missing values when generating output, useful for space delimited data and minimal quoting.
+                
             - Version 0.3.0 (2024-03-31):
                 - Renamed ``include_index`` parameter to ``index`` for package consistency.
 
         Note:
-            - Modifying ``delimiter`` affects how the data is delimited when writing to ``filename`` and when returning as raw literal.
             - When ``index=True``, the ``sdm_index`` property determines the column name of the index in the result.
+            - Modifying ``delimiter`` affects how the data is delimited when writing to ``filename`` and when returning as raw literal, any valid delimiter can be used.
+            - Quoting behavior can be modified by providing an additional keywork arg such as ``quoting=1`` to wrap all values in quotes, or ``quoting=2`` to quote only non-numeric values, see ``csv.QUOTE_X`` enums for all options.
+            - Use :meth:`SQLDataModel.to_text()` to pretty print table in specified style for visualizing output if strict delimiting is unnecessary.
+            - See :meth:`SQLDataModel.from_csv()` for creating a new ``SQLDataModel`` from existing CSV data
         """
-        res = self.sql_db_conn.execute(self._generate_sql_stmt(index=index))
+        res = self.sql_db_conn.execute(self._generate_sql_stmt(index=index, na_rep=na_rep))
         headers = [x[0] for x in res.description]
         if filename is not None:
             with open(filename, 'w', newline='') as file:
-                csvwriter = csv.writer(file,delimiter=delimiter,lineterminator=lineterminator,quotechar=quotechar,quoting=csv.QUOTE_MINIMAL, **kwargs)
+                csvwriter = csv.writer(file,delimiter=delimiter,lineterminator=lineterminator,quotechar=quotechar,**kwargs)
                 csvwriter.writerow(headers)
                 csvwriter.writerows(res.fetchall())
             return
         else:
-            csv_repr = lineterminator.join([delimiter.join([f'''{quotechar}{col}{quotechar}''' for col in headers]),*[delimiter.join([f'''{quotechar}{cell}{quotechar}''' for cell in row]) for row in res.fetchall()]])
-            return csv_repr
+            csv_repr = StringIO()
+            csv_writer = csv.writer(csv_repr,delimiter=delimiter,lineterminator=lineterminator,quotechar=quotechar,**kwargs)
+            csv_writer.writerow(headers)
+            csv_writer.writerows(res.fetchall())
+            return csv_repr.getvalue().strip()
 
     def to_dict(self, orient:Literal["rows","columns","list"]="rows", index:bool=None) -> dict|list[dict]:
         """
         Converts the ``SQLDataModel`` instance to a dictionary or a list of dictionaries based on the specified orientation.
 
         Parameters:
             ``orient`` (Literal["rows", "columns", "list"]): The orientation of the output, see examples for more detail. ``"rows"``: Returns a dictionary with index values as keys and row values as values. ``"columns"``: Returns a dictionary with column names as keys and column values as tuples. ``"list"``: Returns a list of dictionaries, where each dictionary represents a row.
@@ -5948,25 +6064,27 @@
         except Exception as e:
             con.rollback()
             raise SQLProgrammingError (
                 SQLDataModel.ErrorFormat(f"SQLProgrammingError: {e} encountered when trying to insert model data into provided connection")
             ) from None   
         return
 
-    def to_text(self, filename:str=None, index:bool=None, min_column_width:int=None, max_column_width:int=None, float_precision:int=None, column_alignment:Literal['dynamic', 'left', 'center', 'right']=None) -> str|None:
+    def to_text(self, filename:str=None, index:bool=None, min_column_width:int=None, max_column_width:int=None, float_precision:int=None, column_alignment:Literal['dynamic', 'left', 'center', 'right']=None, table_style:Literal['ascii','bare','dash','default','double','list','markdown','outline','pandas','polars','postgresql','round']=None, display_dimensions:bool=False) -> str|None:
         """
         Returns a textual representation of the current ``SQLDataModel`` as a string literal or by writing to file if a ``filename`` is provided.
 
         Parameters:
             ``filename`` (str, optional): The name of the file to write the text content. If provided, writes the text to the specified file. Default is None.
             ``index`` (bool, optional): Whether to include the index column in the text output. Default is value set on :py:attr:`SQLDataModel.display_index`.
             ``min_column_width`` (int, optional): The minimum column width for table cells. Default is value set on :py:attr:`SQLDataModel.min_column_width`.
             ``max_column_width`` (int, optional): The maximum column width for table cells. Default is value set on :py:attr:`SQLDataModel.max_column_width`.
             ``float_precision`` (int, optional): The precision for floating-point values. Default is value set on :py:attr:`SQLDataModel.display_float_precision`.
             ``column_alignment`` (Literal['dynamic', 'left', 'center', 'right'], optional): The alignment for table columns. Default is value set on :py:attr:`SQLDataModel.column_alignment`. Use ``'dynamic'`` dynamically aligns column content, right for numeric types and left for remaining types. Use ``'left'`` left-aligns all column content. Use ``'center'`` center-aligns all column content. Use ``'right'`` right-aligns all column content.
+            ``table_style`` (Literal['ascii','bare','dash','default','double','list','markdown','outline','pandas','polars','postgresql','round'], optional): The table styling to use. Default is value set on :py:attr:`SQLDataModel.table_style`.
+            ``display_dimensions`` (bool, optional): Whether to include the model dimensions ``[N rows x N cols]`` in the text output. Default is False.
 
         Raises:
             ``TypeError``: If arguments are provided but are not the correct types: ``filename`` (str), ``index`` (bool), ``min_column_width`` (int), ``max_column_width`` (int), ``float_precision`` (int).
             ``ValueError``: If the ``column_alignment`` argument is provided and is not one of 'dynamic', 'left', 'center', or 'right'.
             ``Exception``: If there is an OS related error encountered when opening or writing to the provided ``filename``.
 
         Returns:
@@ -6039,26 +6157,34 @@
             ├───┼─────────┼──────┼────────┤
             │ 0 │  John   │  30  │ 175.3  │
             │ 1 │  Alice  │  28  │ 162.0  │
             │ 2 │ Michael │  35  │ 185.8  │
             └───┴─────────┴──────┴────────┘
         ```
         
+        Important:
+            Unlike output from ``print(sdm)`` or other calls to :meth:`SQLDataModel.__repr__()`, the output from this method includes the full ``SQLDataModel`` and is not restricted by current terminal size or the value set at :py:attr:`SQLDataModel.display_max_rows`. As such, horizontal truncation only occurs on cell values as determined by ``max_column_width`` and no other horizontal or vertical table-wide truncation is performed.
+
         Change Log:
+            - Version 0.3.10 (2024-04-16):
+                - Added ``table_style`` parameter and updated output to reflect new formatting styles introduced in version 0.3.9.
+                - Added ``display_dimensions`` parameter to allow toggling display of table dimensions in output.
+
             - Version 0.3.0 (2024-03-31):
                 - Renamed ``include_index`` parameter to ``index`` for package consistency.
 
         Note:
+            - See :meth:`SQLDataModel.set_table_style()` for modifying table format and available styles.
             - If ``filename`` is provided, the method writes the text to the specified file; otherwise, it returns the textual representation as a string.
-            - If ``index`` is ``None``, the method uses the current value on :py:attr:`display_index`.
-            - If ``min_column_width`` is ``None``, the method uses the current value on :py:attr:`min_column_width`.
-            - If ``max_column_width`` is ``None``, the method uses the current value on :py:attr:`max_column_width`.
-            - If ``float_precision`` is ``None``, the method uses the current value on :py:attr:`display_float_precision`.
-            - If ``column_alignment`` is ``None``, the method uses the current value on :py:attr:`column_alignment`.
-
+            - If ``index`` is ``None``, the method uses the current value on :py:attr:`SQLDataModel.display_index`.
+            - If ``min_column_width`` is ``None``, the method uses the current value on :py:attr:`SQLDataModel.min_column_width`.
+            - If ``max_column_width`` is ``None``, the method uses the current value on :py:attr:`SQLDataModel.max_column_width`.
+            - If ``float_precision`` is ``None``, the method uses the current value on :py:attr:`SQLDataModel.display_float_precision`.
+            - If ``column_alignment`` is ``None``, the method uses the current value on :py:attr:`SQLDataModel.column_alignment`.
+            - If ``table_style`` is ``None``, the method uses the current value on :py:attr:`SQLDataModel.table_style`.
         """        
         if not isinstance(filename, str) and filename is not None:
             raise TypeError(
                 SQLDataModel.ErrorFormat(f"TypeError: invalid type '{type(filename).__name__}', expected `filename` to be of type 'str' representing a valid file path to write text")
             )
         if not isinstance(index, bool) and index is not None:
             raise TypeError(
@@ -6076,58 +6202,76 @@
             raise TypeError(
                 SQLDataModel.ErrorFormat(f"TypeError: invalid type '{type(float_precision).__name__}', expected `float_precision` to be of type 'int' representing precision to use for values of type 'float'")
             )          
         if (column_alignment is not None) and (column_alignment not in ('dynamic', 'left', 'center', 'right')):
             raise ValueError(
                 SQLDataModel.ErrorFormat(f"ValueError: invalid value '{column_alignment}', argument for `column_alignment` must be one of 'dynamic', 'left', 'center', 'right' representing column alignment for text output")
             )
-        index = self.display_index if index is None else index
-        min_column_width = self.min_column_width if min_column_width is None else min_column_width
+        if (table_style is not None) and (table_style not in ('ascii','bare','dash','default','double','list','markdown','outline','pandas','polars','postgresql','round')):
+            raise ValueError(
+                SQLDataModel.ErrorFormat(f"ValueError: invalid value '{table_style}', argument for `table_style` must be one of 'ascii', 'bare', 'dash', 'default', 'double', 'list', 'markdown', 'outline', 'pandas', 'polars', 'postgresql' or 'round'")
+            )
+        display_index = self.display_index if index is None else index
+        min_column_width = self.min_column_width  if min_column_width is None else min_column_width
         max_column_width = self.max_column_width if max_column_width is None else max_column_width
         max_column_width = max_column_width if max_column_width >= 2 else 2 # minimum required width
-        float_precision = self.display_float_precision if float_precision is None else float_precision
+        display_float_precision = self.display_float_precision if float_precision is None else float_precision
         column_alignment = self.column_alignment if column_alignment is None else column_alignment
         column_alignment = None if column_alignment == 'dynamic' else '<' if column_alignment == 'left' else '^' if column_alignment == 'center' else '>'
-        display_headers = [self.sql_idx,*self.headers] if index else self.headers
+        display_headers = [self.sql_idx,*self.headers] if display_index else self.headers
+        table_style = self.table_style if table_style is None else table_style
+        table_format = self._generate_table_style(style=table_style)
+        top_lh, top_hbar, top_sep, top_rh = table_format[0]
+        mid_lh, mid_hbar, mid_sep, mid_rh = table_format[1]
+        row_lh, row_sep, row_rh = table_format[2]
+        low_lh, low_hbar, low_sep, low_rh = table_format[3]
+        table_repr = """""" # big things...
+        table_bare_newline = """\n"""
+        display_max_rows = self.row_count
         header_py_dtype_dict = {col:cmeta[1] for col, cmeta in self.header_master.items()}
-        header_printf_modifiers_dict = {col:(f"'% .{float_precision}f'" if dtype == 'float' else "'% d'" if dtype == 'int' else "'%!s'" if dtype != 'bytes' else "'b''%!s'''") for col,dtype in header_py_dtype_dict.items()}
-        headers_sub_select = " ".join(("select",f"""max(length("{self.sql_idx}")) as "{self.sql_idx}",""" if index else "",",".join([f"""max(max(length(printf({header_printf_modifiers_dict[col]},"{col}"))),length('{col}')) as "{col}" """ for col in display_headers if col != self.sql_idx]),f'from "{self.sql_model}" order by "{self.sql_idx}" asc'))
+        header_printf_modifiers_dict = {col:(f"'% .{display_float_precision}f'" if dtype == 'float' else "'%!s'" if dtype != 'bytes' else "'b''%!s'''") for col,dtype in header_py_dtype_dict.items()}
+        headers_sub_select = " ".join(("select",f"""max(length("{self.sql_idx}")) as "{self.sql_idx}",""" if display_index else "",",".join([f"""max(max(length(printf({header_printf_modifiers_dict[col]},"{col}"))),length('{col}')) as "{col}" """ for col in display_headers if col != self.sql_idx]),f'from "{self.sql_model}" order by "{self.sql_idx}" asc'))
         headers_parse_lengths_select = " ".join(("select",",".join([f"""min(max(ifnull("{col}",length('{col}')),{min_column_width}),{max_column_width})""" if col != self.sql_idx else f"""ifnull("{col}",1)""" for col in display_headers]),"from"))
         headers_full_select = f"""{headers_parse_lengths_select}({headers_sub_select})"""
         length_meta = self.sql_db_conn.execute(headers_full_select).fetchone()
         header_length_dict = {display_headers[i]:width for i, width in enumerate(length_meta)}
-        txt_repr = """""" # big things...
-        table_left_edge = """│ """
-        table_right_edge = """ │"""
-        table_bare_newline = """\n"""
-        vconcat_column_separator = """|| ' │ ' ||"""
-        fetch_idx = SQLDataModel.sqlite_printf_format(self.sql_idx,"index",header_length_dict[self.sql_idx]) + vconcat_column_separator if index else ""
-        header_fmt_str = vconcat_column_separator.join([f"""{SQLDataModel.sqlite_printf_format(col,header_py_dtype_dict[col],header_length_dict[col],float_precision,alignment=column_alignment)}""" for col in display_headers if col != self.sql_idx])
-        fetch_fmt_stmt = f"""select '{table_left_edge}' || {fetch_idx}{header_fmt_str}||' │{table_bare_newline}' as "_full_row" from "{self.sql_model}" order by "{self.sql_idx}" asc"""
+        table_dynamic_newline = """\n"""
+        row_sep_concat = f"""|| '{row_sep}' ||"""
+        fetch_idx = SQLDataModel.sqlite_printf_format(self.sql_idx,"index",header_length_dict[self.sql_idx]) + row_sep_concat if display_index else ""
+        header_fmt_str = row_sep_concat.join([f"""{SQLDataModel.sqlite_printf_format(col,header_py_dtype_dict[col],header_length_dict[col],display_float_precision,alignment=column_alignment)}""" for col in display_headers if col != self.sql_idx])
+        fetch_fmt_stmt = f"""select '{row_lh}' || {fetch_idx}{header_fmt_str}||'{row_rh}{table_dynamic_newline}' as "_full_row" from "{self.sql_model}" order by "{self.sql_idx}" asc limit {display_max_rows}"""
         formatted_response = self.sql_db_conn.execute(fetch_fmt_stmt)
         if column_alignment is None: # dynamic alignment
             formatted_headers = [f"""{(col if len(col) <= header_length_dict[col] else f"{col[:(header_length_dict[col]-2)]}⠤⠄"):{'>' if header_py_dtype_dict[col] in ('int','float') else '<'}{header_length_dict[col]}}""" if col != self.sql_idx else f"""{' ':>{header_length_dict[col]}}"""for col in display_headers]
         else: # left, center, right alignment
             formatted_headers = [(f"""{col:{column_alignment}{header_length_dict[col]}}""" if len(col) <= header_length_dict[col] else f"""{col[:(header_length_dict[col]-2)]}⠤⠄""") if col != self.sql_idx else f"""{' ':>{header_length_dict[col]}}"""for col in display_headers]
-        table_cross_bar = """┌─""" + """─┬─""".join(["""─""" * header_length_dict[col] for col in display_headers]) + """─┐""" + table_bare_newline
-        txt_repr = "".join([txt_repr, table_cross_bar])
-        txt_repr = "".join([txt_repr, table_left_edge + """ │ """.join(formatted_headers) + table_right_edge + table_bare_newline])
-        txt_repr = "".join([txt_repr, table_cross_bar.replace("┌","├").replace("┬","┼").replace("┐","┤")])
-        txt_repr = "".join([txt_repr,*[row[0] for row in formatted_response]])
-        txt_repr = "".join([txt_repr, table_cross_bar.replace("┌","└").replace("┬","┴").replace("┐","┘")]).strip()
+        col_lengths = [val for val in header_length_dict.values()]
+        table_top_bar = "".join([top_lh, top_sep.join([top_hbar * length for length in col_lengths]), top_rh, table_bare_newline])
+        table_top_bar = table_top_bar if len(table_top_bar.strip()) >=1 else """"""
+        table_repr = "".join([table_repr, table_top_bar])
+        table_repr = "".join([table_repr, row_lh, row_sep.join(formatted_headers), row_rh, table_dynamic_newline])
+        table_mid_bar = "".join([mid_lh, mid_sep.join([mid_hbar * length for length in col_lengths]), mid_rh, table_bare_newline])
+        table_mid_bar = table_mid_bar if len(table_mid_bar.strip()) >=1 else """"""
+        table_repr = "".join([table_repr, table_mid_bar])
+        table_repr = "".join([table_repr,*[row[0] for row in formatted_response]])
+        table_low_bar = "".join([low_lh, low_sep.join([low_hbar * length for length in col_lengths]), low_rh, table_bare_newline])
+        table_low_bar = table_low_bar if len(table_low_bar.strip()) >=1 else """"""
+        table_repr = "".join([table_repr, table_low_bar])
+        table_caption = f"""[{self.row_count} rows x {self.column_count} columns]""" if display_dimensions else """"""
+        table_repr = "".join([table_repr, table_caption]).rstrip()
         if filename is not None:
             try:
                 with open(filename, "w", encoding='utf-8') as f:
-                    f.write(txt_repr)
+                    f.write(table_repr)
             except Exception as e:
                 raise Exception (
                     SQLDataModel.ErrorFormat(f"{type(e).__name__}: {e} encountered when trying to open and write text to '{filename}'")
                 ) from None
         else:
-            return txt_repr 
+            return table_repr 
 
     def to_local_db(self, db:str=None) -> None:
         """
         Stores the ``SQLDataModel`` internal in-memory database to a local disk database.
 
         Parameters:
             ``db`` (str, optional): The filename or path of the target local disk database. If ``None``, the current filename will be used as a default target.
@@ -7510,23 +7654,23 @@
 
         ```shell        
             1000
         ```
         """        
         return self.row_count
 
-    def set_table_style(self, style:Literal['ascii','bare','dash','default','double','markdown','outline','pandas','polars','postgresql','round','thick']='default') -> None:
+    def set_table_style(self, style:Literal['ascii','bare','dash','default','double','list','markdown','outline','pandas','polars','postgresql','round']='default') -> None:
         """
         Sets the table style used for string representations of ``SQLDataModel``.
         
         Parameters:
-            ``style`` (Literal['ascii','bare','dash','default','double','markdown','outline','pandas','polars','postgresql','round','thick']): The table styling to set, use ``'default'`` for original style.
+            ``style`` (Literal['ascii','bare','dash','default','double','list','markdown','outline','pandas','polars','postgresql','round']): The table styling to set, use ``'default'`` for original style.
 
         Raises:
-            ``ValueError``: If ``style`` provided is not one of the currently supported options 'ascii','bare','dash','default','double','markdown','outline','pandas','polars','postgresql','round' or 'thick'.
+            ``ValueError``: If ``style`` provided is not one of the currently supported options 'ascii','bare','dash','default','double','list','markdown','outline','pandas','polars','postgresql' or 'round'.
         
         Returns:
             ``None``
 
         Examples::
 
             from SQLDataModel import SQLDataModel
@@ -7608,14 +7752,25 @@
             │ Alice │  28 │  162.08 │ 1996-11-20 │
             │ Bobby │  30 │  175.36 │ 1994-06-15 │
             │ Craig │  37 │  185.82 │ 1987-01-07 │
             │ David │  32 │  179.75 │ 1992-12-28 │
             └───────┴─────┴─────────┴────────────┘
             [4 rows x 4 columns]
         ```        
+        
+        Set ``style = 'list'`` to format ``SQLDataModel`` as a list of values, similar to the SQLite CLI representation:
+
+        ```shell
+            Name   Age   Height  Birthday  
+            -----  ---  -------  ----------
+            Alice   28   162.08  1996-11-20
+            Bobby   30   175.36  1994-06-15
+            Craig   37   185.82  1987-01-07
+            David   32   179.75  1992-12-28
+        ```
 
         Set ``style = 'double'`` to format ``SQLDataModel`` using double line borders:
 
         ```shell
             ╔═══════╦═════╦═════════╦════════════╗
             ║ Name  ║ Age ║  Height ║ Birthday   ║
             ╠═══════╬═════╬═════════╬════════════╣
@@ -7679,35 +7834,26 @@
             Name  | Age |  Height | Birthday
             ------+-----+---------+-----------
             Alice |  28 |  162.08 | 1996-11-20
             Bobby |  30 |  175.36 | 1994-06-15
             Craig |  37 |  185.82 | 1987-01-07
             David |  32 |  179.75 | 1992-12-28
         ```
-
-        Set ``style = 'thick'`` to format ``SQLDataModel`` using thick borders:
-
-        ```shell
-            ┏━━━━━━━┳━━━━━┳━━━━━━━━━┳━━━━━━━━━━━━┓
-            ┃ Name  ┃ Age ┃  Height ┃ Birthday   ┃
-            ┣━━━━━━━╋━━━━━╋━━━━━━━━━╋━━━━━━━━━━━━┫
-            ┃ Alice ┃  28 ┃  162.08 ┃ 1996-11-20 ┃
-            ┃ Bobby ┃  30 ┃  175.36 ┃ 1994-06-15 ┃
-            ┃ Craig ┃  37 ┃  185.82 ┃ 1987-01-07 ┃
-            ┃ David ┃  32 ┃  179.75 ┃ 1992-12-28 ┃
-            ┗━━━━━━━┻━━━━━┻━━━━━━━━━┻━━━━━━━━━━━━┛
-        ```
+        
+        Change Log:
+            - Version 0.3.11 (2024-04-18):
+                - Removed ``'thick'`` style and added ``'list'`` style for greater variety of available formats.
 
         Note:
             - The labels given to certain styles are entirely subjective and do not in any way express original design or ownership of the styling used.
             - Legacy character sets on older terminals may not support all the character encodings required for some styles.
         """
-        if style not in ('ascii','bare','dash','default','double','markdown','outline','pandas','polars','postgresql','round','thick'):
+        if style not in ('ascii','bare','dash','default','double','list','markdown','outline','pandas','polars','postgresql','round'):
             raise ValueError(
-                SQLDataModel.ErrorFormat(f"ValueError: invalid value '{style}', argument for `style` must be one of 'ascii', 'bare', 'dash', 'default', 'double', 'markdown', 'outline', 'pandas', 'polars', 'postgresql', 'round' or 'thick'")
+                SQLDataModel.ErrorFormat(f"ValueError: invalid value '{style}', argument for `style` must be one of 'ascii', 'bare', 'dash', 'default', 'double', 'list', 'markdown', 'outline', 'pandas', 'polars', 'postgresql' or 'round'")
             )
         self.table_style = style
 
     def __repr__(self) -> str:
         """
         Returns a formatted string representation of the SQLDataModel instance.
 
@@ -7892,15 +8038,15 @@
             fetch_fmt_stmt = f"""select '{row_lh}' || {fetch_idx}{header_fmt_str}||'{row_rh}{table_dynamic_newline}' as "_full_row" from "{self.sql_model}" order by "{self.sql_idx}" asc limit {max_display_rows}"""
         formatted_response = self.sql_db_conn.execute(fetch_fmt_stmt)
         if column_alignment is None: # dynamic alignment
             formatted_headers = [f"""{(col if len(col) <= header_length_dict[col] else f"{col[:(header_length_dict[col]-2)]}⠤⠄"):{'>' if header_py_dtype_dict[col] in ('int','float') else '<'}{header_length_dict[col]}}""" if col != self.sql_idx else f"""{' ':>{header_length_dict[col]}}"""for col in display_headers]
         else: # left, center, right alignment
             formatted_headers = [(f"""{col:{column_alignment}{header_length_dict[col]}}""" if len(col) <= header_length_dict[col] else f"""{col[:(header_length_dict[col]-2)]}⠤⠄""") if col != self.sql_idx else f"""{' ':>{header_length_dict[col]}}"""for col in display_headers]
         # table_top_bar = "".join([top_lh, top_sep.join([top_hbar * header_length_dict[col] for col in display_headers]), top_rh, table_bare_newline])
-        col_lengths = [val for val in header_length_dict.values()]
+        col_lengths = [header_length_dict[col] for col in display_headers]
         table_top_bar = "".join([top_lh, top_sep.join([top_hbar * length for length in col_lengths]), top_rh, table_bare_newline])
         table_top_bar = table_top_bar if len(table_top_bar.strip()) >=1 else """"""
         table_repr = "".join([table_repr, table_top_bar])
         table_repr = "".join([table_repr, row_lh, row_sep.join(formatted_headers), row_rh, table_dynamic_newline])
         # table_mid_bar = "".join([mid_lh, mid_sep.join([mid_hbar * header_length_dict[col] for col in display_headers]), mid_rh, table_bare_newline])
         table_mid_bar = "".join([mid_lh, mid_sep.join([mid_hbar * length for length in col_lengths]), mid_rh, table_bare_newline])
         table_mid_bar = table_mid_bar if len(table_mid_bar.strip()) >=1 else """"""
@@ -10488,38 +10634,45 @@
         self.header_master = header_master 
         """``dict[str, tuple]``: Maps the current model's column metadata in the format of ``'column_name': ('sql_dtype', 'py_dtype', is_regular_column, 'default_alignment')``, updated by :meth:`SQLDataModel._update_model_metadata`."""
         self.dtypes = {k:v[1] for k,v in self.header_master.items() if v[2]}
         self.shape = (self.shape[0], self.column_count)
         if update_row_meta:
             self._update_indicies()
 
-    def _generate_sql_stmt(self, columns:list[str]=None, rows:int|slice|tuple=None, index:bool=True) -> str:
+    def _generate_sql_stmt(self, columns:list[str]=None, rows:int|slice|tuple=None, index:bool=True, na_rep:str=None) -> str:
         """
         Generate an SQL statement for fetching specific columns and rows from the model, duplicate column references are aliased in order of appearance.
 
         Parameters:
             ``columns`` (list of str, optional): The list of columns to include in the SQL statement. If not provided, all columns from the model will be included.
             ``rows`` (int, slice, tuple, optional): The rows to include in the SQL statement. It can be an integer for a single row, a slice for a range of rows, or a tuple for specific row indices. If not provided, all rows will be included.
             ``index`` (bool, optional): If True, include the primary index column in the SQL statement.
+            ``na_rep`` (str, optional): If provided, all null or empty string values are replaced with value.
 
         Returns:
             ``str``: The generated SQL statement.   
         
         Change Log:
+            - Version 0.4.0 (2024-04-23):
+                - Added ``nap_rep`` parameter to fill null or missing fields with provided value.
+
             - Version 0.3.0 (2024-03-31):
                 - Renamed ``include_index`` parameter to ``index`` for package consistency.
 
         Note:
             - No validation is performed on row or column indicies, see :meth:`SQLDataModel.validate_indicies()` for implementation and usage.
         """
         if columns is None:
             columns = self.headers
         if index:
             columns = [self.sql_idx,*columns]
-        headers_selection_str = ",".join([f'"{col}" as "{col_alias}"' for col,col_alias in zip(columns,SQLDataModel.alias_duplicates(columns))])
+        if na_rep is None:
+            headers_selection_str = ",".join([f'''"{col}" as "{col_alias}"''' for col,col_alias in zip(columns,SQLDataModel.alias_duplicates(columns))])
+        else:
+            headers_selection_str = ",".join([f'''ifnull("{col}",'{na_rep}') as "{col_alias}"''' for col,col_alias in zip(columns,SQLDataModel.alias_duplicates(columns))])
         if isinstance(rows, int):
             row_selection_str = f"""where "{self.sql_idx}" = {rows}"""
         elif isinstance(rows, slice):
             row_selection_str = f"""where "{self.sql_idx}" >= {rows.start} and "{self.sql_idx}" < {rows.stop}"""
         elif isinstance(rows, tuple):
             row_selection_str = f"""where "{self.sql_idx}" in {f'{rows}' if len(rows) != 1 else f'({rows[0]})'}"""
         else:
@@ -10556,84 +10709,92 @@
         if isinstance(columns,str):
             columns = [columns]
         columns_str = ",".join([f'"{col}"' for col in columns])
         ordering_str = f"""order by "{self.sql_idx}" {ordering}""" if ordering in ("asc","desc") else "order by random()"
         fetch_stmt = " ".join(("select",f'"{self.sql_idx}",' if index else '',columns_str,f'from "{self.sql_model}"', ordering_str, f"limit {n_rows}"))
         return fetch_stmt
 
-    def _generate_table_style(self) -> tuple[tuple[str]]:
+    def _generate_table_style(self, style:Literal['ascii','bare','dash','default','double','list','markdown','outline','pandas','polars','postgresql','round']=None) -> tuple[tuple[str]]:
         """
         Generates the character sets required for formatting ``SQLDataModel`` according to the value currently set at :py:attr:`SQLDataModel.table_style`.
         
+        Parameters:
+            ``style`` (Literal['ascii','bare','dash','default','double','list','markdown','outline','pandas','polars','postgresql','round'], optional): The table style to return. Default is value set on :py:attr:`SQLDataModel.table_style`.
+
         Returns:
             ``tuple[tuple[str]]``: A 4-tuple containing the characters required for top, middle, row and lower table sections.
-        
+
+        Change Log:
+            - Version 0.3.10 (2024-04-16):
+                - Added ``style`` parameter to allow use by :meth:`SQLDataModel.to_text()` to generate new formatting styles introduced in version 0.3.9.
+                    
         Note:
             - This method is called by :meth:`SQLDataModel.__repr__()` to parse the characters necessary for constructing the tabular representation of the ``SQLDataModel``, any modifications or changes to this method may result in unexpected behavior.
         """
-        if self.table_style == 'ascii':    
+        style = self.table_style if style is None else style
+        if style == 'ascii':    
             return  (('+-','-','-+-','-+') 
                     ,('+-','-','-+-','-+') 
                     ,('| ',    ' | ',' |') 
                     ,('+-','-','-+-','-+'))
-        if self.table_style == 'bare':     
+        if style == 'bare':     
             return  (('','','','')
                     ,('','-','--','')      
                     ,('',    '  ','')      
                     ,('','','',''))        
-        if self.table_style == 'dash': 
+        if style == 'dash': 
             return  (('┌─','─','─┬─','─┐')
                     ,('├╴','╴','╴┼╴','╴┤')
                     ,('│ ',    ' ╎ ',' │')
                     ,('└─','─','─┴─','─┘'))            
-        if self.table_style == 'default':  
+        if style == 'default':  
             return  (('┌─','─','─┬─','─┐') 
                     ,('├─','─','─┼─','─┤') 
                     ,('│ ',    ' │ ',' │') 
                     ,('└─','─','─┴─','─┘'))
-        if self.table_style == 'double':   
+        if style == 'double':   
             return  (('╔═','═','═╦═','═╗') 
                     ,('╠═','═','═╬═','═╣') 
                     ,('║ ',    ' ║ ',' ║') 
                     ,('╚═','═','═╩═','═╝'))
-        if self.table_style == 'markdown': 
+        if style == 'list':     
+            return  (('',' ','  ','')
+                    ,('','-','  ','')
+                    ,('',    '  ','')
+                    ,('',' ','  ',''))        
+        if style == 'markdown': 
             return  (('','','','')
                     ,('|-','-','-|-','-|')
                     ,('| ',    ' | ',' |')
                     ,('','','',''))
-        if self.table_style == 'outline':
+        if style == 'outline':
             return  (('┌─','─','──','─┐')
                     ,('├─','─','──','─┤')
                     ,('│ ',    '  ',' │')
                     ,('└─','─','──','─┘'))
-        if self.table_style == 'pandas':
+        if style == 'pandas':
             return  (('','','','')
                     ,('','','','')
                     ,('',    '  ','')
                     ,('','','',''))
-        if self.table_style == 'polars':
+        if style == 'polars':
             return  (('┌─','─','─┬─','─┐')
                     ,('╞═','═','═╪═','═╡')
                     ,('│ ',    ' ┆ ',' │')
                     ,('└─','─','─┴─','─┘'))
-        if self.table_style == 'postgresql':
+        if style == 'postgresql':
             return  (('','','','')
                     ,('','-','-+-','')
                     ,('',    ' | ','')
                     ,('','','',''))
-        if self.table_style == 'round':
+        if style == 'round':
             return  (('╭─','─','─┬─','─╮')
                     ,('├─','─','─┼─','─┤')
                     ,('│ ',    ' │ ',' │')
                     ,('╰─','─','─┴─','─╯'))
-        if self.table_style == 'thick':
-            return  (('┏━','━','━┳━','━┓')
-                    ,('┣━','━','━╋━','━┫')
-                    ,('┃ ',    ' ┃ ',' ┃')
-                    ,('┗━','━','━┻━','━┛'))
         else: # default styling
             return  (('┌─','─','─┬─','─┐') 
                     ,('├─','─','─┼─','─┤') 
                     ,('│ ',    ' │ ',' │') 
                     ,('└─','─','─┴─','─┘'))   
 
     def _update_indicies(self) -> None:
```

### Comparing `sqldatamodel-0.3.9/src/SQLDataModel/StandardDeviation.py` & `sqldatamodel-0.4.0/src/SQLDataModel/StandardDeviation.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.3.9/src/SQLDataModel/converters.py` & `sqldatamodel-0.4.0/src/SQLDataModel/converters.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.3.9/src/SQLDataModel/demo.py` & `sqldatamodel-0.4.0/src/SQLDataModel/demo.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.3.9/src/SQLDataModel/exceptions.py` & `sqldatamodel-0.4.0/src/SQLDataModel/exceptions.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.3.9/src/SQLDataModel/extensions/str_utils.c` & `sqldatamodel-0.4.0/src/SQLDataModel/extensions/str_utils.c`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.3.9/src/SQLDataModel.egg-info/PKG-INFO` & `sqldatamodel-0.4.0/src/SQLDataModel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.3.9
+Version: 0.4.0
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
-Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package
+Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package,polars2pandas,pandas2polars
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -262,16 +262,16 @@
 
 # Filter to only 'Future' missions
 sdm = sdm[sdm['Status'] == 'Future']
 
 # Create new column with today's date so it ages better!
 sdm['Updated'] = datetime.date.today()
 
-# Send our table to a new html file, this time without the index
-saturn_html = sdm.to_html('Future-Saturn.html', include_index=False)
+# Create a new html file with our table
+sdm.to_html('Future-Saturn.html', index=False)
 ```
 Here's a snippet from the `Future-Saturn.html` file generated by the `to_html()` method:
 ```html
 <!-- Metadata Removed -->
 <table>
     <tr>
         <th>Mission</th>
@@ -531,15 +531,15 @@
 
   * [`ANSIColor`](https://sqldatamodel.readthedocs.io/en/latest/SQLDataModel.html#SQLDataModel.ANSIColor.ANSIColor) for terminal styling.
   * [`HTMLParser`](https://sqldatamodel.readthedocs.io/en/latest/SQLDataModel.html#SQLDataModel.HTMLParser.HTMLParser) for parsing tabular data from the web.
   * [`JSONEncoder`](https://sqldatamodel.readthedocs.io/en/latest/SQLDataModel.html#SQLDataModel.JSONEncoder.DataTypesEncoder) for type casting and encoding JSON data.
   * [`SQLDataModel`](https://sqldatamodel.readthedocs.io/en/latest/SQLDataModel.html#SQLDataModel.SQLDataModel.SQLDataModel) for wrapping it all up.
 
 
-However, to skip over the less relevant modules and jump straight to the meat of the package, the ``SQLDataModel`` module, click [here](https://sqldatamodel.readthedocs.io/en/latest/SQLDataModel.html#SQLDataModel.SQLDataModel.SQLDataModel). 
+However, to skip over the less relevant modules and jump straight to the meat of the package, the ``SQLDataModel`` module, click [here](https://sqldatamodel.readthedocs.io/en/latest/modules.html). 
 
 ---
 
 ### Motivation
 
 While there are packages/dependencies out there that can accomplish some of the same tasks as `SQLDataModel`, they're either missing key features or end up being overkill for common tasks like grabbing and converting tables from source A to destination B, or they don't quite handle the full process and require additional dependencies to make it all work. When you find yourself doing the same thing over and over again, eventually you sit down and write a package to do it for you.
```

### Comparing `sqldatamodel-0.3.9/src/SQLDataModel.egg-info/SOURCES.txt` & `sqldatamodel-0.4.0/src/SQLDataModel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.3.9/tests/test_Future.py` & `sqldatamodel-0.4.0/tests/test_Future.py`

 * *Files 1% similar despite different names*

```diff
@@ -589,22 +589,34 @@
         assert input_data[i] == output_data[i] 
     ### test from delimited raw csv literal ###
     input_literal = SQLDataModel(sample_data[1:], sample_data[0]).to_csv()
     output_literal = SQLDataModel.from_csv(input_literal).to_csv()
     assert input_literal == output_literal
 
 @pytest.mark.core
-def test_to_from_delimited(sample_data):
+def test_to_from_csv_delimiters(sample_data):
     input_data, input_headers = sample_data[1:], sample_data[0]
     sdm = SQLDataModel(input_data,input_headers)
     input_data = sdm.data(include_headers=True)
     valid_delimiters = (",","\t",";","|",":"," ")
     for delimiter in valid_delimiters:
         dsv = sdm.to_csv(delimiter=delimiter)
-        sdm = SQLDataModel.from_csv(dsv, delimiters=delimiter)
+        sdm = SQLDataModel.from_csv(dsv, delimiter=delimiter)
+        output_data = sdm.data(include_headers=True)
+        assert input_data == output_data
+
+@pytest.mark.core
+def test_to_from_delimited_source(sample_data):
+    input_data, input_headers = sample_data[1:], sample_data[0]
+    sdm = SQLDataModel(input_data,input_headers)
+    input_data = sdm.data(include_headers=True)
+    valid_delimiters = (",","\t",";","|",":"," ")
+    for delimiter in valid_delimiters:
+        dsv = sdm.to_csv(delimiter=delimiter)
+        sdm = SQLDataModel.from_delimited(dsv)
         output_data = sdm.data(include_headers=True)
         assert input_data == output_data
 
 @pytest.mark.core
 def test_merge():
     left_headers = ["Name", "Age", "ID"]
     left_data = [        
@@ -886,14 +898,23 @@
 ║ 0 ║ text 1 ║   1 ║  1.10 ║ 2001-01-11 ║
 ║ 1 ║ text 2 ║   2 ║  2.20 ║ 2002-02-12 ║
 ║ 2 ║ text 3 ║   3 ║  3.30 ║ 2003-03-13 ║
 ║ 3 ║ text 4 ║   4 ║  4.40 ║ 2004-04-14 ║
 ╚═══╩════════╩═════╩═══════╩════════════╝
 [4 rows x 4 columns]
 """,
+'list':"""
+   string  int  float  date      
+-  ------  ---  -----  ----------
+0  text 1    1   1.10  2001-01-11
+1  text 2    2   2.20  2002-02-12
+2  text 3    3   3.30  2003-03-13
+3  text 4    4   4.40  2004-04-14
+[4 rows x 4 columns]
+""",
 'markdown':"""
 |   | string | int | float | date       |
 |---|--------|-----|-------|------------|
 | 0 | text 1 |   1 |  1.10 | 2001-01-11 |
 | 1 | text 2 |   2 |  2.20 | 2002-02-12 |
 | 2 | text 3 |   3 |  3.30 | 2003-03-13 |
 | 3 | text 4 |   4 |  4.40 | 2004-04-14 |
@@ -945,33 +966,22 @@
 ├───┼────────┼─────┼───────┼────────────┤
 │ 0 │ text 1 │   1 │  1.10 │ 2001-01-11 │
 │ 1 │ text 2 │   2 │  2.20 │ 2002-02-12 │
 │ 2 │ text 3 │   3 │  3.30 │ 2003-03-13 │
 │ 3 │ text 4 │   4 │  4.40 │ 2004-04-14 │
 ╰───┴────────┴─────┴───────┴────────────╯
 [4 rows x 4 columns]
-""",
-'thick':"""
-┏━━━┳━━━━━━━━┳━━━━━┳━━━━━━━┳━━━━━━━━━━━━┓
-┃   ┃ string ┃ int ┃ float ┃ date       ┃
-┣━━━╋━━━━━━━━╋━━━━━╋━━━━━━━╋━━━━━━━━━━━━┫
-┃ 0 ┃ text 1 ┃   1 ┃  1.10 ┃ 2001-01-11 ┃
-┃ 1 ┃ text 2 ┃   2 ┃  2.20 ┃ 2002-02-12 ┃
-┃ 2 ┃ text 3 ┃   3 ┃  3.30 ┃ 2003-03-13 ┃
-┃ 3 ┃ text 4 ┃   4 ┃  4.40 ┃ 2004-04-14 ┃
-┗━━━┻━━━━━━━━┻━━━━━┻━━━━━━━┻━━━━━━━━━━━━┛
-[4 rows x 4 columns]
 """}
     headers = ['string', 'int', 'float', 'date']
     data = [
          ('text 1',  1, 1.1, datetime.date(2001, 1, 11))
         ,('text 2', 2, 2.2, datetime.date(2002, 2, 12))
         ,('text 3', 3, 3.3, datetime.date(2003, 3, 13))
         ,('text 4', 4, 4.4, datetime.date(2004, 4, 14))
     ]
     sdm = SQLDataModel(data,headers, min_column_width=3, max_column_width=38, display_index=True, display_float_precision=2)
-    repr_styles = ['ascii','bare','dash','default','double','markdown','outline','pandas','polars','postgresql','round','thick']   
+    repr_styles = ['ascii','bare','dash','default','double','list','markdown','outline','pandas','polars','postgresql','round']   
     for style in repr_styles:
         sdm.set_table_style(style=style)
         expected_repr = style_output_dict[style].strip('\n')
         output_repr = sdm.__repr__()
         assert output_repr == expected_repr
```

### Comparing `sqldatamodel-0.3.9/tests/test_SQLDataModel.py` & `sqldatamodel-0.4.0/tests/test_SQLDataModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -589,22 +589,34 @@
         assert input_data[i] == output_data[i] 
     ### test from delimited raw csv literal ###
     input_literal = SQLDataModel(sample_data[1:], sample_data[0]).to_csv()
     output_literal = SQLDataModel.from_csv(input_literal).to_csv()
     assert input_literal == output_literal
 
 @pytest.mark.core
-def test_to_from_delimited(sample_data):
+def test_to_from_csv_delimiters(sample_data):
     input_data, input_headers = sample_data[1:], sample_data[0]
     sdm = SQLDataModel(input_data,input_headers)
     input_data = sdm.data(include_headers=True)
     valid_delimiters = (",","\t",";","|",":"," ")
     for delimiter in valid_delimiters:
         dsv = sdm.to_csv(delimiter=delimiter)
-        sdm = SQLDataModel.from_csv(dsv, delimiters=delimiter)
+        sdm = SQLDataModel.from_csv(dsv, delimiter=delimiter)
+        output_data = sdm.data(include_headers=True)
+        assert input_data == output_data
+
+@pytest.mark.core
+def test_to_from_delimited_source(sample_data):
+    input_data, input_headers = sample_data[1:], sample_data[0]
+    sdm = SQLDataModel(input_data,input_headers)
+    input_data = sdm.data(include_headers=True)
+    valid_delimiters = (",","\t",";","|",":"," ")
+    for delimiter in valid_delimiters:
+        dsv = sdm.to_csv(delimiter=delimiter)
+        sdm = SQLDataModel.from_delimited(dsv)
         output_data = sdm.data(include_headers=True)
         assert input_data == output_data
 
 @pytest.mark.core
 def test_merge():
     left_headers = ["Name", "Age", "ID"]
     left_data = [        
@@ -886,14 +898,23 @@
 ║ 0 ║ text 1 ║   1 ║  1.10 ║ 2001-01-11 ║
 ║ 1 ║ text 2 ║   2 ║  2.20 ║ 2002-02-12 ║
 ║ 2 ║ text 3 ║   3 ║  3.30 ║ 2003-03-13 ║
 ║ 3 ║ text 4 ║   4 ║  4.40 ║ 2004-04-14 ║
 ╚═══╩════════╩═════╩═══════╩════════════╝
 [4 rows x 4 columns]
 """,
+'list':"""
+   string  int  float  date      
+-  ------  ---  -----  ----------
+0  text 1    1   1.10  2001-01-11
+1  text 2    2   2.20  2002-02-12
+2  text 3    3   3.30  2003-03-13
+3  text 4    4   4.40  2004-04-14
+[4 rows x 4 columns]
+""",
 'markdown':"""
 |   | string | int | float | date       |
 |---|--------|-----|-------|------------|
 | 0 | text 1 |   1 |  1.10 | 2001-01-11 |
 | 1 | text 2 |   2 |  2.20 | 2002-02-12 |
 | 2 | text 3 |   3 |  3.30 | 2003-03-13 |
 | 3 | text 4 |   4 |  4.40 | 2004-04-14 |
@@ -945,33 +966,22 @@
 ├───┼────────┼─────┼───────┼────────────┤
 │ 0 │ text 1 │   1 │  1.10 │ 2001-01-11 │
 │ 1 │ text 2 │   2 │  2.20 │ 2002-02-12 │
 │ 2 │ text 3 │   3 │  3.30 │ 2003-03-13 │
 │ 3 │ text 4 │   4 │  4.40 │ 2004-04-14 │
 ╰───┴────────┴─────┴───────┴────────────╯
 [4 rows x 4 columns]
-""",
-'thick':"""
-┏━━━┳━━━━━━━━┳━━━━━┳━━━━━━━┳━━━━━━━━━━━━┓
-┃   ┃ string ┃ int ┃ float ┃ date       ┃
-┣━━━╋━━━━━━━━╋━━━━━╋━━━━━━━╋━━━━━━━━━━━━┫
-┃ 0 ┃ text 1 ┃   1 ┃  1.10 ┃ 2001-01-11 ┃
-┃ 1 ┃ text 2 ┃   2 ┃  2.20 ┃ 2002-02-12 ┃
-┃ 2 ┃ text 3 ┃   3 ┃  3.30 ┃ 2003-03-13 ┃
-┃ 3 ┃ text 4 ┃   4 ┃  4.40 ┃ 2004-04-14 ┃
-┗━━━┻━━━━━━━━┻━━━━━┻━━━━━━━┻━━━━━━━━━━━━┛
-[4 rows x 4 columns]
 """}
     headers = ['string', 'int', 'float', 'date']
     data = [
          ('text 1',  1, 1.1, datetime.date(2001, 1, 11))
         ,('text 2', 2, 2.2, datetime.date(2002, 2, 12))
         ,('text 3', 3, 3.3, datetime.date(2003, 3, 13))
         ,('text 4', 4, 4.4, datetime.date(2004, 4, 14))
     ]
     sdm = SQLDataModel(data,headers, min_column_width=3, max_column_width=38, display_index=True, display_float_precision=2)
-    repr_styles = ['ascii','bare','dash','default','double','markdown','outline','pandas','polars','postgresql','round','thick']   
+    repr_styles = ['ascii','bare','dash','default','double','list','markdown','outline','pandas','polars','postgresql','round']   
     for style in repr_styles:
         sdm.set_table_style(style=style)
         expected_repr = style_output_dict[style].strip('\n')
         output_repr = sdm.__repr__()
         assert output_repr == expected_repr
```

