# Comparing `tmp/tablinum-0.1.1.tar.gz` & `tmp/tablinum-0.1.2.tar.gz`

## Comparing `tablinum-0.1.1.tar` & `tablinum-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 tablinum-0.1.1/src/tablinum/__about__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tablinum-0.1.1/src/tablinum/__init__.py
--rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 tablinum-0.1.1/src/tablinum/tab_fun_dates.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 tablinum-0.1.1/src/tablinum/tab_fun_maths.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 tablinum-0.1.1/src/tablinum/tab_fun_useful.py
--rw-r--r--   0        0        0    58663 2020-02-02 00:00:00.000000 tablinum-0.1.1/src/tablinum/tablinum.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tablinum-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tablinum-0.1.1/tests/test-input.txt
--rw-r--r--   0        0        0     9691 2020-02-02 00:00:00.000000 tablinum-0.1.1/tests/test_tab_calculation.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 tablinum-0.1.1/tests/test_tab_command_line.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tablinum-0.1.1/tests/test_tab_contingency.py
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 tablinum-0.1.1/tests/test_tab_filter.py
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 tablinum-0.1.1/tests/test_tab_grouping.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 tablinum-0.1.1/tests/test_tab_help.py
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 tablinum-0.1.1/tests/test_tab_levels.py
--rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 tablinum-0.1.1/tests/test_tab_makers.py
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 tablinum-0.1.1/tests/test_tab_parsing.py
--rw-r--r--   0        0        0     9593 2020-02-02 00:00:00.000000 tablinum-0.1.1/tests/test_tab_poppers_and_adders.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 tablinum-0.1.1/tests/test_tab_roller.py
--rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 tablinum-0.1.1/tests/test_tab_sort.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 tablinum-0.1.1/tests/test_tab_text_manip.py
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 tablinum-0.1.1/tests/test_tab_wrangler.py
--rw-r--r--   0        0        0    13736 2020-02-02 00:00:00.000000 tablinum-0.1.1/tests/test_tablinum.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 tablinum-0.1.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tablinum-0.1.1/LICENSE
--rw-r--r--   0        0        0    58932 2020-02-02 00:00:00.000000 tablinum-0.1.1/README.md
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 tablinum-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    59820 2020-02-02 00:00:00.000000 tablinum-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 tablinum-0.1.2/src/tablinum/__about__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tablinum-0.1.2/src/tablinum/__init__.py
+-rw-r--r--   0        0        0     7697 2020-02-02 00:00:00.000000 tablinum-0.1.2/src/tablinum/tab_fun_dates.py
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 tablinum-0.1.2/src/tablinum/tab_fun_maths.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 tablinum-0.1.2/src/tablinum/tab_fun_useful.py
+-rw-r--r--   0        0        0    58701 2020-02-02 00:00:00.000000 tablinum-0.1.2/src/tablinum/tablinum.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test-input.txt
+-rw-r--r--   0        0        0     9691 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_calculation.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_command_line.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_contingency.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_filter.py
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_grouping.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_help.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_levels.py
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_makers.py
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_parsing.py
+-rw-r--r--   0        0        0     9593 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_poppers_and_adders.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_roller.py
+-rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_sort.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_text_manip.py
+-rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_wrangler.py
+-rw-r--r--   0        0        0    13743 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tablinum.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 tablinum-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tablinum-0.1.2/LICENSE
+-rw-r--r--   0        0        0    60858 2020-02-02 00:00:00.000000 tablinum-0.1.2/README.md
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 tablinum-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    61746 2020-02-02 00:00:00.000000 tablinum-0.1.2/PKG-INFO
```

### Comparing `tablinum-0.1.1/src/tablinum/tab_fun_dates.py` & `tablinum-0.1.2/src/tablinum/tab_fun_dates.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,193 +1,185 @@
 #! /usr/bin/env python3
 '''Date functions to use in tabulate `arr` expressions
 
-Toby Thurston -- 10 Feb 2021
+date()        takes int, returns string 
+parse_date()  takes int or string, returns datetime.date
+base()        takes string, returns int
+
+Toby Thurston -- 21 Apr 2024
 
-    "dow": tab_fun_dates.dow,
-    "base": tab_fun_dates.base,
-    "date": tab_fun_dates.date,
-
-    "hms": tab_fun_dates.hms,
-    "hr": tab_fun_dates.hr,
-    "mins": tab_fun_dates.mins,
-    "secs": tab_fun_dates.secs,
 
 '''
 import datetime
+import re
 
 
 def parse_date(sss, today=None):
     '''Try to parse a date
-    >>> parse_date(730486).isoformat()
-    '2001-01-01'
-    >>> parse_date("1 January 2001").isoformat()
-    '2001-01-01'
-    >>> parse_date(base("1 January 2001")).isoformat()
-    '2001-01-01'
-    >>> parse_date("6/7/95").isoformat()
-    '1995-07-06'
-    >>> parse_date("2022-W47-2").isoformat()
-    '2022-11-22'
-    >>> parse_date("Fri 1st Apr 2022").isoformat()
-    '2022-04-01'
-    >>> parse_date("Sat 29th July 2023").isoformat()
-    '2023-07-29'
-    >>> parse_date("Fri 29th Sept 2023").isoformat()
-    '2023-09-29'
-    >>> parse_date("Sat 19th Mar 2022").isoformat()
-    '2022-03-19'
-    >>> parse_date("Sunday", today='2022-03-17').isoformat()
-    '2022-03-20'
+    >>> parse_date(730486)
+    datetime.date(2001, 1, 1)
+
+    >>> parse_date(20010101)
+    datetime.date(2001, 1, 1)
+
+    >>> parse_date(3652059)
+    datetime.date(9999, 12, 31)
+
+    >>> parse_date('1')
+    datetime.date(1, 1, 1)
+
+    >>> parse_date("730486")
+    datetime.date(2001, 1, 1)
+    
+    >>> parse_date("1 January 2001")
+    datetime.date(2001, 1, 1)
+    
+    >>> parse_date("6/7/95")
+    datetime.date(1995, 7, 6)
+
+    >>> parse_date("2022-W47-2")
+    datetime.date(2022, 11, 22)
+
+    >>> parse_date("Fri 1st Apr 2022")
+    datetime.date(2022, 4, 1)
+
+    >>> parse_date("Sat 29th July 2023")
+    datetime.date(2023, 7, 29)
+
+    >>> parse_date("Fri 29th Sept 2023")
+    datetime.date(2023, 9, 29)
+
+    >>> parse_date("Sat 19th Mar 2022")
+    datetime.date(2022, 3, 19)
+
+    >>> parse_date("Sunday", today='2022-03-17')
+    datetime.date(2022, 3, 20)
+
     '''
