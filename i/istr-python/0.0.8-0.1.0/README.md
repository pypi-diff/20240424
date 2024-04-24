# Comparing `tmp/istr_python-0.0.8.tar.gz` & `tmp/istr_python-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istr_python-0.0.8.tar", last modified: Thu Apr 18 07:29:38 2024, max compression
+gzip compressed data, was "istr_python-0.1.0.tar", last modified: Wed Apr 24 16:01:57 2024, max compression
```

## Comparing `istr_python-0.0.8.tar` & `istr_python-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 07:29:38.146533 istr_python-0.0.8/
--rw-rw-rw-   0        0        0     6551 2024-04-18 07:29:38.144531 istr_python-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5782 2024-04-18 07:29:24.000000 istr_python-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 07:29:38.119970 istr_python-0.0.8/istr/
--rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-0.0.8/istr/__init__.py
--rw-rw-rw-   0        0        0     7734 2024-04-14 16:04:53.000000 istr_python-0.0.8/istr/install istr.py
--rw-rw-rw-   0        0        0    12812 2024-04-18 07:26:37.000000 istr_python-0.0.8/istr/istr.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:29:38.143533 istr_python-0.0.8/istr_python.egg-info/
--rw-rw-rw-   0        0        0     6551 2024-04-18 07:29:38.000000 istr_python-0.0.8/istr_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-04-18 07:29:38.000000 istr_python-0.0.8/istr_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 07:29:38.000000 istr_python-0.0.8/istr_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-18 07:29:38.000000 istr_python-0.0.8/istr_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      744 2024-04-18 07:29:32.000000 istr_python-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-18 07:29:38.147532 istr_python-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-18 07:29:38.140544 istr_python-0.0.8/tests/
--rw-rw-rw-   0        0        0     9682 2024-04-17 07:00:43.000000 istr_python-0.0.8/tests/test_istr.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:01:57.723514 istr_python-0.1.0/
+-rw-rw-rw-   0        0        0    10346 2024-04-24 16:01:57.720511 istr_python-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9419 2024-04-24 14:54:22.000000 istr_python-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 16:01:57.666693 istr_python-0.1.0/istr/
+-rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-0.1.0/istr/__init__.py
+-rw-rw-rw-   0        0        0     7734 2024-04-14 16:04:53.000000 istr_python-0.1.0/istr/install istr.py
+-rw-rw-rw-   0        0        0    15553 2024-04-24 12:19:57.000000 istr_python-0.1.0/istr/istr.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:01:57.713932 istr_python-0.1.0/istr_python.egg-info/
+-rw-rw-rw-   0        0        0    10346 2024-04-24 16:01:57.000000 istr_python-0.1.0/istr_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-04-24 16:01:57.000000 istr_python-0.1.0/istr_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 16:01:57.000000 istr_python-0.1.0/istr_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-24 16:01:57.000000 istr_python-0.1.0/istr_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      744 2024-04-24 16:01:50.000000 istr_python-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-24 16:01:57.724954 istr_python-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 16:01:57.706870 istr_python-0.1.0/tests/
+-rw-rw-rw-   0        0        0    11213 2024-04-23 14:50:53.000000 istr_python-0.1.0/tests/test_istr.py
```

### Comparing `istr_python-0.0.8/istr/install istr.py` & `istr_python-0.1.0/istr/install istr.py`

 * *Files identical despite different names*

### Comparing `istr_python-0.0.8/istr/istr.py` & `istr_python-0.1.0/istr/istr.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,188 @@
-from functools import partial
+import functools
 import math
-import contextlib
+
 
 #   _       _
 #  (_) ___ | |_  _ __
 #  | |/ __|| __|| '__|
 #  | |\__ \| |_ | |
 #  |_||___/ \__||_|    use strings as integers
 
