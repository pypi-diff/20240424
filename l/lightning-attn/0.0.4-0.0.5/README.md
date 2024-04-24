# Comparing `tmp/lightning_attn-0.0.4.tar.gz` & `tmp/lightning_attn-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning_attn-0.0.4.tar", last modified: Sun Mar 10 07:14:01 2024, max compression
+gzip compressed data, was "lightning_attn-0.0.5.tar", last modified: Wed Apr 24 07:43:19 2024, max compression
```

## Comparing `lightning_attn-0.0.4.tar` & `lightning_attn-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-10 07:14:01.503208 lightning_attn-0.0.4/
--rw-r--r--   0 root         (0) root         (0)     1068 2024-01-14 03:16:35.000000 lightning_attn-0.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      100 2024-03-10 07:14:01.500437 lightning_attn-0.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4832 2024-03-10 07:12:13.000000 lightning_attn-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-10 07:14:01.345283 lightning_attn-0.0.4/lightning_attn/
--rw-r--r--   0 root         (0) root         (0)       40 2024-01-15 08:41:10.000000 lightning_attn-0.0.4/lightning_attn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-10 07:14:01.406719 lightning_attn-0.0.4/lightning_attn/ops/
--rw-r--r--   0 root         (0) root         (0)       83 2024-01-15 13:41:41.000000 lightning_attn-0.0.4/lightning_attn/ops/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1337 2024-03-10 06:35:56.000000 lightning_attn-0.0.4/lightning_attn/ops/lightning_attn_interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-10 07:14:01.434505 lightning_attn-0.0.4/lightning_attn/ops/torch/
--rw-r--r--   0 root         (0) root         (0)       56 2024-01-15 08:26:56.000000 lightning_attn-0.0.4/lightning_attn/ops/torch/__init__.py
--rw-r--r--   0 root         (0) root         (0)      814 2024-03-10 06:38:10.000000 lightning_attn-0.0.4/lightning_attn/ops/torch/linear_attention.py
--rw-r--r--   0 root         (0) root         (0)      563 2024-01-14 05:21:48.000000 lightning_attn-0.0.4/lightning_attn/ops/torch/srmsnorm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-10 07:14:01.471657 lightning_attn-0.0.4/lightning_attn/ops/triton/
--rw-r--r--   0 root         (0) root         (0)      118 2024-03-10 06:30:03.000000 lightning_attn-0.0.4/lightning_attn/ops/triton/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14298 2024-03-10 06:05:11.000000 lightning_attn-0.0.4/lightning_attn/ops/triton/lightning_attn2.py
--rw-r--r--   0 root         (0) root         (0)    12754 2024-03-10 07:12:53.000000 lightning_attn-0.0.4/lightning_attn/ops/triton/lightning_attn2_no_decay.py
--rw-r--r--   0 root         (0) root         (0)     5126 2024-01-14 03:16:23.000000 lightning_attn-0.0.4/lightning_attn/ops/triton/srmsnorm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-10 07:14:01.489326 lightning_attn-0.0.4/lightning_attn/utils/
--rw-r--r--   0 root         (0) root         (0)       51 2024-01-15 09:09:20.000000 lightning_attn-0.0.4/lightning_attn/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1227 2024-01-15 09:20:33.000000 lightning_attn-0.0.4/lightning_attn/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-10 07:14:01.389147 lightning_attn-0.0.4/lightning_attn.egg-info/
--rw-r--r--   0 root         (0) root         (0)      100 2024-03-10 07:14:00.000000 lightning_attn-0.0.4/lightning_attn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      677 2024-03-10 07:14:01.000000 lightning_attn-0.0.4/lightning_attn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-10 07:14:00.000000 lightning_attn-0.0.4/lightning_attn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-03-10 07:14:00.000000 lightning_attn-0.0.4/lightning_attn.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-10 07:14:00.000000 lightning_attn-0.0.4/lightning_attn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-10 07:14:01.504823 lightning_attn-0.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      321 2024-03-10 07:13:41.000000 lightning_attn-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:43:19.159625 lightning_attn-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-01-14 03:16:35.000000 lightning_attn-0.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      100 2024-04-24 07:43:19.152460 lightning_attn-0.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4834 2024-04-24 07:33:40.000000 lightning_attn-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:43:18.763290 lightning_attn-0.0.5/lightning_attn/
+-rw-r--r--   0 root         (0) root         (0)       40 2024-01-15 08:41:10.000000 lightning_attn-0.0.5/lightning_attn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:43:18.909502 lightning_attn-0.0.5/lightning_attn/ops/
+-rw-r--r--   0 root         (0) root         (0)       83 2024-01-15 13:41:41.000000 lightning_attn-0.0.5/lightning_attn/ops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-04-24 07:37:19.000000 lightning_attn-0.0.5/lightning_attn/ops/lightning_attn_interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:43:18.988762 lightning_attn-0.0.5/lightning_attn/ops/torch/
+-rw-r--r--   0 root         (0) root         (0)       56 2024-01-15 08:26:56.000000 lightning_attn-0.0.5/lightning_attn/ops/torch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      814 2024-03-10 06:38:10.000000 lightning_attn-0.0.5/lightning_attn/ops/torch/linear_attention.py
+-rw-r--r--   0 root         (0) root         (0)      563 2024-01-14 05:21:48.000000 lightning_attn-0.0.5/lightning_attn/ops/torch/srmsnorm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:43:19.080083 lightning_attn-0.0.5/lightning_attn/ops/triton/
+-rw-r--r--   0 root         (0) root         (0)      118 2024-03-10 06:30:03.000000 lightning_attn-0.0.5/lightning_attn/ops/triton/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14298 2024-03-10 06:05:11.000000 lightning_attn-0.0.5/lightning_attn/ops/triton/lightning_attn2.py
+-rw-r--r--   0 root         (0) root         (0)    12754 2024-03-10 07:12:53.000000 lightning_attn-0.0.5/lightning_attn/ops/triton/lightning_attn2_no_decay.py
+-rw-r--r--   0 root         (0) root         (0)     5126 2024-01-14 03:16:23.000000 lightning_attn-0.0.5/lightning_attn/ops/triton/srmsnorm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:43:19.127330 lightning_attn-0.0.5/lightning_attn/utils/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-01-15 09:09:20.000000 lightning_attn-0.0.5/lightning_attn/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2024-01-15 09:20:33.000000 lightning_attn-0.0.5/lightning_attn/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:43:18.867561 lightning_attn-0.0.5/lightning_attn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      100 2024-04-24 07:43:18.000000 lightning_attn-0.0.5/lightning_attn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      677 2024-04-24 07:43:18.000000 lightning_attn-0.0.5/lightning_attn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 07:43:18.000000 lightning_attn-0.0.5/lightning_attn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-24 07:43:18.000000 lightning_attn-0.0.5/lightning_attn.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-24 07:43:18.000000 lightning_attn-0.0.5/lightning_attn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 07:43:19.163847 lightning_attn-0.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      321 2024-04-24 07:42:29.000000 lightning_attn-0.0.5/setup.py
```

### Comparing `lightning_attn-0.0.4/LICENSE` & `lightning_attn-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning_attn-0.0.4/README.md` & `lightning_attn-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -71,25 +71,25 @@
 1   1024.0    2.334296    0.957989     2.027344
 2   2048.0    4.657026    2.739919     5.976820
 3   4096.0    9.307817    8.891191    19.931032
 4   8192.0   18.617611   31.986572    72.536194
 5  16384.0   37.212578  121.685730   276.402618
 6  32768.0   74.594788  470.666473  1075.611450
 