-    try:
-        if 0 < int(sss) < 900000:
+
+    maxo = datetime.date.max.toordinal()
+    mino = datetime.date.min.toordinal()
+
+    if isinstance(sss, int):
+        if mino <= sss <= maxo:
             return datetime.date.fromordinal(sss)
-    except (TypeError, ValueError) as _:
-        pass
+   
+    sss = str(sss)
 
-    days = "Monday Tuesday Wednesday Thursday Friday Saturday Sunday".split()
-    try:
-        iso_dow = 1 + days.index(str(sss).capitalize())
-    except ValueError:
-        pass
-    else:
-        if 1 <= iso_dow <= 7:
-            if today is None:
-                today = datetime.datetime.today()
-            else:
-                today = datetime.datetime.strptime(today, '%Y-%m-%d')
-            year, week = today.strftime("%G-%V").split("-")
-            return datetime.datetime.strptime(f'{year}-W{week}-{iso_dow}', "%G-W%V-%u").date()
+    if sss.isdigit() and int(sss) <= maxo:
+        return datetime.date.fromordinal(int(sss))
 
-    sss = str(sss).replace('Sept ', 'Sep ')
+    days = "Monday Tuesday Wednesday Thursday Friday Saturday Sunday".split()
+    if sss.capitalize() in days:
+        iso_dow = 1 + days.index(sss.capitalize())
+        if today is None:
+            today = datetime.datetime.today()
+        else:
+            today = datetime.datetime.strptime(today, '%Y-%m-%d')
+        year, week = today.strftime("%G-%V").split("-")
+        return datetime.datetime.strptime(f'{year}-W{week}-{iso_dow}', "%G-W%V-%u").date()
 
+    sss = sss.replace('Sept ', 'Sep ')
     for fmt in ('%Y-%m-%d', '%Y%m%d', '%d %B %Y', '%d %b %Y', '%G-W%V-%u', '%d-%b-%Y',
                 '%d %b %y', '%d %B %y', '%d/%m/%Y', '%d/%m/%y', '%B %d, %Y',
                 '%A %d %B %Y',
                 '%a %dth %b %Y', '%a %dst %b %Y', '%a %dnd %b %Y', '%a %drd %b %Y',
                 '%a %dth %B %Y', '%a %dst %B %Y', '%a %dnd %B %Y', '%a %drd %B %Y',
                 '%m/%d/%Y',
                 '%c', '%x'):
         try:
             return datetime.datetime.strptime(str(sss), fmt).date()
         except ValueError:
-            pass
+            continue
 
     raise ValueError
 
 
-def dow(sss, date_format="%a"):
+def dow(sss):
     '''Is it Friday yet?
     >>> dow("1 January 2001")
     'Mon'
     >>> dow(base("1 January 2001"))
     'Mon'
     >>> dow("31/12/2021")
     'Fri'
-    >>> dow("1 January 2001", "%A")
-    'Monday'
-    >>> dow("date")
-    '%a'
-
-    You can actually use this to produce any strftime format...
-
-    >>> dow("25 Dec 2001", "%c")
-    'Tue Dec 25 00:00:00 2001'
-
-    >>> dow("25 Dec 2001", "%u")
-    '2'
 
     '''
-    try:
-        return parse_date(sss).strftime(date_format)
-    except (TypeError, ValueError):
-        return date_format
+    d = datetime.date.today() if sss is None else parse_date(sss)
+    return d.strftime('%a')
 
 
 def base(sss=None):
     '''Get today's date as "base" number, or whatever date you give
+    
+
     >>> base("1 January 2001")
     730486
     >>> base("1 January 1901")
     693961
     >>> base("01/01/01")
     730486
     >>> base("20010102")
     730487
-    >>> base(20010102)
-    730487
     >>> base("2001-01-03")
     730488
     >>> base("03-jan-2001")
     730488
     >>> base("31 Dec 2000")-base("1 Jan 1901")
     36524
-    >>> base() - datetime.date.today().toordinal()
-    0
-    >>> datetime.date.today().toordinal() - base(-4)
-    4
-    >>> base('Date')
-    'base(Date)'
-    '''
-    if sss is None:
-        return datetime.date.today().toordinal()
-
-    if isinstance(sss, int) and abs(sss) < 1000:
-        return datetime.date.today().toordinal() + sss
-
-    try:
-        return parse_date(sss).toordinal()
-    except (TypeError, ValueError):
-        return f'base({sss})'
+    >>> base() == datetime.date.today().toordinal()
+    True
+    '''
+    d = datetime.date.today() if sss is None else parse_date(sss)
+    return d.toordinal()
 
 
-def date(ordinal=0):
+def date(sss='0', format=None):
     '''Turn a base number (or an epoch time or a millisecond epoch time) into a date
-    >>> date(716257)
+    >>> date('716257')
     '1962-01-17'
-    >>> date(3652059)
+    >>> date('3652059')
     '9999-12-31'
-    >>> date(3652060)
+    >>> date('3652060')
     '1970-02-12T07:27:40'
-    >>> date(100000000000)
+    >>> date('100000000000')
     '5138-11-16T09:46:40'
