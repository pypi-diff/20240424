# Comparing `tmp/anycrc-0.3.3.tar.gz` & `tmp/anycrc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycrc-0.3.3.tar", last modified: Sat Apr 20 04:38:25 2024, max compression
+gzip compressed data, was "anycrc-0.4.0.tar", last modified: Tue Apr 23 19:27:28 2024, max compression
```

## Comparing `anycrc-0.3.3.tar` & `anycrc-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:38:25.178666 anycrc-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-20 04:38:20.000000 anycrc-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-20 04:38:25.178666 anycrc-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-20 04:38:20.000000 anycrc-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:38:25.174666 anycrc-0.3.3/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:38:25.178666 anycrc-0.3.3/lib/crcany/
--rw-r--r--   0 runner    (1001) docker     (127)    22314 2024-04-20 04:38:20.000000 anycrc-0.3.3/lib/crcany/crc.c
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-20 04:38:20.000000 anycrc-0.3.3/lib/crcany/crc.h
--rw-r--r--   0 runner    (1001) docker     (127)    18683 2024-04-20 04:38:20.000000 anycrc-0.3.3/lib/crcany/model.c
--rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-04-20 04:38:20.000000 anycrc-0.3.3/lib/crcany/model.h
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-20 04:38:20.000000 anycrc-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 04:38:25.178666 anycrc-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-20 04:38:20.000000 anycrc-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:38:25.174666 anycrc-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:38:25.178666 anycrc-0.3.3/src/anycrc/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-20 04:38:20.000000 anycrc-0.3.3/src/anycrc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-20 04:38:20.000000 anycrc-0.3.3/src/anycrc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   445287 2024-04-20 04:38:24.000000 anycrc-0.3.3/src/anycrc/anycrc.c
--rw-r--r--   0 runner    (1001) docker     (127)    15050 2024-04-20 04:38:20.000000 anycrc-0.3.3/src/anycrc/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:38:25.178666 anycrc-0.3.3/src/anycrc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-20 04:38:25.000000 anycrc-0.3.3/src/anycrc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-20 04:38:25.000000 anycrc-0.3.3/src/anycrc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 04:38:25.000000 anycrc-0.3.3/src/anycrc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-20 04:38:25.000000 anycrc-0.3.3/src/anycrc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:27:28.943459 anycrc-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-23 19:27:22.000000 anycrc-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-23 19:27:28.943459 anycrc-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-23 19:27:22.000000 anycrc-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:27:28.943459 anycrc-0.4.0/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:27:28.943459 anycrc-0.4.0/lib/crcany/
+-rw-r--r--   0 runner    (1001) docker     (127)    23924 2024-04-23 19:27:22.000000 anycrc-0.4.0/lib/crcany/crc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18683 2024-04-23 19:27:22.000000 anycrc-0.4.0/lib/crcany/model.c
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-23 19:27:22.000000 anycrc-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:27:28.943459 anycrc-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-23 19:27:22.000000 anycrc-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:27:28.943459 anycrc-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:27:28.943459 anycrc-0.4.0/src/anycrc/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 19:27:22.000000 anycrc-0.4.0/src/anycrc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-23 19:27:22.000000 anycrc-0.4.0/src/anycrc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-23 19:27:22.000000 anycrc-0.4.0/src/anycrc/anycrc.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    17529 2024-04-23 19:27:22.000000 anycrc-0.4.0/src/anycrc/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:27:28.943459 anycrc-0.4.0/src/anycrc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-23 19:27:28.000000 anycrc-0.4.0/src/anycrc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-23 19:27:28.000000 anycrc-0.4.0/src/anycrc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:27:28.000000 anycrc-0.4.0/src/anycrc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 19:27:28.000000 anycrc-0.4.0/src/anycrc.egg-info/top_level.txt
```

### Comparing `anycrc-0.3.3/LICENSE` & `anycrc-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anycrc-0.3.3/README.md` & `anycrc-0.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-This is a Cython module with bindings to the [crcany](https://github.com/madler/crcany) library. It supports calculating CRC hashes of arbitary sizes as well as updating a crc hash over time.
+This is a Cython module with bindings to the [crcany](https://github.com/madler/crcany) library. It supports calculating CRC hashes of arbitary sizes as well as updating a crc hash over time. It takes advantage of crcany's ability to efficiently combine multiple CRCs to parallelize the CRC's calculation.
 
 ## Installation
 
 `pip install anycrc`
 
 ## Usage
 
@@ -38,32 +38,41 @@
 ```python
 >>> # width, poly, init, refin, refout, xorout
 >>> my_crc = anycrc.CRC(10, 0b0101010101, 0x3ff, True, False, 0)
 >>> my_crc.calc('Hello World!')
 35
 ```
 
+This module will sometimes compute the CRC in parallel using multiple processors. To disable parallelism write:
+
+`python
+anycrc.set_parallel(False)
+`
+
 The CRC's width cannot exceed your system's maximum integer width.
 
 For a list of pre-built models, check [models.py](https://github.com/marzooqy/anycrc/blob/main/src/anycrc/models.py). To get a list of the models at any time, use the following command:
 
 `python -m anycrc models`
 
 ## Benchmarks
 
 Calculating the CRC32 for lorem ipsum 10 million times:
 
 | Module | Time Elapsed (s) | Speed (MiB/s) | Relative |
 |---|:-:|:-:|:-:|
-| anycrc | 6.660 | 637.26 | 1.000 |
-| zlib | 7.567 | 560.86 | 1.136 |
-| fastcrc | 17.508 | 242.39 | 2.629 |
-| crcmod-plus | 19.619 | 216.32 | 2.946 |
+| anycrc | 2.397 | 1770.21 | 1.000 |
+| zlib | 2.791 | 1520.45 | 1.164 |
+| fastcrc | 7.782 | 545.37 | 3.246 |
+| crcmod-plus | 8.891 | 477.35 | 3.708 |
 
 Calculating the CRC32 for the text of lorem ipsum repeated 1 million times in a single pass:
 
 | Module | Time Elapsed (s) | Speed (MiB/s) | Relative |
 |---|:-:|:-:|:-:|
-| anycrc | 0.293 | 1447.36 | 1.000 |
-| zlib | 0.496 | 856.06 | 1.691 |
-| fastcrc | 1.310 | 323.88 | 4.469 |
-| crcmod-plus | 1.280 | 331.44 | 4.367 |
+| anycrc (parallel) | 0.018 | 24231.05 | 1.000 |
+| anycrc (serial) | 0.202 | 2100.68 | 11.535 |
+| zlib | 0.215 | 1977.93 | 12.251 |
+| fastcrc | 0.670 | 633.75 | 38.234 |
+| crcmod-plus | 0.668 | 635.19 | 38.148 |
+
+Tested on a 12th generation Intel i7 processor. Parallel performance will depend on your system. Note that parallelism is disabled when the length of the input data is under 20k, as the serial method is faster in that case.
```

### Comparing `anycrc-0.3.3/lib/crcany/crc.c` & `anycrc-0.4.0/lib/crcany/crc.c`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,22 @@
  */
 
 /*
 * Edited by Hussain Al Marzooq to add support for the slice-by-16 algorithm
 */
   
 #include <stddef.h>
+#include <stdio.h>
+#include <stdlib.h>
 #include <assert.h>
+
+#if defined(_OPENMP)
+#include "omp.h"
+#endif
+
 #include "crc.h"
 
 word_t crc_bitwise(model_t *model, word_t crc, void const *dat, size_t len) {
     unsigned char const *buf = dat;
     word_t poly = model->poly;
 
     // If requested, return the initial CRC.
@@ -372,95 +379,95 @@
     else
         while (len && ((ptrdiff_t)buf & (WORDCHARS - 1))) {
             crc = (crc << 8) ^
                   model->table_byte[((crc >> shift) ^ *buf++) & 0xff];
             len--;
         }
 
-    // Process as many 16 byte chunks as are available.
+    // Process as many 16 byte block as are available.
     if (len >= 16) {
         crc <<= top;
         if (little) {
             if (!model->ref)
                 crc = swap(crc);
             do {
-				uint32_t crc_hi = crc >> 32;
-				uint32_t crc_lo = crc & 0xffffffff;
-				uint32_t i1 = *(uint32_t const *)buf;
-				uint32_t i2 = *(uint32_t const *)(buf + 4);
-				uint32_t i3 = *(uint32_t const *)(buf + 8);
-				uint32_t i4 = *(uint32_t const *)(buf + 12);
-				
-				crc_hi ^= i2;
-				crc_lo ^= i1;
-				
+                uint32_t crc_hi = crc >> 32;
+                uint32_t crc_lo = crc & 0xffffffff;
+                uint32_t i1 = *(uint32_t const *)buf;
+                uint32_t i2 = *(uint32_t const *)(buf + 4);
+                uint32_t i3 = *(uint32_t const *)(buf + 8);
+                uint32_t i4 = *(uint32_t const *)(buf + 12);
+
+                crc_hi ^= i2;
+                crc_lo ^= i1;
+
                 crc = model->table_word[15][crc_lo & 0xff]
                     ^ model->table_word[14][(crc_lo >> 8) & 0xff]
                     ^ model->table_word[13][(crc_lo >> 16) & 0xff]
-                    ^ model->table_word[12][(crc_lo >> 24) & 0xff]
+                    ^ model->table_word[12][crc_lo >> 24]
                     ^ model->table_word[11][crc_hi & 0xff]
                     ^ model->table_word[10][(crc_hi >> 8) & 0xff]
                     ^ model->table_word[9][(crc_hi >> 16) & 0xff]
                     ^ model->table_word[8][crc_hi >> 24]
-					^ model->table_word[7][i3 & 0xff]
+                    ^ model->table_word[7][i3 & 0xff]
                     ^ model->table_word[6][(i3 >> 8) & 0xff]
                     ^ model->table_word[5][(i3 >> 16) & 0xff]
                     ^ model->table_word[4][i3 >> 24]
                     ^ model->table_word[3][i4 & 0xff]
                     ^ model->table_word[2][(i4 >> 8) & 0xff]
                     ^ model->table_word[1][(i4 >> 16) & 0xff]
                     ^ model->table_word[0][i4 >> 24];
-					
+                    
                 buf += 16;
                 len -= 16;
             } while (len >= 16);
             if (!model->ref)
                 crc = swap(crc);
         }
         else {
             if (model->ref)
                 crc = swap(crc);
             do {
-				uint32_t crc_hi = crc >> 32;
-				uint32_t crc_lo = crc & 0xffffffff;
-				uint32_t i1 = *(uint32_t const *)buf;
-				uint32_t i2 = *(uint32_t const *)(buf + 4);
-				uint32_t i3 = *(uint32_t const *)(buf + 8);
-				uint32_t i4 = *(uint32_t const *)(buf + 12);
-				
-				crc_hi ^= i1;
-				crc_lo ^= i2;
-				
+                uint32_t crc_hi = crc >> 32;
+                uint32_t crc_lo = crc & 0xffffffff;
+                uint32_t i1 = *(uint32_t const *)buf;
+                uint32_t i2 = *(uint32_t const *)(buf + 4);
+                uint32_t i3 = *(uint32_t const *)(buf + 8);
+                uint32_t i4 = *(uint32_t const *)(buf + 12);
+
+                crc_hi ^= i1;
+                crc_lo ^= i2;
+		
                 crc = model->table_word[0][i4 & 0xff]
                     ^ model->table_word[1][(i4 >> 8) & 0xff]
                     ^ model->table_word[2][(i4 >> 16) & 0xff]
-                    ^ model->table_word[3][(i4 >> 24) & 0xff]
+                    ^ model->table_word[3][i4 >> 24]
                     ^ model->table_word[4][i3 & 0xff]
                     ^ model->table_word[5][(i3 >> 8) & 0xff]
                     ^ model->table_word[6][(i3 >> 16) & 0xff]
                     ^ model->table_word[7][i3 >> 24]
                     ^ model->table_word[8][crc_lo & 0xff]
                     ^ model->table_word[9][(crc_lo >> 8) & 0xff]
                     ^ model->table_word[10][(crc_lo >> 16) & 0xff]
                     ^ model->table_word[11][crc_lo >> 24]
                     ^ model->table_word[12][crc_hi & 0xff]
                     ^ model->table_word[13][(crc_hi >> 8) & 0xff]
                     ^ model->table_word[14][(crc_hi >> 16) & 0xff]
-                    ^ model->table_word[15][(crc_hi >> 24) & 0xff];
-					
+                    ^ model->table_word[15][crc_hi >> 24];
+                    
                 buf += 16;
                 len -= 16;
             } while (len >= 16);
             if (model->ref)
                 crc = swap(crc);
         }
         crc >>= top;
     }
 
-    // Process any remaining bytes after the last 16 byte chunk.
+    // Process any remaining bytes after the last 16 byte block.
     if (model->ref)
         while (len--)
             crc = (crc >> 8) ^ model->table_byte[(crc ^ *buf++) & 0xff];
     else if (model->width <= 8) {
         while (len--)
             crc = model->table_byte[(crc ^ *buf++) & 0xff];
         crc >>= shift;
@@ -474,14 +481,52 @@
 
     // Post-process and return the CRC.
     if (model->rev)
         crc = reverse(crc, model->width);
     return crc;
 }
 
+word_t crc_parallel(model_t *model, word_t crc, void const *dat, size_t len) {
+    #if defined(_OPENMP)
+    char nthreads = omp_get_max_threads();
+    #else
+    char nthreads = 1;
+    #endif
+    
+	word_t* crc_p = (word_t*)malloc(nthreads * sizeof(word_t));
+	size_t block_len = len / nthreads;
+    
+    // This way all of the later blocks will have the same size
+    size_t first_block_len = block_len + (len - nthreads * block_len);
+    void const *offset = (unsigned char*)dat + first_block_len;
+    
+    char i;
+    
+    // Split the data into a number of blocks equal to the system's number of threads and compute the CRC for each in parallel
+	#pragma omp parallel for
+	for(i = 0; i < nthreads; i++) {
+        // First block goes directly into the initial CRC
+        if(i == 0) {
+            crc = crc_slice16(model, crc, (unsigned char*)dat, first_block_len);
+        } else {
+            crc_p[(unsigned char)i] = crc_slice16(model, model->init, (unsigned char*)offset + ((i - 1) * block_len), block_len);
+        }
+	}
+	
+    // Combine the CRCs
+    // Not much could be done to parallelize this, so just do it serially
+    for(unsigned char i = 1; i < nthreads; i++) {
+        crc = crc_combine(model, crc, crc_p[i], block_len);
+    }
+    
+    free(crc_p);
+    
+	return crc;
+}
+
 // Return a(x) multiplied by b(x) modulo p(x), where p(x) is the CRC
 // polynomial. For speed, this requires that a not be zero.
 static word_t multmodp(model_t *model, word_t a, word_t b) {
     word_t top = (word_t)1 << (model->width - 1);
     word_t prod = 0;
     if (model->ref) {
         // Reflected polynomial.
```

### Comparing `anycrc-0.3.3/lib/crcany/model.c` & `anycrc-0.4.0/lib/crcany/model.c`

 * *Files identical despite different names*

### Comparing `anycrc-0.3.3/src/anycrc/models.py` & `anycrc-0.4.0/src/anycrc/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -107,8 +107,83 @@
     'CRC32-XFER': model(width=32, poly=0x000000af, init=0x00000000, refin=False, refout=False, xorout=0x00000000, check=0xbd0be338, residue=0x00000000),
     'CRC40-GSM': model(width=40, poly=0x0004820009, init=0x0000000000, refin=False, refout=False, xorout=0xffffffffff, check=0xd4164fc646, residue=0xc4ff8071ff),
     'CRC64-ECMA-182': model(width=64, poly=0x42f0e1eba9ea3693, init=0x0000000000000000, refin=False, refout=False, xorout=0x0000000000000000, check=0x6c40df5f0b497347, residue=0x0000000000000000),
     'CRC64-GO-ISO': model(width=64, poly=0x000000000000001b, init=0xffffffffffffffff, refin=True, refout=True, xorout=0xffffffffffffffff, check=0xb90956c775a41001, residue=0x5300000000000000),
     'CRC64-MS': model(width=64, poly=0x259c84cba6426349, init=0xffffffffffffffff, refin=True, refout=True, xorout=0x0000000000000000, check=0x75d4b74f024eceea, residue=0x0000000000000000),
     'CRC64-WE': model(width=64, poly=0x42f0e1eba9ea3693, init=0xffffffffffffffff, refin=False, refout=False, xorout=0xffffffffffffffff, check=0x62ec59e3f1a4f00a, residue=0xfcacbebd5931a992),
     'CRC64-XZ': model(width=64, poly=0x42f0e1eba9ea3693, init=0xffffffffffffffff, refin=True, refout=True, xorout=0xffffffffffffffff, check=0x995dc9bbdf1939fa, residue=0x49958c9abd7d353f)
+}
+
+aliases = {
+    'CRC4-ITU': 'CRC4-G-704',
+    'CRC5-EPC': 'CRC5-EPC-C1G2',
+    'CRC5-ITU': 'CRC5-G-704',
+    'CRC6-ITU': 'CRC6-G-704',
+    'CRC7': 'CRC7-MMC',
+    'CRC8-ITU': 'CRC8-I-432-1',
+    'CRC8-MAXIM': 'CRC8-MAXIM-DOW',
+    'DOW-CRC': 'CRC8-MAXIM-DOW',
+    'CRC8': 'CRC8-SMBUS',
+    'CRC8-AES': 'CRC8-TECH-3250',
+    'CRC8-EBU': 'CRC8-TECH-3250',
+    'CRC10': 'CRC10-ATM',
+    'CRC10-I-610': 'CRC10-ATM',
+    'CRC11': 'CRC11-FLEXRAY',
+    'X-CRC12': 'CRC12-DECT',
+    'CRC12': 'CRC12-UMTS',
+    '3GPP': 'CRC12-UMTS',
+    'CRC15': 'CRC15-CAN',
+    'ARC': 'CRC16-ARC',
+    'CRC16': 'CRC16-ARC',
+    'CRC16-LHA': 'CRC16-ARC',
+    'CRC-IBM': 'CRC16-ARC',
+    'R-CRC16': 'CRC16-DECT-R',
+    'X-CRC16': 'CRC16-DECT-X',
+    'CRC16-DARC': 'CRC16-GENIBUS',
+    'CRC16-EPC': 'CRC16-GENIBUS',
+    'CRC16-EPC-C1G2': 'CRC16-GENIBUS',
+    'CRC16-I-CODE': 'CRC16-GENIBUS',
+    'CRC16-AUTOSAR': 'CRC16-IBM-3740',
+    'CRC16-CCITT-FALSE': 'CRC16-IBM-3740',
+    'CRC16-ISO-HDLC': 'CRC16-IBM-SDLC',
+    'CRC16-ISO-IEC-14443-3-B': 'CRC16-IBM-SDLC',
+    'CRC16-X-25': 'CRC16-IBM-SDLC',
+    'CRC-A': 'CRC16-ISO-IEC-14443-3-A',
+    'CRC16-BLUETOOTH': 'CRC16-KERMIT',
+    'CRC16-CCITT': 'CRC16-KERMIT',
+    'CRC16-CCITT-TRUE': 'CRC16-KERMIT',
+    'CRC16-V-41-LSB': 'CRC16-KERMIT',
+    'CRC-CCITT': 'CRC16-KERMIT',
+    'KERMIT': 'CRC16-KERMIT',
+    'CRC16-MAXIM': 'CRC16-MAXIM-DOW',
+    'MODBUS': 'CRC16-MODBUS',
+    'CRC16-IEC-61158-2': 'CRC16-PROFIBUS',
+    'CRC16-AUG-CCITT': 'CRC16-SPI-FUJITSU',
+    'CRC16-BUYPASS': 'CRC16-UMTS',
+    'CRC16-VERIFONE': 'CRC16-UMTS',
+    'CRC15-ACORN': 'CRC16-XMODEM',
+    'CRC16-LTE': 'CRC16-XMODEM',
+    'CRC16-V-41-MSB': 'CRC16-XMODEM',
+    'XMODEM': 'CRC16-XMODEM',
+    'ZMODEM': 'CRC16-XMODEM',
+    'CRC24': 'CRC24-OPENPGP',
+    'CRC32Q': 'CRC32-AIXM',
+    'CRC32D': 'CRC32-BASE91-D',
+    'CRC32-AAL5': 'CRC32-BZIP2',
+    'CRC32-DECT-B': 'CRC32-BZIP2',
+    'B-CRC32': 'CRC32-BZIP2',
+    'CKSUM': 'CRC32-CKSUM',
+    'CRC32-POSIX': 'CRC32-CKSUM',
+    'CRC32-BASE91-C': 'CRC32-ISCSI',
+    'CRC32-CASTAGNOLI': 'CRC32-ISCSI',
+    'CRC32-INTERLAKEN': 'CRC32-ISCSI',
+    'CRC32C': 'CRC32-ISCSI',
+    'CRC32': 'CRC32-ISO-HDLC',
+    'CRC32-ADCCP': 'CRC32-ISO-HDLC',
+    'CRC32-V-42': 'CRC32-ISO-HDLC',
+    'CRC32-XZ': 'CRC32-ISO-HDLC',
+    'PKZIP': 'CRC32-ISO-HDLC',
+    'JAMCRC': 'CRC32-JAMCRC',
+    'XFER': 'CRC32-XFER',
+    'CRC64': 'CRC64-ECMA-182',
+    'CRC64-GO-ECMA': 'CRC64-XZ'
 }
```

