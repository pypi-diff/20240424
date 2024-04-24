# Comparing `tmp/primers-0.5.7-py3-none-any.whl.zip` & `tmp/primers-0.5.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 15733 bytes, number of entries: 13
+Zip file size: 15734 bytes, number of entries: 13
 -rw-r--r--  2.0 unx      450 b- defN 24-Apr-23 14:47 primers/__init__.py
 -rw-r--r--  2.0 unx     4588 b- defN 24-Apr-23 14:47 primers/main.py
 -rw-r--r--  2.0 unx     1662 b- defN 24-Apr-23 14:47 primers/off_targets.py
 -rw-r--r--  2.0 unx    20989 b- defN 24-Apr-23 14:47 primers/primers.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 14:47 tests/__init__.py
 -rw-r--r--  2.0 unx      637 b- defN 24-Apr-23 14:47 tests/off_targets_test.py
 -rw-r--r--  2.0 unx     7539 b- defN 24-Apr-23 14:47 tests/primers_test.py
--rw-r--r--  2.0 unx     1075 b- defN 24-Apr-24 10:11 primers-0.5.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     9291 b- defN 24-Apr-24 10:11 primers-0.5.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 10:11 primers-0.5.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 24-Apr-24 10:11 primers-0.5.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 24-Apr-24 10:11 primers-0.5.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1013 b- defN 24-Apr-24 10:11 primers-0.5.7.dist-info/RECORD
-13 files, 47396 bytes uncompressed, 14051 bytes compressed:  70.4%
+-rw-r--r--  2.0 unx     1075 b- defN 24-Apr-24 10:12 primers-0.5.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9291 b- defN 24-Apr-24 10:12 primers-0.5.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 10:12 primers-0.5.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 24-Apr-24 10:12 primers-0.5.8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 24-Apr-24 10:12 primers-0.5.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1013 b- defN 24-Apr-24 10:12 primers-0.5.8.dist-info/RECORD
+13 files, 47396 bytes uncompressed, 14052 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: tests/off_targets_test.py
 Comment: 
 
 Filename: tests/primers_test.py
 Comment: 
 
-Filename: primers-0.5.7.dist-info/LICENSE
+Filename: primers-0.5.8.dist-info/LICENSE
 Comment: 
 
-Filename: primers-0.5.7.dist-info/METADATA
+Filename: primers-0.5.8.dist-info/METADATA
 Comment: 
 
-Filename: primers-0.5.7.dist-info/WHEEL
+Filename: primers-0.5.8.dist-info/WHEEL
 Comment: 
 
-Filename: primers-0.5.7.dist-info/entry_points.txt
+Filename: primers-0.5.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: primers-0.5.7.dist-info/top_level.txt
+Filename: primers-0.5.8.dist-info/top_level.txt
 Comment: 
 
-Filename: primers-0.5.7.dist-info/RECORD
+Filename: primers-0.5.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `primers-0.5.7.dist-info/LICENSE` & `primers-0.5.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `primers-0.5.7.dist-info/METADATA` & `primers-0.5.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primers
-Version: 0.5.7
+Version: 0.5.8
 Summary: Create PCR primers with optimal lengths, tms, gc%s and free energies
 Home-page: https://github.com/Lattice-Automation/primers
 Author: JJTimmons
 Author-email: jtimmons@latticeautomation.com
 License: mit
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `primers-0.5.7.dist-info/RECORD` & `primers-0.5.8.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 primers/__init__.py,sha256=52ewfExu3E2wvSGRe9W561B0gzw0hFKHv86XKIexBgU,450
 primers/main.py,sha256=_Rrw3-SzfRGAXV4CYuu7XQxcFuVzX19LzlA9_wxu0w4,4588
 primers/off_targets.py,sha256=d7h51TXuBiLvTn7kBpe2txTcSwFFrH4OR3QmQfRpByM,1662
 primers/primers.py,sha256=tEwXj3b9np00wt83nXP5fR2FeTBydvp6lfYmgSysBpc,20989
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/off_targets_test.py,sha256=uOfHXxQVP7YrAb-LrMVgtTgUvmeEsuG6coZ_arFODA4,637
 tests/primers_test.py,sha256=Z7Wxzg4vyKPzWXS44lABvrfQRQQt2DkimZQ6PC_8qsA,7539
-primers-0.5.7.dist-info/LICENSE,sha256=7Vk9JLhU9IE6g8bAeeneyADepMrJMrzv-ZK9bUYtrOo,1075
-primers-0.5.7.dist-info/METADATA,sha256=-mLa5JKW6nnCWiyt-3hQU4Ov48gqv704z5W-mTM9J5I,9291
-primers-0.5.7.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-primers-0.5.7.dist-info/entry_points.txt,sha256=3O_amguYXQnwLM7AO9PFZS9ILKYOujgA-pjyJ-Tnm48,46
-primers-0.5.7.dist-info/top_level.txt,sha256=aArUtmNkt-jC7HpfQUFIsKSBVNchrbl5EEo1-JBoI8k,14
-primers-0.5.7.dist-info/RECORD,,
+primers-0.5.8.dist-info/LICENSE,sha256=7Vk9JLhU9IE6g8bAeeneyADepMrJMrzv-ZK9bUYtrOo,1075
+primers-0.5.8.dist-info/METADATA,sha256=DtjGajU8u2MAndAs7LxkCyKGSz2frcyPafkT0YuvHug,9291
+primers-0.5.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+primers-0.5.8.dist-info/entry_points.txt,sha256=3O_amguYXQnwLM7AO9PFZS9ILKYOujgA-pjyJ-Tnm48,46
+primers-0.5.8.dist-info/top_level.txt,sha256=aArUtmNkt-jC7HpfQUFIsKSBVNchrbl5EEo1-JBoI8k,14
+primers-0.5.8.dist-info/RECORD,,
```

