# Comparing `tmp/grutil-0.1.4.tar.gz` & `tmp/grutil-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grutil-0.1.4.tar", max compression
+gzip compressed data, was "grutil-0.2.0.tar", max compression
```

## Comparing `grutil-0.1.4.tar` & `grutil-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-23 19:55:13.376022 grutil-0.1.4/grutil/__init__.py
--rw-r--r--   0        0        0      388 2024-04-23 17:34:27.834727 grutil-0.1.4/grutil/afm.py
--rw-r--r--   0        0        0      596 2024-04-23 17:40:10.985103 grutil-0.1.4/grutil/amka.py
--rw-r--r--   0        0        0     4843 2024-04-23 19:46:07.559037 grutil-0.1.4/grutil/dates.py
--rw-r--r--   0        0        0      628 2024-04-23 19:52:08.437928 grutil-0.1.4/grutil/numbers.py
--rw-r--r--   0        0        0      383 2024-04-23 19:06:07.821075 grutil-0.1.4/grutil/text.py
--rw-r--r--   0        0        0      276 2024-04-23 19:59:48.950982 grutil-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       45 2024-04-23 18:22:42.049682 grutil-0.1.4/README.md
--rw-r--r--   0        0        0      376 1970-01-01 00:00:00.000000 grutil-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-23 19:55:13.376022 grutil-0.2.0/grutil/__init__.py
+-rw-r--r--   0        0        0      388 2024-04-23 17:34:27.834727 grutil-0.2.0/grutil/afm.py
+-rw-r--r--   0        0        0      596 2024-04-23 17:40:10.985103 grutil-0.2.0/grutil/amka.py
+-rw-r--r--   0        0        0     4922 2024-04-23 20:28:33.083023 grutil-0.2.0/grutil/dates.py
+-rw-r--r--   0        0        0      695 2024-04-23 20:39:27.875522 grutil-0.2.0/grutil/numbers.py
+-rw-r--r--   0        0        0      383 2024-04-23 19:06:07.821075 grutil-0.2.0/grutil/text.py
+-rw-r--r--   0        0        0      276 2024-04-23 20:49:42.805389 grutil-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-04-23 18:22:42.049682 grutil-0.2.0/README.md
+-rw-r--r--   0        0        0      376 1970-01-01 00:00:00.000000 grutil-0.2.0/PKG-INFO
```

### Comparing `grutil-0.1.4/grutil/amka.py` & `grutil-0.2.0/grutil/amka.py`

 * *Files identical despite different names*

### Comparing `grutil-0.1.4/grutil/dates.py` & `grutil-0.2.0/grutil/dates.py`

 * *Files 16% similar despite different names*

```diff
@@ -52,90 +52,94 @@
     return date(int(year), int(month), int(day))
 
 
 def is_greek_date(grdate: str) -> bool:
     return re.match(r"\d{2}\/\d{2}\/\d{4}", grdate, re.I)
 
 
-def delta_hours(apo: datetime, eos: datetime) -> float:
+def delta_hours(dfrom: datetime, dto: datetime) -> float:
     """Returns hours between two datetime objects"""
-    delta = eos - apo
+    delta = dto - dfrom
     return round(delta.seconds / 3600, 1)
 
 
 def round_half(hours: float) -> float:
-    """Ωρες στρογγυλεμένες ανα μισάωρο"""
+    """Hours rounded to nearest half hour"""
     return round(hours * 2) / 2
 
 
-def daynight_hours(dapo: datetime, deos: datetime) -> dict[str, float]:
+def daynight_hours(dfrom: datetime, dto: datetime) -> dict[str, float]:
     """
     Calculate the number of day and night hours between two datetime objects.
 
     Parameters:
-    - dapo: datetime object representing the start datetime
-    - deos: datetime object representing the end datetime
+    - dfrom: datetime object representing the start datetime
+    - dto: datetime object representing the end datetime
 
     Returns:
     - HOURS object containing the number of day and night hours
     """
     day_start = time(6, 0)  # 6:00 AM
     day_end = time(22, 0)  # 10:00 PM
-    dt_day_start = datetime.combine(dapo, day_start)
-    dt_day_end = datetime.combine(dapo, day_end)
+    dt_day_start = datetime.combine(dfrom, day_start)
+    dt_day_end = datetime.combine(dfrom, day_end)
     dt_next_day_start = dt_day_start + timedelta(days=1)
 
     # dts: dt_day_start, dte: dt_day_end, ndts: dt_next_day_start
     #
     #       dts            dte       ndts
     # 0     6              22        6                22
     #  -----|---------------|--+-----|----------------|--
     # 1  *-*|               |        |
     # 2  *--|----------*    |        |