-    >>> date(100000000001)
+    >>> date('100000000001')
     '1973-03-03T09:46:40.001000'
-    >>> date(10) == (datetime.date.today() + datetime.timedelta(days=10)).isoformat()
+    >>> date('10') == (datetime.date.today() + datetime.timedelta(days=10)).isoformat()
+    True
+    >>> date('-10000000000000000000000000') == date('0')
     True
-    >>> date('ts')
-    'date(ts)'
-    >>> date(-10000000000000000000000000) == date(0)
+    >>> date('-2000') == date('0')
     True
-    >>> date(-2000) == date(0)
+    >>> date() == datetime.date.today().isoformat()
     True
-    >>> date(base(730486))
+    >>> date(730486)
     '2001-01-01'
+    >>> date(730486, '%a')
+    'Mon'
     '''
-    try:
-        ordinal = int(ordinal)
-    except (TypeError, ValueError):
-        ordinal = base(ordinal)
-        if ordinal.startswith('base'):
-            return ordinal.replace('base', 'date')
+    ordinal = int(sss)
 
     if abs(ordinal) < 1000:
-        dt = datetime.date.today() + datetime.timedelta(days=ordinal)
+        d = datetime.date.today() + datetime.timedelta(days=ordinal)
     elif ordinal > 100000000000:  # about 5000 AD as an epoch, so assume epoch ms
-        dt = datetime.datetime.fromtimestamp(ordinal / 1000)
+        d = datetime.datetime.fromtimestamp(ordinal / 1000)
     elif ordinal > datetime.date.max.toordinal():  # > max date, so assume epoch seconds
-        dt = datetime.datetime.fromtimestamp(ordinal)
+        d = datetime.datetime.fromtimestamp(ordinal)
     else:
         try:
-            dt = datetime.date.fromordinal(ordinal)
+            d = datetime.date.fromordinal(ordinal)
         except (TypeError, ValueError, OverflowError):
-            dt = datetime.date.today()
+            d = datetime.date.today()
+
+    if format is None:
+        return d.isoformat()
 
-    return dt.isoformat()
+    return d.strftime(format)
 
 
 def hms(fractional_things):
     '''Turn decimal hours/degrees into h/d:mm:ss.fff
 
     >>> hms(57.2957795)
     '57:17:44.806'
@@ -282,20 +274,20 @@
     return date_time_string
 
 
 def UK_tax_year(sss):
     '''Return the UK tax year
 
     >>> UK_tax_year('1962-01-17')
-    'FY61/62'
+    'TY61/62'
     >>> UK_tax_year('2023-09-17')
-    'FY23/24'
+    'TY23/24'
 
     '''
     b = base(sss)
     year = int(date(b)[:4])
     c = base(f'{year}-04-05')
     if c > b:
         year -= 1
 
-    return f'FY{year % 100}/{(year+1) % 100}'
+    return f'TY{year % 100}/{(year+1) % 100}'
```

### Comparing `tablinum-0.1.1/src/tablinum/tab_fun_maths.py` & `tablinum-0.1.2/src/tablinum/tab_fun_maths.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.1/src/tablinum/tab_fun_useful.py` & `tablinum-0.1.2/src/tablinum/tab_fun_useful.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.1/src/tablinum/tablinum.py` & `tablinum-0.1.2/src/tablinum/tablinum.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,38 +51,38 @@
     'log': lambda x: decimal.Decimal(x).ln(),
     'log10': lambda x: decimal.Decimal(x).log10(),
     'sqrt': lambda x: decimal.Decimal(x).sqrt(),
     'caps': lambda x: str(x).capitalize(),
     'lower': lambda x: str(x).lower(),
     'upper': lambda x: str(x).upper(),
     'randomd': lambda: decimal.Decimal(str(random.random())),
-    'mlog': tab_fun_maths.mlog,
-    'mexp': tab_fun_maths.mexp,
-    'angle': tab_fun_maths.angle,
-    'dir': tab_fun_maths.dir,
     'floor': math.floor,
     'time': tab_fun_dates.as_time,
     'base': tab_fun_dates.base,
     'date': tab_fun_dates.date,
     'dow': tab_fun_dates.dow,
     'epoch': tab_fun_dates.epoch,
     'hms': tab_fun_dates.hms,
     'hr': tab_fun_dates.hr,
     'mins': tab_fun_dates.mins,
     'secs': tab_fun_dates.secs,
     'uktaxyear': tab_fun_dates.UK_tax_year,
-    'pi': tab_fun_maths.PI,
-    'tau': tab_fun_maths.TAU,
+    'angle': tab_fun_maths.angle,
     'cos': tab_fun_maths.cos, 'cosd': tab_fun_maths.cosd,
     'tan': tab_fun_maths.cos, 'tand': tab_fun_maths.tand,
     'hex': tab_fun_maths.decimal_to_hex,
     'oct': tab_fun_maths.decimal_to_oct,
+    'dir': tab_fun_maths.dir,
     'factors': tab_fun_maths.factors,
+    'mexp': tab_fun_maths.mexp,
+    'mlog': tab_fun_maths.mlog,
+    'pi': tab_fun_maths.PI,
     'hypot': tab_fun_maths.pyth_add,
     'sin': tab_fun_maths.sin, 'sind': tab_fun_maths.sind,
+    'tau': tab_fun_maths.TAU,
     'len': tab_fun_useful.length,
     'all': tab_fun_useful.t_all,
     'any': tab_fun_useful.t_any,
     'max': tab_fun_useful.t_max,
     'min': tab_fun_useful.t_min,
     'minp': tab_fun_useful.t_minp,
     'sorted': tab_fun_useful.t_sorted,
@@ -105,32 +105,32 @@
     >>> as_numeric_tuple(None)
     (1000000000000.0, '')
 
     >>> as_numeric_tuple("3.14")
     (3.14, '3.14')
 
     >>> as_numeric_tuple("2020-05-01")