-lightning2-speed_fwd-batch4-head32-qk_dim128-v_dim128-dtype_bf16:
+lightning2-memory_fwd-batch4-head32-qk_dim128-v_dim128-dtype_bf16:
          n   Lightning2       Flash2     Xformers
 0    512.0    64.000488    64.250977    64.250488
 1   1024.0   128.000488   128.500977   128.500488
 2   2048.0   256.000488   257.000977   257.000488
 3   4096.0   512.000488   514.000977   514.000488
 4   8192.0  1024.000488  1028.000977  1028.000488
 5  16384.0  2048.000488  2056.000977  2056.000488
 6  32768.0  4096.000488  4112.000977  4112.000488
 
-lightning2-speed_bwd-batch4-head32-qk_dim128-v_dim128-dtype_bf16:
+lightning2-memory_bwd-batch4-head32-qk_dim128-v_dim128-dtype_bf16:
          n    Lightning2        Flash2      Xformers
 0    512.0    173.600488    206.100977    270.100977
 1   1024.0    347.200488    412.200977    540.200977
 2   2048.0    694.400488    824.400977   1080.400977
 3   4096.0   1388.800488   1648.800977   2160.800977
 4   8192.0   2777.600488   3297.600977   4321.600977
 5  16384.0   5555.200488   6595.200977   8643.200977