-    #    *--|---------------|-*      |    Αδύνατο
+    #    *--|---------------|-*      |    impossible
     # 3     |  *--------*   |        |
     # 4     |            *--|------* |
     # 5     |             *-|--------|--*
     # 6     |               |   *---*|
     # 7     |               |   *----|-------*
 
     night_hours = 0
     day_hours = 0
 
     # 1
-    if dapo < dt_day_start and deos <= dt_day_start:
-        night_hours += delta_hours(dapo, deos)
+    if dfrom < dt_day_start and dto <= dt_day_start:
+        night_hours += delta_hours(dfrom, dto)
     # 2
-    elif dapo < dt_day_start and dt_day_start <= deos <= dt_day_end:
-        night_hours += delta_hours(dapo, dt_day_start)
-        day_hours += delta_hours(dt_day_start, deos)
+    elif dfrom < dt_day_start and dt_day_start <= dto <= dt_day_end:
+        night_hours += delta_hours(dfrom, dt_day_start)
+        day_hours += delta_hours(dt_day_start, dto)
     # 3
-    elif dt_day_start <= dapo <= dt_day_end and dt_day_start < deos <= dt_day_end:
-        day_hours += delta_hours(dapo, deos)
+    elif dt_day_start <= dfrom <= dt_day_end and dt_day_start < dto <= dt_day_end:
+        day_hours += delta_hours(dfrom, dto)
     # 4
-    elif dt_day_start < dapo < dt_day_end and dt_day_end < deos <= dt_next_day_start:
-        day_hours += delta_hours(dapo, dt_day_end)
-        night_hours += delta_hours(dt_day_end, deos)
+    elif dt_day_start < dfrom < dt_day_end and dt_day_end < dto <= dt_next_day_start:
+        day_hours += delta_hours(dfrom, dt_day_end)
+        night_hours += delta_hours(dt_day_end, dto)
     # 5
-    elif dt_day_start < dapo < dt_day_end and dt_next_day_start < deos:
-        day_hours += delta_hours(dapo, dt_day_end)
+    elif dt_day_start < dfrom < dt_day_end and dt_next_day_start < dto:
+        day_hours += delta_hours(dfrom, dt_day_end)
         night_hours += delta_hours(dt_day_end, dt_next_day_start)
-        day_hours += delta_hours(dt_next_day_start, deos)
+        day_hours += delta_hours(dt_next_day_start, dto)
     # 6
     elif (
-        dt_day_end <= dapo < dt_next_day_start
-        and dt_day_end < deos <= dt_next_day_start
+        dt_day_end <= dfrom < dt_next_day_start
+        and dt_day_end < dto <= dt_next_day_start
     ):
-        night_hours += delta_hours(dapo, dt_next_day_start)
+        night_hours += delta_hours(dfrom, dt_next_day_start)
     # 7
-    elif dt_day_end <= dapo < dt_next_day_start and dt_next_day_start < deos:
-        night_hours += delta_hours(dapo, dt_next_day_start)
-        day_hours += delta_hours(dt_next_day_start, deos)
+    elif dt_day_end <= dfrom < dt_next_day_start and dt_next_day_start < dto:
+        night_hours += delta_hours(dfrom, dt_next_day_start)
+        day_hours += delta_hours(dt_next_day_start, dto)
     else:
-        raise ValueError(f"Wrong TimeRange {dapo}-{deos}")
+        raise ValueError(f"Wrong TimeRange {dfrom}-{dto}")
 
     return {"day_hours": day_hours, "night_hours": night_hours}
 
 
 def do_overlap(from1: datetime, to1: datetime, from2: datetime, to2: datetime) -> bool:
     """Checks if two time ranges overlap"""
-    return from1 < to2 and from2 < to1
+    return from1 < to2 and from2 < to1
+
+
+def iso2dtime(isodatetime: str) -> datetime :
+    return datetime.fromisoformat(isodatetime)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `grutil-0.1.4/grutil/numbers.py` & `grutil-0.2.0/grutil/numbers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-def float2grnum(val: float, decimals=2) -> str:
+def float2gr(val: float, decimals=2) -> str:
     """1234567.89 => 1.234.567,89"""
     txtfloat = f"{val:,.{decimals}f}"
     return txtfloat.replace(",", "X").replace(".", ",").replace("X", ".")
 
 
-def float2grnum_or_space(val: float, decimals=2) -> str:
+def float2gr_(val: float, decimals=2) -> str:
+    """If val == 0, return empty string"""
     if val == 0:
         return ""
-    return float2grnum(val, decimals)
+    return float2gr(val, decimals)
 
 
-def grnum2float(strval) -> float:
+def gr2float(strval: str) -> float:
     """Greek decimal string to python decimal number
 
+        1.234.567,89 => 1234567.89
+
     :param strval: Greek decimal string
     :param decimals: Number of decimal digits
     :return: Python decimal number
     """
     return float(strval.replace(".", "").replace(",", "."))
```