-    (1588287600, '2020-05-01')
+    (737546, '2020-05-01')
 
     >>> as_numeric_tuple("2 May 2020")
-    (1588374000, '2 MAY 2020')
+    (737547, '2 MAY 2020')
 
     >>> as_numeric_tuple("A19")
     (-1000000000000.0, 'A000000000000019')
 
     >>> as_numeric_tuple("A:1")
     (-1000000000000.0, 'A:000000000000001')
     >>> as_numeric_tuple('"A:19"')
     (-1000000000000.0, '"A:00000000000019"')
 
     >>> as_numeric_tuple("The War of the Roses")
     (-1000000000000.0, 'WAR OF THE ROSES')
 
     >>> as_numeric_tuple("")
-    (-1000000000000.0, '')
+    (1000000000000.0, '')
 
     >>> as_numeric_tuple("50k")
     (50000.0, '50K')
 
     >>> as_numeric_tuple("4 MiB")
     (4194304.0, '4 MIB')
 
@@ -147,26 +147,26 @@
     True
     '''
 
     alpha, omega = -1e12, 1e12
     if backwards:
         alpha, omega = omega, alpha
 
-    if x is None:
+    if x is None or x == '':
         return (omega, '')  # put it at the bottom
 
     x = x.upper()
 
     try:
         return (float(x), x)
     except ValueError:
         pass
 
     try:
-        return (int(tab_fun_dates.parse_date(x).strftime("%s")), x)
+        return (tab_fun_dates.parse_date(x).toordinal(), x)   # make parse date return epoch sec string
     except ValueError:
         pass
 
     # is this a time?
     m = re.match(r'(\d+):([0-5]\d):([0-5]\d(\.\d+)?)', x)
     if m is not None:
         return (int(m.group(1)) * 3600 + int(m.group(2)) * 60 + float(m.group(3)), x)
```

### Comparing `tablinum-0.1.1/tests/test_tab_calculation.py` & `tablinum-0.1.2/tests/test_tab_calculation.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.1/tests/test_tab_command_line.py` & `tablinum-0.1.2/tests/test_tab_command_line.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.1/tests/test_tab_contingency.py` & `tablinum-0.1.2/tests/test_tab_contingency.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.1/tests/test_tab_filter.py` & `tablinum-0.1.2/tests/test_tab_filter.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.1/tests/test_tab_grouping.py` & `tablinum-0.1.2/tests/test_tab_grouping.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.1/tests/test_tab_help.py` & `tablinum-0.1.2/tests/test_tab_help.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.1/tests/test_tab_levels.py` & `tablinum-0.1.2/tests/test_tab_levels.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.1/tests/test_tab_makers.py` & `tablinum-0.1.2/tests/test_tab_makers.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.1/tests/test_tab_parsing.py` & `tablinum-0.1.2/tests/test_tab_parsing.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.1/tests/test_tab_poppers_and_adders.py` & `tablinum-0.1.2/tests/test_tab_poppers_and_adders.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.1/tests/test_tab_roller.py` & `tablinum-0.1.2/tests/test_tab_roller.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.1/tests/test_tab_sort.py` & `tablinum-0.1.2/tests/test_tab_sort.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.1/tests/test_tab_text_manip.py` & `tablinum-0.1.2/tests/test_tab_text_manip.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.1/tests/test_tab_wrangler.py` & `tablinum-0.1.2/tests/test_tab_wrangler.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.1/tests/test_tablinum.py` & `tablinum-0.1.2/tests/test_tablinum.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,15 @@
         self.tab.append(['2011-01-17'])
         self.tab.append(['2011-02-23'])
         self.tab.append(['2011-03-19'])
         self.tab.append(['2011-07-05'])
 
         self.tab.do("arr a{dow(a)}")
         self.assertEqual("\n" + str(self.tab) + "\n", '''