-__version__ = "0.0.8"
+__version__ = "0.1.0"
+
+"""
+changelog
+
+version 0.1.0  2024-04-22  
+-------------------------
+Changed the way istr.range is implemenented.
+
+Changed the context manager istr.format() to be used directly without the with statement.
+Also, noww istr.format() works without any argument and then returns the current format.
+
+istr class now uses __slots__
+
+All internal values and methods now start with an underscore.
+
+Introduced istr.repr_mode()
+
+Introduced istr.base()
+
+Extended tests for new functionality
+
+
+version 0.0.8  2024-04-18  
+-------------------------
+initial version with changelog
+"""
+
+class _range:
+    """
+    based on https://codereview.stackexchange.com/questions/229073/pure-python-range-implementation
+    """
+
+    def __init__(self, cls, start, stop=None, step=1):
+        if stop is None:
+            start, stop = 0, start
+        self.start, self.stop, self.step = (int(obj) for obj in (start, stop, step))
+        if step == 0:
+            raise ValueError("range() arg 3 must not be zero")
+        if self.step < 0:
+            step_sign = -1
+        else:
+            step_sign = 1
+        self._len = max(1 + (self.stop - self.start - step_sign) // self.step, 0)
+        self.parent_cls = cls
+
+    def __contains__(self, value):
+        if isinstance(value, int):
+            return self._index(value) != -1
+        return any(n == value for n in self)
+
+    def __eq__(self, other):
+        if not isinstance(other, type(self)):
+            return False
+        if self._len != len(other):
+            return False
+        if self._len == 0:
+            return True
+        if self.start != other.start:
+            return False
+        if self[-1] == other[-1]:
+            return True
+        return False
+
+    def __getitem__(self, index):
+        def adjust_indices(length, start, stop, step):
+            if step is None:
+                step = 1
+            else:
+                step = int(step)
+
+            if start is None:
+                start = length - 1 if step < 0 else 0
+            else:
+                start = int(start)
+                if start < 0:
+                    start += length
+                    if start < 0:
+                        start = -1 if step < 0 else 0
+                elif start >= length:
+                    start = length - 1 if step < 0 else length
+
+            if stop is None:
+                stop = -1 if step < 0 else length
+            else:
+                stop = int(stop)
+                if stop < 0:
+                    stop += length
+                    if stop < 0:
+                        stop = -1 if step < 0 else 0
+                elif stop >= length:
+                    stop = length - 1 if step < 0 else length
+
+            return start, stop, step
+
+        if isinstance(index, slice):
+            start, stop, step = adjust_indices(self._len, index.start, index.stop, index.step)
+            return self.parent_cls.range(self.start + self.step * start, self.start + self.step * stop, self.step * step)
+        index = int(index)
+        if index < 0:
+            index += self._len
+        if not 0 <= index < self._len:
+            raise IndexError("range object index out of range")
+        return self.parent_cls(self.start + self.step * index)
+
+    def __hash__(self):
+        if self._len == 0:
+            return id(self.parent_cls.range)
+        return hash((self._len, self.start, int(self[-1])))
+
+    def __iter__(self):
+        value = self.start
+        if self.step > 0:
+            while value < self.stop:
+                yield self.parent_cls(value)
+                value += self.step
+        else:
+            while value > self.stop:
+                yield self.parent_cls(value)
+                value += self.step
+
+    def __len__(self):
+        return self._len
+
+    def __repr__(self):
+        if self.step == 1:
+            return f"{self.parent_cls.__name__}.range({self.start}, {self.stop})"
+        return f"{self.parent_cls.__name__}.range({self.start}, {self.stop}, {self.step})"
+
+    def __reversed__(self):
+        return iter(self[::-1])
+
+    def _index(self, value):
+        index_mul_step = value - self.start
+        if index_mul_step % self.step:
+            return -1
+        index = index_mul_step // self.step
+        if 0 <= index < self._len:
+            return index
+        return -1
+
+    def count(self, value):
+        """
+        Rangeobject.count(value) -> integer
+        Return number of occurrences of value.
+        """
+        return sum(1 for n in self if int(n) == int(value))
+
+    def index(self, value, start=0, stop=None):
+        if start < 0:
+            start = max(self._len + start, 0)
+        if stop is None:
+            stop = self._len
+        if stop < 0:
+            stop += self._len
+
+        if isinstance(value, int):
+            index = self._index(value)
+            if start <= index < stop:
+                return index
+            raise ValueError(f"{value} is not in range")
+
+        i = start
+        n = self.start + self.step * i
+        while i < stop:
+            if n == int(value):
+                return i
+            i += 1
+            n += self.step
+        raise ValueError(f"{value} is not in range")
+
 
 class istr(str):
     """
     istr object
 
     Parameters
     ----------
@@ -34,364 +204,306 @@
             istr(range(3)) ==> istr.range(3)
             list(istr(range(3))) ==> [istr("0"), istr("1"), istr("2")]
             len(istr(range(3))) ==> 3
 
         it is possible to give more than one parameter, in which case a tuple
         of the istrs of the parameters will be returned, which can be handy
         to multiple assign, e.g.
-            a, b, c = istr(5, 6, 7) ==> a=istr("5") , b=istr("6"), c=istr("7")
-"""
+            a, b, c = istr(5, 6, 7) ==> a=istr("5") , b=istr("6"), c=istr("7")"""
+
+    __slots__ = ("_as_int", "_as_repr")
 
     _format = ""
+    _mode = "istr"
+    _base = 10
+
+    @staticmethod
+    def _to_base(number, base):
+        if number < 0:
+            raise ValueError(f"negative numbers are not allowed for base {base}")
+        result = ""
+        while number:
+            result += "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ"[number % base]
+            number //= base
+        return result[::-1] or "0"
 
     @classmethod
-    def toint(cls, value):
+    def _to_int(cls, value):
         try:
-            return int(value)
+            if cls._base != 10 and isinstance(value, str):
+                return int(value, cls._base)
+            else:
+                return int(value)
         except (ValueError, TypeError):
-            raise ValueError(f"unable to convert {repr(value)} to int")
-
-    @classmethod
-    def check_format(cls, format):
-        if format is None:
-            return cls._format
-        if not (isinstance(format, str) and all(x in "0123456789" for x in format)):
-            raise ValueError(f"{repr(format)} is incorrect format")
-        return format
+            raise ValueError(f"unable to convert {repr(value)} to int (base {cls._base})")
 
     def __new__(cls, *value):
         if len(value) == 0:
             raise TypeError("no parameter given")
         if len(value) == 1:
             value = value[0]  # normal case of 1 parameter
         if isinstance(value, range):
             return cls.range(value.start, value.stop, value.step)
+        if isinstance(value, _range):
+            return value
         if isinstance(value, dict):
             return type(value)((k, cls(v)) for k, v in value.items())
         if not isinstance(value, (str, type)) and hasattr(value, "__iter__"):
-            if hasattr(value, "__next__") or type(value) == range:
-                return map(partial(cls), value)
-            return type(value)(map(partial(cls), value))
+            if hasattr(value, "__next__"):
+                return map(functools.partial(cls), value)
+            return type(value)(map(functools.partial(cls), value))
         if value == "":
-            asstr = ""
-            asint = 0
+            as_str = ""
+            as_int = 0
         else:
-            asint = cls.toint(value)
-            if cls._format == "":
+            as_int = cls._to_int(value)
+            if cls._format == "" or cls._base != 10:
                 if isinstance(value, str):
-                    asstr = value
+                    as_str = value
                 else:
-                    asstr = str(asint)
+                    if cls._base == 10:
+                        as_str = str(as_int)
+                    else:
+                        as_str = istr._to_base(as_int, cls._base)
             else:
-                asstr = f"{asint:{cls._format}}"
+                as_str = f"{as_int:{cls._format}}"
 
-        self = super().__new__(cls, asstr)
-        self.asint = asint
+        self = super().__new__(cls, as_str)
+        self._as_int = as_int
+        if self._mode == "istr":
+            self._as_repr = f"{cls.__name__}({repr(as_str)})"
+        elif self._mode == "int":
+            self._as_repr = repr(as_int)
+        else:
+            self._as_repr = repr(as_str)
         return self
 
     def __hash__(self):
         return hash((self.__class__, str(self)))
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
-            return self.asint == other.asint
+            return self._as_int == other._as_int
         if isinstance(other, str):
             return super().__eq__(other)
         try:
-            return self.asint == self.toint(other)
+            return self._as_int == self._to_int(other)
         except Exception:
             return False
 
     def __ne__(self, other):
         return not self == other
 
     def __contains__(self, other):
         return super().__contains__(str(other))
 
     def __repr__(self):
-        return f"{self.__class__.__name__}({super().__repr__()})"
+        return self._as_repr
 
     def __le__(self, other):
-        return self.asint <= self.toint(other)
+        return self._as_int <= self._to_int(other)
 
     def __lt__(self, other):
-        return self.asint < self.toint(other)
+        return self._as_int < self._to_int(other)
 
     def __ge__(self, other):
-        return self.asint >= self.toint(other)
+        return self._as_int >= self._to_int(other)
 
     def __gt__(self, other):
-        return self.asint > self.toint(other)
+        return self._as_int > self._to_int(other)
 
     def __bool__(self):
-        return bool(self.asint)
+        return bool(self._as_int)
 
     def __add__(self, other):
-        return self.__class__(self.asint + self.toint(other))
+        return self.__class__(self._as_int + self._to_int(other))
 
     def __sub__(self, other):
-        return self.__class__(self.asint - self.toint(other))
+        return self.__class__(self._as_int - self._to_int(other))
 
     def __mul__(self, other):
-        return self.__class__(self.asint * self.toint(other))
+        return self.__class__(self._as_int * self._to_int(other))
 
     def __floordiv__(self, other):
-        return self.__class__(self.asint // self.toint(other))
+        return self.__class__(self._as_int // self._to_int(other))
 
     def __rfloordiv__(self, other):
-        return self.__class__(self.toint(other) // self.asint)
+        return self.__class__(self._to_int(other) // self._as_int)
 
     def __truediv__(self, other):
-        return self.__class__(self.asint // self.toint(other))
+        return self.__class__(self._as_int // self._to_int(other))
 
     def __rtruediv__(self, other):
-        return self.__class__(self.toint(other) // self.asint)
+        return self.__class__(self._to_int(other) // self._as_int)
 
     def __pow__(self, other):
-        return self.__class__(self.asint ** self.toint(other))
+        return self.__class__(self._as_int ** self._to_int(other))
 
     def __rpow__(self, other):
-        return self.__class__(self.toint(other) ** self.asint)
+        return self.__class__(self._to_int(other) ** self._as_int)
 
     def __radd__(self, other):
-        return self.__class__(self.toint(other) + self.asint)
+        return self.__class__(self._to_int(other) + self._as_int)
 
     def __rsub__(self, other):
-        return self.__class__(self.toint(other) - self.asint)
+        return self.__class__(self._to_int(other) - self._as_int)
 
     def __rmul__(self, other):
-        return self.__class__(self.toint(other) * self.asint)
+        return self.__class__(self._to_int(other) * self._as_int)
 
     def __mod__(self, other):
-        return self.__class__(self.asint % self.toint(other))
+        return self.__class__(self._as_int % self._to_int(other))
 
     def __rmod__(self, other):
-        return self.__class__(self.toint(other) % self.asint)
+        return self.__class__(self._to_int(other) % self._as_int)
 
     def __or__(self, other):
         return self.__class__("".join((self, self.__class__(other))))
 
     def __ror__(self, other):
         return self.__class__("".join((self.__class__(other), self)))
 
     def __int__(self):
-        return int(self.asint)
+        return int(self._as_int)
 
     def __round__(self):
-        return self.__class__(round(self.asint))
+        return self.__class__(round(self._as_int))
 
     def __trunc__(self):
-        return self.__class__(math.trunc(self.asint))
+        return self.__class__(math.trunc(self._as_int))
 
     def __floor__(self):
-        return self.__class__(math.floor(self.asint))
+        return self.__class__(math.floor(self._as_int))
 
     def __ceil__(self):
-        return self.__class__(math.ceil(self.asint))
+        return self.__class__(math.ceil(self._as_int))
 
     def __matmul__(self, other):
         return self.__class__(super().__mul__(other))
 
     def __rmatmul__(self, other):
         return self.__class__(super().__rmul__(other))
 
     def __divmod__(self, other):
-        return self.__class__(divmod(self.asint, self.toint(other)))
+        return self.__class__(divmod(self._as_int, self._to_int(other)))
 
     def __rdivmod__(self, other):
-        return self.__class__(divmod(self.toint(other), self.asint))
+        return self.__class__(divmod(self._to_int(other), self._as_int))
 
     def __neg__(self):
-        return self.__class__(-self.asint)
+        return self.__class__(-self._as_int)
 
     def __pos__(self):
         return self
 
     def __abs__(self):
-        return self.__class__(abs(self.asint))
+        return self.__class__(abs(self._as_int))
 
     def is_even(self):
-        return self.asint % 2 == 0
+        return self._as_int % 2 == 0
 
     def is_odd(self):
-        return self.asint % 2 == 1
+        return self._as_int % 2 == 1
 
     def join(self, iterable):
         s = super().join(iterable)
         return self.__class__(s)
 
     def reversed(self):
         return self[::-1]
 
     def __getitem__(self, key):
         return self.__class__(super().__getitem__(key))
 
     @classmethod
+    def concat(cls, iterable):
+        return map(lambda x: istr("").join(x), istr(iterable))
+
+    @classmethod
     def enumerate(cls, iterable, start=0):
         for i, value in enumerate(iterable, start):
             yield cls(i), value
 
     @classmethod
-    @contextlib.contextmanager
-    def format(cls, format):
-        saved_format = cls._format
-        cls._format = cls.check_format(format)
-        yield
-        cls._format = saved_format
+    class format:
+        def __new__(cls, cls_format, format=None):
+            if format is None:
+                return cls_format._format
+            return super().__new__(cls)
+
+        def __init__(self, cls, format):
+            self.saved_format = cls._format
+            self.saved_cls = cls
+            if not (isinstance(format, str) and all(x in "0123456789" for x in format)):
+                raise ValueError(f"{repr(format)} is incorrect format")
 
-    @classmethod
-    def default_format(cls, format=None):
-        if format is not None:
-            cls._format = cls.check_format(format)
-        return cls._format
+            cls._format = format
+
+        def __enter__(self):
+            ...
+
+        def __exit__(self, exc_type, exc_value, exc_tb):
+            self.saved_cls._format = self.saved_format
 
     @classmethod
-    class range:
-        """
-        based on https://codereview.stackexchange.com/questions/229073/pure-python-range-implementation
-        """
+    class repr_mode:
+        def __new__(cls, cls_mode, mode=None):
+            if mode is None:
+                return cls_mode._mode
+            if mode in ("istr", "str", "int"):
+                return super().__new__(cls)
+            raise TypeError(f"mode not 'istr', 'str' or 'int', but {repr(mode)}")
+
+        def __init__(self, cls, mode):
+            self.saved_mode = cls._mode
+            self.saved_cls = cls
+            cls._mode = mode
 
-        def __init__(self, cls, start, stop=None, step=1):
-            if stop is None:
-                start, stop = 0, start
-            self.start, self.stop, self.step = (int(obj) for obj in (start, stop, step))
-            if step == 0:
-                raise ValueError("range() arg 3 must not be zero")
-            if self.step < 0:
-                step_sign = -1
-            else:
-                step_sign = 1
-            self._len = max(1 + (self.stop - self.start - step_sign) // self.step, 0)
-            self.parent_cls = cls
-
-        def __contains__(self, value):
-            if isinstance(value, int):
-                return self._index(value) != -1
-            return any(n == value for n in self)
-
-        def __eq__(self, other):
-            if not isinstance(other, type(self)):
-                return False
-            if self._len != len(other):
-                return False
-            if self._len == 0:
-                return True
-            if self.start != other.start:
-                return False
-            if self[-1] == other[-1]:
-                return True
-            return False
+        def __enter__(self):
+            ...
 
-        def __getitem__(self, index):
-            def adjust_indices(length, start, stop, step):
-                if step is None:
-                    step = 1
-                else:
-                    step = int(step)
+        def __exit__(self, exc_type, exc_value, exc_tb):
+            self.saved_cls._mode = self.saved_mode
 
-                if start is None:
-                    start = length - 1 if step < 0 else 0
-                else:
-                    start = int(start)
-                    if start < 0:
-                        start += length
-                        if start < 0:
-                            start = -1 if step < 0 else 0
-                    elif start >= length:
-                        start = length - 1 if step < 0 else length
+    @classmethod
+    class base:
+        def __new__(cls, cls_base, base=None):
+            if base is None:
+                return cls_base._base
+            if 2 <= base <= 36:
+                return super().__new__(cls)
+            raise ValueError(f"base not between 2 and 36, but {base}")
+
+        def __init__(self, cls, base):
+            self.saved_base = cls._base
+            self.saved_cls = cls
+            cls._base = base
 
-                if stop is None:
-                    stop = -1 if step < 0 else length
-                else:
-                    stop = int(stop)
-                    if stop < 0:
-                        stop += length
-                        if stop < 0:
-                            stop = -1 if step < 0 else 0
-                    elif stop >= length:
-                        stop = length - 1 if step < 0 else length
-
-                return start, stop, step
-
-            if isinstance(index, slice):
-                start, stop, step = adjust_indices(self._len, index.start, index.stop, index.step)
-                return self.parent_cls.range(self.start + self.step * start, self.start + self.step * stop, self.step * step)
-            index = int(index)
-            if index < 0:
-                index += self._len
-            if not 0 <= index < self._len:
-                raise IndexError("range object index out of range")
-            return self.parent_cls(self.start + self.step * index)
-
-        def __hash__(self):
-            if self._len == 0:
-                return id(self.parent_cls.range)
-            return hash((self._len, self.start, int(self[-1])))
-
-        def __iter__(self):
-            value = self.start
-            if self.step > 0:
-                while value < self.stop:
-                    yield self.parent_cls(value)
-                    value += self.step
-            else:
-                while value > self.stop:
-                    yield self.parent_cls(value)
-                    value += self.step
-
-        def __len__(self):
-            return self._len
-
-        def __repr__(self):
-            if self.step == 1:
-                return f"{self.parent_cls.__name__}.range({self.start}, {self.stop})"
-            return f"{self.parent_cls.__name__}.range({self.start}, {self.stop}, {self.step})"
-
-        def __reversed__(self):
-            return iter(self[::-1])
-
-        def _index(self, value):
-            index_mul_step = value - self.start
-            if index_mul_step % self.step:
-                return -1
-            index = index_mul_step // self.step
-            if 0 <= index < self._len:
-                return index
-            return -1
+        def __enter__(self):
+            ...
+
+        def __exit__(self, exc_type, exc_value, exc_tb):
+            self.saved_cls._base = self.saved_base
+
+    @classmethod
+    def range(cls, start,stop=None,step=1):
+        return _range(cls,start,stop,step) 
 
-        def count(self, value):
-            """
-            Rangeobject.count(value) -> integer
-            Return number of occurrences of value.
-            """
-            return sum(1 for n in self if int(n) == int(value))
-
-        def index(self, value, start=0, stop=None):
-            if start < 0:
-                start = max(self._len + start, 0)
-            if stop is None:
-                stop = self._len
-            if stop < 0:
-                stop += self._len
-
-            if isinstance(value, int):
-                index = self._index(value)
-                if start <= index < stop:
-                    return index
-                raise ValueError(f"{value} is not in range")
-
-            i = start
-            n = self.start + self.step * i
-            while i < stop:
-                if n == int(value):
-                    return i
-                i += 1
-                n += self.step
-            raise ValueError(f"{value} is not in range")
 
 
 def main():
-    for i,c in istr.enumerate("abc"):
-        print(f"{i!r} {c}")
+    print(repr(istr("  12")))
+    with istr.base(16):
+        print(repr(istr("  12")))
+
+
+    with istr.format("05"):
+        print(repr(istr("  12")))
+        print(repr(istr(12)))
+        with istr.base(16):
+            print(repr(istr("   12")))
+
+
 
 if __name__ == "__main__":
     main()
+
```

### Comparing `istr_python-0.0.8/pyproject.toml` & `istr_python-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "istr-python"
 authors = [
     {name = "Ruud van der Ham", email = "rt.van.der.ham@gmail.com"}
 ]
 description = "istr is a module to use strings as if they were integers."
-version = "0.0.8"
+version = "0.1.0"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
 ]
 classifiers = [
   # How mature is this project? Common values are
   #   3 - Alpha
```

### Comparing `istr_python-0.0.8/tests/test_istr.py` & `istr_python-0.1.0/tests/test_istr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import math
+import itertools
 
 if __name__ == "__main__":  # to make the tests run without the pytest cli
     import sys
 
     sys.path = ["../istr"] + sys.path
 
 import pytest
@@ -131,15 +132,20 @@
     assert two != istr
 
 
 def test_order():
     assert " ".join(sorted(istr.range(1, 13))) == "1 2 3 4 5 6 7 8 9 10 11 12"
     assert " ".join(sorted(map(istr, range(1, 13)))) == "1 2 3 4 5 6 7 8 9 10 11 12"
 
-
+def test_concat():
+    c = list(istr.concat(((1,2),(3,4))))
+    assert c == istr(['12','34'])
+    c=list(istr.concat(itertools.permutations(range(3),2)))
+    assert c == [istr('01'), istr('02'), istr('10'), istr('12'), istr('20'), istr('21')]
+    
 def test_range():
     assert one_to_twelve == istr.range("1", "13")
     assert one_to_twelve == istr.range(one, thirteen, one)
     assert one_to_twelve == istr(range(1, 13))
 
     assert len(one_to_twelve) == 12
     assert 2 in one_to_twelve
@@ -262,19 +268,19 @@
         with istr.format("a"):
             ...
     with pytest.raises(ValueError):
         with istr.format(1):
             ...
     with istr.format("0"):
         assert istr(" 3 ") == "3"
-    assert istr.default_format() == ""
-    istr.default_format("03")
-    assert istr.default_format() == "03"
+    assert istr.format() == ""
+    istr.format("03")
+    assert istr.format() == "03"
     assert istr("  8 ") == "008"
-    istr.default_format("")
+    istr.format("")
     assert istr(" 8 ") == " 8 "
 
 
 def test_range_format():
     r = istr.range(11)
     assert repr(r) == "istr.range(0, 11)"
     assert " ".join(r) == "0 1 2 3 4 5 6 7 8 9 10"
@@ -319,14 +325,15 @@
     with pytest.raises(TypeError):
         three @ five
     with pytest.raises(TypeError):
         three @ "5"
     with pytest.raises(TypeError):
         "3" @ five
 
+
 def test_str():
     assert repr(str(five)) == "'5'"
 
 
 def test_trunc_and_friends():
     assert math.trunc(one).equals(istr("1"))
     assert math.ceil(one).equals(istr("1"))
@@ -364,27 +371,83 @@
     with pytest.raises(ValueError):
         istr("ab")
     with pytest.raises(ValueError):
         istr(istr)
     assert istr(istr(one)).equals(istr("1"))
     with pytest.raises(TypeError):
         istr()
-
+    rng=istr.range(5)
+    assert rng is istr(rng)
 
 def test_unpacking():
     a = istr("123")
     x, y, z = istr(*a)
     assert x.equals(istr(1))
     assert y.equals(istr(2))
     assert z.equals(istr(3))
 
 
+def test_repr_mode():
+    hundred = istr(100)
+    assert repr(hundred) == "istr('100')"
+
+    with istr.repr_mode("istr"):
+        hundred = istr(100)
+    assert repr(hundred) == "istr('100')"
+
+    with istr.repr_mode("int"):
+        hundred = istr(100)
+    assert repr(hundred) == "100"
+    with istr.repr_mode("str"):
+        hundred = istr(100)
+    assert repr(hundred) == "'100'"
+    hundred = istr(100)
+    assert repr(hundred) == "istr('100')"
+
+    assert istr.repr_mode() == "istr"
+
+    with pytest.raises(TypeError):
+        istr.repr_mode("no")
+
+
+def test_base():
+    assert istr.base() == 10
+    with istr.base(16):
+        a = istr("7fff")
+        assert a == 32767
+        assert a == "7fff"
+        b = istr("3fff")
+        c = a - b
+        assert c == istr("4000")
+        assert c == 2**14
+    assert istr.base() == 10
+    with istr.base(36):
+        a = istr("PA7")
+        assert a == 32767
+
+    with istr.base(2):
+        a = istr("111")
+        assert a == 7
+        b = a - istr("110")
+        assert repr(b) == "istr('1')"
+
+    with pytest.raises(ValueError):
+        istr.base(1)
+    with pytest.raises(ValueError):
+        istr.base(37)
+
+    with pytest.raises(ValueError):
+        with istr.base(16):
+            istr(-1)
+
+
 def test_subclassing():
     class jstr(istr):
         ...
 
     assert jstr(5).equals(jstr(5))
     assert repr(jstr(*range(3))) == "(jstr('0'), jstr('1'), jstr('2'))"
 
 
 if __name__ == "__main__":
     pytest.main(["-vv", "-s", "-x", __file__])
+
```

