# Comparing `tmp/regex_rust-0.1.0rc1-cp312-none-win_amd64.whl.zip` & `tmp/regex_rust-0.2.0-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 701740 bytes, number of entries: 6
--rw-r--r--  4.6 unx     2512 b- defN 24-Apr-20 00:22 regex_rust-0.1.0rc1.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 24-Apr-20 00:22 regex_rust-0.1.0rc1.dist-info/WHEEL
--rw-r--r--  4.6 unx     1099 b- defN 24-Apr-20 00:22 regex_rust-0.1.0rc1.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      111 b- defN 24-Apr-20 00:22 regexrs/__init__.py
--rwxr-xr-x  4.6 unx  1909248 b- defN 24-Apr-20 00:22 regexrs/regexrs.cp312-win_amd64.pyd
--rw-r--r--  4.6 unx      502 b- defN 24-Apr-20 00:22 regex_rust-0.1.0rc1.dist-info/RECORD
-6 files, 1913567 bytes uncompressed, 700834 bytes compressed:  63.4%
+Zip file size: 1721617 bytes, number of entries: 6
+-rw-r--r--  4.6 unx     2549 b- defN 24-Apr-23 23:48 regex_rust-0.2.0.dist-info/METADATA
+-rw-r--r--  4.6 unx      121 b- defN 24-Apr-23 23:48 regex_rust-0.2.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1078 b- defN 24-Apr-23 23:48 regex_rust-0.2.0.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      111 b- defN 24-Apr-23 23:48 regexrs/__init__.py
+-rwxr-xr-x  4.6 unx  5692956 b- defN 24-Apr-23 23:48 regexrs/regexrs.cpython-312-i386-linux-gnu.so
+-rw-r--r--  4.6 unx      501 b- defN 24-Apr-23 23:48 regex_rust-0.2.0.dist-info/RECORD
+6 files, 5697316 bytes uncompressed, 1720715 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: regex_rust-0.1.0rc1.dist-info/METADATA
+Filename: regex_rust-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: regex_rust-0.1.0rc1.dist-info/WHEEL
+Filename: regex_rust-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: regex_rust-0.1.0rc1.dist-info/license_files/LICENSE
+Filename: regex_rust-0.2.0.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: regexrs/__init__.py
 Comment: 
 
-Filename: regexrs/regexrs.cp312-win_amd64.pyd
+Filename: regexrs/regexrs.cpython-312-i386-linux-gnu.so
 Comment: 
 
-Filename: regex_rust-0.1.0rc1.dist-info/RECORD
+Filename: regex_rust-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `regex_rust-0.1.0rc1.dist-info/METADATA` & `regex_rust-0.2.0.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: regex-rust
-Version: 0.1.0rc1
+Version: 0.2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -17,19 +17,22 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 License-File: LICENSE
 Author-email: Spencer Phillip Young <spencer.young@spyoung.com>
 License: MIT
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
-# regexrs
+# regex-rust (regexrs)
 
 Leverages the Rust [`regex` crate](https://crates.io/crates/regex) with PyO3 to create an interface similar to the Python
 standard library `re` module.
 
+```bash
+pip install regex-rust
+```
 
 ```python
 >>> import regexrs as re
 >>> pattern = re.compile(r'(\w+) (\w+)')
 >>> m = pattern.match('hello rust')
 >>> m.groups()
 ('hello', 'rust')
@@ -61,10 +64,10 @@
 regex library for Python today, see the [regex project on PyPI](https://pypi.org/project/regex/).
 
 
 Differences compared to standard lib:
 
 - The `endpos` argument normally found in the `re` module is not supported in `regexrs` for the `match`/`search`/`findall`/`finditer` methods.
 - Some regex features are not supported (because they are not supported by the `regex` crate), such as lookarounds and backreferences.
-- Until a future release, flags are expected to be part of your pattern. For example, instead of passing `re.I` for case-insensitive patterns or other flags, you would write these flags inline like `(?i)` at the beginning of your pattern.
+- Not all flags are supported. At present release, you may use the flags `IGNORECASE`, `MULTILINE`, `DOTALL` and `VERBOSE` (or their shorthand equivalents). These are translated to inline flags and prepended to your given pattern.
 - Until a future release, there is no cache for avoiding re-compiling the same patterns multiple times
```

## Comparing `regex_rust-0.1.0rc1.dist-info/license_files/LICENSE` & `regex_rust-0.2.0.dist-info/license_files/LICENSE`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Spencer Phillip Young
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Spencer Phillip Young
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