-Date        %a
+Date        dow(Date)
 2011-01-17  Mon
 2011-02-23  Wed
 2011-03-19  Sat
 2011-07-05  Tue
 ''')
 
         self.tab.do("pop 0 arr a{base('2020-05-22')-base(a)}")
```

### Comparing `tablinum-0.1.1/.gitignore` & `tablinum-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.1/LICENSE` & `tablinum-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.1/README.md` & `tablinum-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,33 +5,22 @@
 [![PyPI - Version](https://img.shields.io/pypi/v/tablinum.svg)](https://pypi.org/project/tablinum)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tablinum.svg)](https://pypi.org/project/tablinum)
 
 -----
 
 **Table of Contents**
 
-- [Installation](#installation)
 - [Introduction](#introduction)
-- [Usage modes](#usage-modes)
+- [Usage modes and installation](#usage-modes-and-installation)
 - [Special rows](#special-rows)
 - [Verbs in the DSL](#verbs-in-the-dsl)
 - [What counts as a number?](#what-counts-as-a-number?)
 - [Methods available for a Table object](#methods-available-for-a-table-object)
 - [License](#license)
 
-## Installation
-
-As usual in the modern Python ecosystem, you are recommended to install tablinum in to a virtual 
-environment.  Fortunately it is small and easy to install.  The only prerequisites are the tools 
-used for testing.  Everything else is self-contained, and uses only standard library modules.
-
-```console
-pip install tablinum
-```
-
 
 ## Introduction
 
 Tablinum is an exportable module that will line up tabular material automatically,
 and so save you hours of time faffing about with format and alignment.  As a script
 it provides a filter with a simple DSL (domain-specific language) that can be used
 to make and manipulate tables in editors that support external filters (such as
@@ -78,55 +67,86 @@
 
 Many of my Python scripts create tables of data that I need to share in plain
 text (on Slack for example), and I often found myself loading the output into
 Vim just so I could tidy it up with Tablinum.  So I have re-written my original
 Perl `tabulate` script as a Python package that can be imported, and used to
 tidy up a list of lists of data for printing directly as part of a script.
 
-## Usage modes
+## Usage modes and installation
 
 You can use Tablinum from the command line, from your editor, or as a Python module.
-In each case, you use the same mini-language of verbs to act on your table.  These
-are described in the next main section.
+In each case, you use the same mini-language of verbs to act on your table.  This
+mini-language is described in the next main section.
 
 ### Usage from the command line
 
 The package provides a command line filter "entry point" called `tablinum_filter`. 
-This  lets you get use Tablinum from the command line.  After successful installtion
-you should be able to do `tablinum_filter --h` to get this:
+This lets you get use Tablinum from the command line as a regular script.
+
+If you are always working inside a Python virtual environment, you can install the library
+and the script with:
+
+```console
+pip install tablinum
+```
+
+After successful installation you should be able to do `tablinum_filter --h` from within your 
+virtual environment, to get this:
 
     usage: tablinum_filter [-h] [--file FILE] [agenda [agenda ...]]
 
     positional arguments:
       agenda       [delimiter.maxsplit] [verb [option]]...
 
     optional arguments:
       -h, --help   show this help message and exit
       --file FILE  Source file name, defaults to STDIN
 
 The script can be used with the DSL `gen` to generate data or to read from STDIN
-or from an optional file path.  If you don't like typing such a long name, then
-you could do something like `alias tbl=tablinum_filter`.
+or from an optional file path.  
+
+If you want the script part available globally, then you might prefer to install it using 
+[pipx](https://pipx.pypa.io/stable/installation/).  Once you have `pipx` available on your
+system you should be able to do.
+
+```console
+pipx install tablinum
+```
+
+Then `tablinum_filter` should be available from any command line. 
+
+If you don't like typing such a long name, then you could try something 
+like `alias tbl=tablinum_filter`.
 
 ### Usage from within Vim
 
-Assuming you have installed successfully and you can run `tablinum_filter` from the console
+The Tablinum filter was originally written for use from Vim.  Originally all you 
+had to do was store the whole script locally and set up a command that pointed to it.
+But now that it has grown into a proper Python package with an entry-point script, you
+need to install it in your system and get it working on the command line before you 
+can use it in Vim.  It is theoretically possible to get Vim to work within an activated
+Python virtual environment, but it is probably easier to use `pipx` as shown above.
+
+So, once you have installed successfully and you can run `tablinum_filter` from the console
 then you can use the same filter from within Vim, by adding a line to your `.vimrc` 
 file like this:
 
-    :command! -nargs=* -range=% Table <line1>,<line2>!tablinum_filter <q-args>
+```vimscript
+:command! -nargs=* -range=% Table <line1>,<line2>!tablinum_filter <q-args>
+```
 
 You can of course use some word other than `Table` as the command name. Perhaps
 `Tbl` ?  Take your pick, you can choose anything, except that Vim insists on
 the name starting with an uppercase letter.  
 
 With a definition like this, when you type `:Table` in normal mode in Vim, it
-will pass the current buffer to the script and replace the contents with the output.  
-If you are in Visual Line mode then the current buffer will just be the marked lines.
-If you are in Normal mode then the current buffer will be the whole file.
+will pass the current buffer to the script and replace the contents with the
+output.  If you are in Visual Line mode then the current buffer will just be
+the marked lines.  If you are in Normal mode then the current buffer will be
+the whole file.
 
     :Table [delimiter.maxsplit] [verb [option]]...
 
 ### Writing the agenda line
 
 Whether you are calling Tablinum from Vim or the command line, the
 parsing of your input is the same.
@@ -167,17 +187,24 @@
 it's treated as one.  If it doesn't, it's assumed to be an option.  Anything
 coming after an option, but not recognized as a verb, causes an error.  A
 message will be written back in the file.  You will probably want to use the
 `undo` function after reading it.
 
 ### Usage as a Python library
 
-Tablinum can also be used from your own Python scripts.  If you have data as a
-list of lists, or a  list of strings, then you can use the package to format
-them neatly.  Something like this
+Tablinum can also be used from your own Python projects.  Assuming that you
+are working in a virtual environment, then after you have activated it you can 
+just do 
+```console
+pip install tablinum
+```
+to make the library available.  You might also add it to your `requirements.txt` file.
+
+Once installed you can use the pacakge to parse and format lists of lists or lists
+of strings.  Something like this
 
 ```python
 import tablinum
 data = [('Item', 'Amount'), ('First label', 23), ('Second thing', 45), ('Third one', 55)]
 tt = tablinum.Table()
 tt.parse_lol(data)
 tt.do("rule add")
@@ -194,20 +221,24 @@
 --------------------
 Total            123
 ```
 
 `parse_lol` is expecting a list of lists (or list of iterables) as shown.  But
 you can also use `tt.parse_lines(object_with_lines)` to read a file or a list of strings.
 
-    tt.parse_lines(lines_thing, splitter=re.compile('\\s\\s+'), splits=0)
+```python
+tt.parse_lines(lines_thing, splitter=re.compile('\\s\\s+'), splits=0)
+```
 
 As shown, `parse_lines` takes two optional arguments:  a regex for splitting
 and a maximum number of splits to make, where 0 means "as many as there are".
+The defaults are as shown above -- split on two or more consecutive spaces, and
+make as many splits as needed.
 
-You could also add lines one at a time using the Table.append() method.  So the example
+You can also add lines one at a time using the Table.append() method.  So the example
 above could be done as
 ```python
 import tablinum
 data = [('Item', 'Amount'), ('First label', 23), ('Second thing', 45), ('Third one', 55)]
 tt = tablinum.Table()
 for row in data:
     tt.append(row)
@@ -219,15 +250,15 @@
 
 The `do` method processes a list of verbs and options as described above.
 
 The tabulate module overloads the `__str__` method, so that printing your Table object
 will show it neatly tabulated.  If you want the individual lines, use the `tabulate()` method
 to get a generator of neat lines.
 
-See below for all the public methods provided by a `Table` object.
+See [below](#methods-available-for-a-table-object) for all the public methods provided by a `Table` object.
 
 ## Special rows
 
 Any blank lines in your table are saved as special lines and reinserted at the
 appropriate place on output. So if you have a long table you can use blanks to
 separate blocks of data.  Similarly any lines consisting entirely of `-`
 characters are treated as horizontal rules and reinserted (appropriately sized)
@@ -492,19 +523,24 @@
     ybsorc   CRINES   HobbiesSola    11
     onuj     ARIL     HornCulicid    11
     anhsirk  PARCHED  DebouchMoutan  13
     ellil    GOWD     MediusTanrec   12
 
 There are also some simple date routines included.
 
-- `base` returns the number of days since 1 Jan in the year 1 (assuming the
-  Gregorian calendar extended backwards).  The argument should be blank for
-  today, or some recognisable form of a date.
+- `base` returns an integer representing the number of days since 1 Jan in the
+  year 1 (assuming the Gregorian calendar extended backwards).  The argument
+  should be blank for today, or some recognisable form of a date.  So you can 
+  parse most common date strings.  The default is None, so that you should have
+  `base() == datetime.date.today().toordinal()`
+  
 - `date` does the opposite: given a number that represents the number of days
-  since the year dot, it returns the date in `yyyy-mm-dd` form.  There's also
+  since the year dot, it returns the date in `yyyy-mm-dd` form.  However see below
+  for special cases of small and large values.
+
 - `dow` which takes a date and returns the day of the week, as a three letter
   string.
 
 So given a table with a column of dates, like this
 
     2011-01-17
     2011-02-23
@@ -527,20 +563,24 @@
 
 And `arr a{date(base(a)+140)}` will add 20 weeks to each date
 
     2011-01-17  2011-06-06
     2011-02-23  2011-07-13
     2011-03-19  2011-08-06
 
-As a convenience, if the number given to `date()` is less than 1000, then it's
-assumed that you mean a delta on today rather than a day in the pre-Christian
-era.  So `date(70)` will produce the date in 10 weeks time, and `date(-91)`
-will give you the date three months ago, and so on. `date(0)` or just `date()`
-produces today's date.  If the number you give date is large, it will be
-interpreted as epoch seconds, and if it is very large, epoch milliseconds.
+As a convenience `date()` supports some special ranges of values.
+
+- If the abs value of the number is less than 1000, then it's assumed that you
+  mean a delta on today.  So `date(70)` will produce the date in 10 weeks time,
+  and `date(-91)` will give you the date three months ago, and so on. 
+
+- `date(0)` or just `date()` produces today's date.  
+
+- If the number is larger than `datetime.date.max.toordinal`, then the number
+  will be interpreted as epoch seconds, and if it is very large, epoch milliseconds.
 
 Note: `base()` will actually recognize dates in several different (mainly ISO
 or British) forms as well as `yyyy-mm-dd`, as follows:
 
     Example                   strftime format used
     ----------------------------------------------
     2020-12-25                %Y-%m-%d
@@ -550,22 +590,39 @@
     12/25/20                  %x
     25 December 2020          %d %B %Y
     25 Dec 2020               %d %b %Y
     25 Dec 20                 %d %b %y
     25 December 20            %d %B %y
     25/12/2020                %d/%m/%Y
     25/12/20                  %d/%m/%y
-    Fri                       %a
-    Friday                    %A
     15-dec-2020               %d-%b-%Y
+    Friday                    %A
 
 This table shows the strftime formats used.  This is not as clever as using
 `dateutil.parser` but it does mean that the package only uses the standard Python3
-libraries.  If you want to convert from any of these formats to standard ISO format
-then do `date(base(a))`.
+libraries.  Note that for the last one, you would get the date of next Friday, 
+so `date(base('Monday'))` will give you the date of next Monday in ISO format.
+
+If you want to convert a date in column `a` from any of these formats to
+standard ISO format then do `date(base(a))`. 
+
+If you want something other than ISO date format, then `date()` takes an optional
+second argument that can be any strftime code.  So given the table from above
+
+    2011-01-17
+    2011-02-23
+    2011-03-19
+    2011-07-05
+    
+then `arr a{date(a, "%G-W%V-%u")}` will produce this:
+
+    2011-01-17  2011-W03-1
+    2011-02-23  2011-W08-3
+    2011-03-19  2011-W11-6
+    2011-07-05  2011-W27-2
 
 There are also a few useful functions to convert HH:MM:SS to fractional hours,
 minutes or seconds.  `hms()` takes fractional hours and produces `hh:mm:ss`,
 while `hr`, `mins`, and `secs` go the other way.
 
 Plus `epoch()` that will convert a full date-time timestamp to epoch seconds.
```

### Comparing `tablinum-0.1.1/pyproject.toml` & `tablinum-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
   "pytest",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
-  "coverage report",
+  "coverage report -m",
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
```

### Comparing `tablinum-0.1.1/PKG-INFO` & `tablinum-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tablinum
-Version: 0.1.1
+Version: 0.1.2
 Project-URL: Documentation, https://github.com/unknown/tablinum#readme
 Project-URL: Issues, https://github.com/unknown/tablinum/issues
 Project-URL: Source, https://github.com/unknown/tablinum
 Author-email: Toby Thurston <toby.thurston@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
@@ -26,33 +26,22 @@
 [![PyPI - Version](https://img.shields.io/pypi/v/tablinum.svg)](https://pypi.org/project/tablinum)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tablinum.svg)](https://pypi.org/project/tablinum)
 
 -----
 
 **Table of Contents**
 
-- [Installation](#installation)
 - [Introduction](#introduction)
-- [Usage modes](#usage-modes)
+- [Usage modes and installation](#usage-modes-and-installation)
 - [Special rows](#special-rows)
 - [Verbs in the DSL](#verbs-in-the-dsl)
 - [What counts as a number?](#what-counts-as-a-number?)
 - [Methods available for a Table object](#methods-available-for-a-table-object)
 - [License](#license)
 
-## Installation
-
-As usual in the modern Python ecosystem, you are recommended to install tablinum in to a virtual 
-environment.  Fortunately it is small and easy to install.  The only prerequisites are the tools 
-used for testing.  Everything else is self-contained, and uses only standard library modules.
-
-```console
-pip install tablinum
-```
-
 
 ## Introduction
 
 Tablinum is an exportable module that will line up tabular material automatically,
 and so save you hours of time faffing about with format and alignment.  As a script
 it provides a filter with a simple DSL (domain-specific language) that can be used
 to make and manipulate tables in editors that support external filters (such as
@@ -99,55 +88,86 @@
 
 Many of my Python scripts create tables of data that I need to share in plain
 text (on Slack for example), and I often found myself loading the output into
 Vim just so I could tidy it up with Tablinum.  So I have re-written my original
 Perl `tabulate` script as a Python package that can be imported, and used to
 tidy up a list of lists of data for printing directly as part of a script.
 
-## Usage modes
+## Usage modes and installation
 
 You can use Tablinum from the command line, from your editor, or as a Python module.
-In each case, you use the same mini-language of verbs to act on your table.  These
-are described in the next main section.
+In each case, you use the same mini-language of verbs to act on your table.  This
+mini-language is described in the next main section.
 
 ### Usage from the command line
 
 The package provides a command line filter "entry point" called `tablinum_filter`. 
-This  lets you get use Tablinum from the command line.  After successful installtion
-you should be able to do `tablinum_filter --h` to get this:
+This lets you get use Tablinum from the command line as a regular script.
+
+If you are always working inside a Python virtual environment, you can install the library
+and the script with:
+
+```console
+pip install tablinum
+```
+
+After successful installation you should be able to do `tablinum_filter --h` from within your 
+virtual environment, to get this:
 
     usage: tablinum_filter [-h] [--file FILE] [agenda [agenda ...]]
 
     positional arguments:
       agenda       [delimiter.maxsplit] [verb [option]]...
 
     optional arguments:
       -h, --help   show this help message and exit
       --file FILE  Source file name, defaults to STDIN
 
 The script can be used with the DSL `gen` to generate data or to read from STDIN
-or from an optional file path.  If you don't like typing such a long name, then
-you could do something like `alias tbl=tablinum_filter`.
+or from an optional file path.  
+
+If you want the script part available globally, then you might prefer to install it using 
+[pipx](https://pipx.pypa.io/stable/installation/).  Once you have `pipx` available on your
+system you should be able to do.
+
+```console
+pipx install tablinum
+```
+
+Then `tablinum_filter` should be available from any command line. 
+
+If you don't like typing such a long name, then you could try something 
+like `alias tbl=tablinum_filter`.
 
 ### Usage from within Vim
 
-Assuming you have installed successfully and you can run `tablinum_filter` from the console
+The Tablinum filter was originally written for use from Vim.  Originally all you 
+had to do was store the whole script locally and set up a command that pointed to it.
+But now that it has grown into a proper Python package with an entry-point script, you
+need to install it in your system and get it working on the command line before you 
+can use it in Vim.  It is theoretically possible to get Vim to work within an activated
+Python virtual environment, but it is probably easier to use `pipx` as shown above.
+
+So, once you have installed successfully and you can run `tablinum_filter` from the console
 then you can use the same filter from within Vim, by adding a line to your `.vimrc` 
 file like this:
 
-    :command! -nargs=* -range=% Table <line1>,<line2>!tablinum_filter <q-args>
+```vimscript
+:command! -nargs=* -range=% Table <line1>,<line2>!tablinum_filter <q-args>
+```
 
 You can of course use some word other than `Table` as the command name. Perhaps
 `Tbl` ?  Take your pick, you can choose anything, except that Vim insists on
 the name starting with an uppercase letter.  
 
 With a definition like this, when you type `:Table` in normal mode in Vim, it
-will pass the current buffer to the script and replace the contents with the output.  
-If you are in Visual Line mode then the current buffer will just be the marked lines.
-If you are in Normal mode then the current buffer will be the whole file.
+will pass the current buffer to the script and replace the contents with the
+output.  If you are in Visual Line mode then the current buffer will just be
+the marked lines.  If you are in Normal mode then the current buffer will be
+the whole file.
 
     :Table [delimiter.maxsplit] [verb [option]]...
 
 ### Writing the agenda line
 
 Whether you are calling Tablinum from Vim or the command line, the
 parsing of your input is the same.
@@ -188,17 +208,24 @@
 it's treated as one.  If it doesn't, it's assumed to be an option.  Anything
 coming after an option, but not recognized as a verb, causes an error.  A
 message will be written back in the file.  You will probably want to use the
 `undo` function after reading it.
 
 ### Usage as a Python library
 
-Tablinum can also be used from your own Python scripts.  If you have data as a
-list of lists, or a  list of strings, then you can use the package to format
-them neatly.  Something like this
+Tablinum can also be used from your own Python projects.  Assuming that you
+are working in a virtual environment, then after you have activated it you can 
+just do 
+```console
+pip install tablinum
+```
+to make the library available.  You might also add it to your `requirements.txt` file.
+
+Once installed you can use the pacakge to parse and format lists of lists or lists
+of strings.  Something like this
 
 ```python
 import tablinum
 data = [('Item', 'Amount'), ('First label', 23), ('Second thing', 45), ('Third one', 55)]
 tt = tablinum.Table()
 tt.parse_lol(data)
 tt.do("rule add")
@@ -215,20 +242,24 @@
 --------------------
 Total            123
 ```
 
 `parse_lol` is expecting a list of lists (or list of iterables) as shown.  But
 you can also use `tt.parse_lines(object_with_lines)` to read a file or a list of strings.
 
-    tt.parse_lines(lines_thing, splitter=re.compile('\\s\\s+'), splits=0)
+```python
+tt.parse_lines(lines_thing, splitter=re.compile('\\s\\s+'), splits=0)
+```
 
 As shown, `parse_lines` takes two optional arguments:  a regex for splitting
 and a maximum number of splits to make, where 0 means "as many as there are".
+The defaults are as shown above -- split on two or more consecutive spaces, and
+make as many splits as needed.
 
-You could also add lines one at a time using the Table.append() method.  So the example
+You can also add lines one at a time using the Table.append() method.  So the example
 above could be done as
 ```python
 import tablinum
 data = [('Item', 'Amount'), ('First label', 23), ('Second thing', 45), ('Third one', 55)]
 tt = tablinum.Table()
 for row in data:
     tt.append(row)
@@ -240,15 +271,15 @@
 
 The `do` method processes a list of verbs and options as described above.
 
 The tabulate module overloads the `__str__` method, so that printing your Table object
 will show it neatly tabulated.  If you want the individual lines, use the `tabulate()` method
 to get a generator of neat lines.
 
-See below for all the public methods provided by a `Table` object.
+See [below](#methods-available-for-a-table-object) for all the public methods provided by a `Table` object.
 
 ## Special rows
 
 Any blank lines in your table are saved as special lines and reinserted at the
 appropriate place on output. So if you have a long table you can use blanks to
 separate blocks of data.  Similarly any lines consisting entirely of `-`
 characters are treated as horizontal rules and reinserted (appropriately sized)
@@ -513,19 +544,24 @@
     ybsorc   CRINES   HobbiesSola    11
     onuj     ARIL     HornCulicid    11
     anhsirk  PARCHED  DebouchMoutan  13
     ellil    GOWD     MediusTanrec   12
 
 There are also some simple date routines included.
 
-- `base` returns the number of days since 1 Jan in the year 1 (assuming the
-  Gregorian calendar extended backwards).  The argument should be blank for
-  today, or some recognisable form of a date.
+- `base` returns an integer representing the number of days since 1 Jan in the
+  year 1 (assuming the Gregorian calendar extended backwards).  The argument
+  should be blank for today, or some recognisable form of a date.  So you can 
+  parse most common date strings.  The default is None, so that you should have
+  `base() == datetime.date.today().toordinal()`
+  
 - `date` does the opposite: given a number that represents the number of days
-  since the year dot, it returns the date in `yyyy-mm-dd` form.  There's also
+  since the year dot, it returns the date in `yyyy-mm-dd` form.  However see below
+  for special cases of small and large values.
+
 - `dow` which takes a date and returns the day of the week, as a three letter
   string.
 
 So given a table with a column of dates, like this
 
     2011-01-17
     2011-02-23
@@ -548,20 +584,24 @@
 
 And `arr a{date(base(a)+140)}` will add 20 weeks to each date
 
     2011-01-17  2011-06-06
     2011-02-23  2011-07-13
     2011-03-19  2011-08-06
 
-As a convenience, if the number given to `date()` is less than 1000, then it's
-assumed that you mean a delta on today rather than a day in the pre-Christian
-era.  So `date(70)` will produce the date in 10 weeks time, and `date(-91)`
-will give you the date three months ago, and so on. `date(0)` or just `date()`
-produces today's date.  If the number you give date is large, it will be
-interpreted as epoch seconds, and if it is very large, epoch milliseconds.
+As a convenience `date()` supports some special ranges of values.
+
+- If the abs value of the number is less than 1000, then it's assumed that you
+  mean a delta on today.  So `date(70)` will produce the date in 10 weeks time,
+  and `date(-91)` will give you the date three months ago, and so on. 
+
+- `date(0)` or just `date()` produces today's date.  
+
+- If the number is larger than `datetime.date.max.toordinal`, then the number
+  will be interpreted as epoch seconds, and if it is very large, epoch milliseconds.
 
 Note: `base()` will actually recognize dates in several different (mainly ISO
 or British) forms as well as `yyyy-mm-dd`, as follows:
 
     Example                   strftime format used
     ----------------------------------------------
     2020-12-25                %Y-%m-%d
@@ -571,22 +611,39 @@
     12/25/20                  %x
     25 December 2020          %d %B %Y
     25 Dec 2020               %d %b %Y
     25 Dec 20                 %d %b %y
     25 December 20            %d %B %y
     25/12/2020                %d/%m/%Y
     25/12/20                  %d/%m/%y
-    Fri                       %a
-    Friday                    %A
     15-dec-2020               %d-%b-%Y
+    Friday                    %A
 
 This table shows the strftime formats used.  This is not as clever as using
 `dateutil.parser` but it does mean that the package only uses the standard Python3
-libraries.  If you want to convert from any of these formats to standard ISO format
-then do `date(base(a))`.
+libraries.  Note that for the last one, you would get the date of next Friday, 
+so `date(base('Monday'))` will give you the date of next Monday in ISO format.
+
+If you want to convert a date in column `a` from any of these formats to
+standard ISO format then do `date(base(a))`. 
+
+If you want something other than ISO date format, then `date()` takes an optional
+second argument that can be any strftime code.  So given the table from above
+
+    2011-01-17
+    2011-02-23
+    2011-03-19
+    2011-07-05
+    
+then `arr a{date(a, "%G-W%V-%u")}` will produce this:
+
+    2011-01-17  2011-W03-1
+    2011-02-23  2011-W08-3
+    2011-03-19  2011-W11-6
+    2011-07-05  2011-W27-2
 
 There are also a few useful functions to convert HH:MM:SS to fractional hours,
 minutes or seconds.  `hms()` takes fractional hours and produces `hh:mm:ss`,
 while `hr`, `mins`, and `secs` go the other way.
 
 Plus `epoch()` that will convert a full date-time timestamp to epoch seconds.
```