```

#### html2text {}

```diff
@@ -22,20 +22,20 @@
 1.134238 0.754831 1.297325 3 4096.0 2.240815 2.740033 4.804503 4 8192.0
 4.414397 10.392551 18.329409 5 16384.0 8.832678 40.573997 71.699486 6 32768.0
 17.661427 162.895615 286.869446 lightning2-speed_bwd-batch4-head32-qk_dim128-
 v_dim128-dtype_bf16: n Lightning2 Flash2 Xformers 0 512.0 1.169621 0.397422
 0.797627 1 1024.0 2.334296 0.957989 2.027344 2 2048.0 4.657026 2.739919
 5.976820 3 4096.0 9.307817 8.891191 19.931032 4 8192.0 18.617611 31.986572
 72.536194 5 16384.0 37.212578 121.685730 276.402618 6 32768.0 74.594788
-470.666473 1075.611450 lightning2-speed_fwd-batch4-head32-qk_dim128-v_dim128-
+470.666473 1075.611450 lightning2-memory_fwd-batch4-head32-qk_dim128-v_dim128-
 dtype_bf16: n Lightning2 Flash2 Xformers 0 512.0 64.000488 64.250977 64.250488
 1 1024.0 128.000488 128.500977 128.500488 2 2048.0 256.000488 257.000977
 257.000488 3 4096.0 512.000488 514.000977 514.000488 4 8192.0 1024.000488
 1028.000977 1028.000488 5 16384.0 2048.000488 2056.000977 2056.000488 6 32768.0
-4096.000488 4112.000977 4112.000488 lightning2-speed_bwd-batch4-head32-
+4096.000488 4112.000977 4112.000488 lightning2-memory_bwd-batch4-head32-
 qk_dim128-v_dim128-dtype_bf16: n Lightning2 Flash2 Xformers 0 512.0 173.600488
 206.100977 270.100977 1 1024.0 347.200488 412.200977 540.200977 2 2048.0
 694.400488 824.400977 1080.400977 3 4096.0 1388.800488 1648.800977 2160.800977
 4 8192.0 2777.600488 3297.600977 4321.600977 5 16384.0 5555.200488 6595.200977
 8643.200977 6 32768.0 11110.400488 13190.400977 17286.400977 ``` ## Todo - [ ]
 Add support for lightning attention parallel version. - [x] Add support for
 linear attention with no decay. - [ ] Add support for linear attention with
```

### Comparing `lightning_attn-0.0.4/lightning_attn/ops/lightning_attn_interface.py` & `lightning_attn-0.0.5/lightning_attn/ops/lightning_attn_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 
 def next_power_of_2(n):
     return 2 ** (int(math.ceil(math.log(n, 2))))
 
 
 def lightning_attn_func(q, k, v, s=None):
-    assert s != None
     b, h, n, d = q.shape
     e = v.shape[-1]
     assert is_support(d) and is_support(e)
 
     # pad v's feature dim to power of 2
     e_pad = next_power_of_2(e)
     need_pad = e_pad != e
```

### Comparing `lightning_attn-0.0.4/lightning_attn/ops/torch/linear_attention.py` & `lightning_attn-0.0.5/lightning_attn/ops/torch/linear_attention.py`

 * *Files identical despite different names*

### Comparing `lightning_attn-0.0.4/lightning_attn/ops/torch/srmsnorm.py` & `lightning_attn-0.0.5/lightning_attn/ops/torch/srmsnorm.py`

 * *Files identical despite different names*

### Comparing `lightning_attn-0.0.4/lightning_attn/ops/triton/lightning_attn2.py` & `lightning_attn-0.0.5/lightning_attn/ops/triton/lightning_attn2.py`

 * *Files identical despite different names*

### Comparing `lightning_attn-0.0.4/lightning_attn/ops/triton/lightning_attn2_no_decay.py` & `lightning_attn-0.0.5/lightning_attn/ops/triton/lightning_attn2_no_decay.py`

 * *Files identical despite different names*

### Comparing `lightning_attn-0.0.4/lightning_attn/ops/triton/srmsnorm.py` & `lightning_attn-0.0.5/lightning_attn/ops/triton/srmsnorm.py`

 * *Files identical despite different names*

### Comparing `lightning_attn-0.0.4/lightning_attn/utils/utils.py` & `lightning_attn-0.0.5/lightning_attn/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lightning_attn-0.0.4/lightning_attn.egg-info/SOURCES.txt` & `lightning_attn-0.0.5/lightning_attn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

