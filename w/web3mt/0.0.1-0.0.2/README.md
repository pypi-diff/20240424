# Comparing `tmp/web3mt-0.0.1.tar.gz` & `tmp/web3mt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3mt-0.0.1.tar", max compression
+gzip compressed data, was "web3mt-0.0.2.tar", max compression
```

## Comparing `web3mt-0.0.1.tar` & `web3mt-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      791 2024-04-13 18:24:54.427221 web3mt-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 15:23:17.775417 web3mt-0.0.1/web3mt/__init__.py
--rw-r--r--   0        0        0        0 2023-12-30 07:13:43.356765 web3mt-0.0.1/web3mt/aptos/__init__.py
--rw-r--r--   0        0        0      163 2024-01-05 12:13:56.887788 web3mt-0.0.1/web3mt/aptos/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4979 2024-03-09 21:10:21.667601 web3mt-0.0.1/web3mt/aptos/__pycache__/bluemove.cpython-311.pyc
--rw-r--r--   0        0        0     5509 2024-04-13 03:49:25.200887 web3mt-0.0.1/web3mt/aptos/__pycache__/client.cpython-311.pyc
--rw-r--r--   0        0        0     2672 2024-04-13 15:33:14.006445 web3mt-0.0.1/web3mt/aptos/bluemove.py
--rw-r--r--   0        0        0     2921 2024-04-13 15:33:14.018449 web3mt-0.0.1/web3mt/aptos/client.py
--rw-r--r--   0        0        0      484 2024-02-10 14:59:01.635928 web3mt-0.0.1/web3mt/aptos/v1_token.graphql
--rw-r--r--   0        0        0      449 2024-02-10 17:46:28.592334 web3mt-0.0.1/web3mt/aptos/v2_token.graphql
--rw-r--r--   0        0        0       51 2024-04-08 22:32:58.137310 web3mt-0.0.1/web3mt/evm/__init__.py
--rw-r--r--   0        0        0      245 2024-04-09 12:28:53.444954 web3mt-0.0.1/web3mt/evm/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    23641 2024-04-13 17:56:27.760101 web3mt-0.0.1/web3mt/evm/__pycache__/client.cpython-311.pyc
--rw-r--r--   0        0        0     6545 2024-04-12 19:44:32.432969 web3mt-0.0.1/web3mt/evm/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0    16922 2024-04-13 17:56:26.460913 web3mt-0.0.1/web3mt/evm/client.py
--rw-r--r--   0        0        0     6819 2024-04-12 14:28:53.161153 web3mt-0.0.1/web3mt/evm/models.py
--rw-r--r--   0        0        0      227 2024-04-12 20:24:49.988168 web3mt-0.0.1/web3mt/utils/__init__.py
--rw-r--r--   0        0        0      548 2024-04-13 03:49:24.411725 web3mt-0.0.1/web3mt/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1303 2024-04-13 03:50:09.353860 web3mt-0.0.1/web3mt/utils/__pycache__/logger.cpython-311.pyc
--rw-r--r--   0        0        0     7095 2024-04-13 17:55:55.107540 web3mt-0.0.1/web3mt/utils/__pycache__/profile_session.cpython-311.pyc
--rw-r--r--   0        0        0     1732 2024-04-13 03:49:25.194882 web3mt-0.0.1/web3mt/utils/__pycache__/reader.cpython-311.pyc
--rw-r--r--   0        0        0      906 2024-02-28 19:02:21.549432 web3mt-0.0.1/web3mt/utils/__pycache__/sleeping.cpython-311.pyc
--rw-r--r--   0        0        0      777 2024-02-26 00:45:46.240188 web3mt-0.0.1/web3mt/utils/__pycache__/windows.cpython-311.pyc
--rw-r--r--   0        0        0      734 2024-04-13 03:50:07.580834 web3mt-0.0.1/web3mt/utils/logger.py
--rw-r--r--   0        0        0     4766 2024-04-13 16:52:07.492311 web3mt-0.0.1/web3mt/utils/profile_session.py
--rw-r--r--   0        0        0      498 2024-04-12 20:24:50.012177 web3mt-0.0.1/web3mt/utils/reader.py
--rw-r--r--   0        0        0      351 2024-02-27 15:07:31.632532 web3mt-0.0.1/web3mt/utils/sleeping.py
--rw-r--r--   0        0        0      230 2024-02-26 00:30:43.779500 web3mt-0.0.1/web3mt/utils/windows.py
--rw-r--r--   0        0        0      728 1970-01-01 00:00:00.000000 web3mt-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      791 2024-04-24 18:37:14.554891 web3mt-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 15:23:17.775417 web3mt-0.0.2/web3mt/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-30 07:13:43.356765 web3mt-0.0.2/web3mt/aptos/__init__.py
+-rw-r--r--   0        0        0      163 2024-01-05 12:13:56.887788 web3mt-0.0.2/web3mt/aptos/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4979 2024-03-09 21:10:21.667601 web3mt-0.0.2/web3mt/aptos/__pycache__/bluemove.cpython-311.pyc
+-rw-r--r--   0        0        0     5509 2024-04-13 03:49:25.200887 web3mt-0.0.2/web3mt/aptos/__pycache__/client.cpython-311.pyc
+-rw-r--r--   0        0        0     2672 2024-04-13 15:33:14.006445 web3mt-0.0.2/web3mt/aptos/bluemove.py
+-rw-r--r--   0        0        0     2921 2024-04-13 15:33:14.018449 web3mt-0.0.2/web3mt/aptos/client.py
+-rw-r--r--   0        0        0      484 2024-02-10 14:59:01.635928 web3mt-0.0.2/web3mt/aptos/v1_token.graphql
+-rw-r--r--   0        0        0      449 2024-02-10 17:46:28.592334 web3mt-0.0.2/web3mt/aptos/v2_token.graphql
+-rw-r--r--   0        0        0       51 2024-04-08 22:32:58.137310 web3mt-0.0.2/web3mt/evm/__init__.py
+-rw-r--r--   0        0        0      245 2024-04-09 12:28:53.444954 web3mt-0.0.2/web3mt/evm/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    23745 2024-04-23 10:36:18.380542 web3mt-0.0.2/web3mt/evm/__pycache__/client.cpython-311.pyc
+-rw-r--r--   0        0        0     6724 2024-04-24 15:24:47.574718 web3mt-0.0.2/web3mt/evm/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0    17041 2024-04-14 19:35:56.004135 web3mt-0.0.2/web3mt/evm/client.py
+-rw-r--r--   0        0        0     7041 2024-04-24 15:23:44.628653 web3mt-0.0.2/web3mt/evm/models.py
+-rw-r--r--   0        0        0      227 2024-04-12 20:24:49.988168 web3mt-0.0.2/web3mt/utils/__init__.py
+-rw-r--r--   0        0        0      548 2024-04-13 03:49:24.411725 web3mt-0.0.2/web3mt/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1303 2024-04-13 03:50:09.353860 web3mt-0.0.2/web3mt/utils/__pycache__/logger.cpython-311.pyc
+-rw-r--r--   0        0        0     7222 2024-04-24 15:24:47.106055 web3mt-0.0.2/web3mt/utils/__pycache__/profile_session.cpython-311.pyc
+-rw-r--r--   0        0        0     1732 2024-04-13 03:49:25.194882 web3mt-0.0.2/web3mt/utils/__pycache__/reader.cpython-311.pyc
+-rw-r--r--   0        0        0      906 2024-02-28 19:02:21.549432 web3mt-0.0.2/web3mt/utils/__pycache__/sleeping.cpython-311.pyc
+-rw-r--r--   0        0        0      777 2024-02-26 00:45:46.240188 web3mt-0.0.2/web3mt/utils/__pycache__/windows.cpython-311.pyc
+-rw-r--r--   0        0        0      734 2024-04-13 03:50:07.580834 web3mt-0.0.2/web3mt/utils/logger.py
+-rw-r--r--   0        0        0     4930 2024-04-24 15:29:03.699225 web3mt-0.0.2/web3mt/utils/profile_session.py
+-rw-r--r--   0        0        0      498 2024-04-12 20:24:50.012177 web3mt-0.0.2/web3mt/utils/reader.py
+-rw-r--r--   0        0        0      351 2024-02-27 15:07:31.632532 web3mt-0.0.2/web3mt/utils/sleeping.py
+-rw-r--r--   0        0        0      230 2024-02-26 00:30:43.779500 web3mt-0.0.2/web3mt/utils/windows.py
+-rw-r--r--   0        0        0      728 1970-01-01 00:00:00.000000 web3mt-0.0.2/PKG-INFO
```

### Comparing `web3mt-0.0.1/pyproject.toml` & `web3mt-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "web3mt"
-version = "0.0.1"
+version = "0.0.2"
 description = "Web3 multitool"
 authors = ["timertimertimer <timerkhan2002@gmail.com>"]
 repository = "https://github.com/timertimertimer/web3mt"
 packages = [{include = "web3mt"}]
 
 [tool.poetry.urls]
 Source = "https://github.com/timertimertimer/web3mt"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-web3 = "^6.17.0"
-web3db = "^1.0.0"
+web3 = "^6.17.2"
+web3db = "^1.0.2"
 python-okx = "^0.2.8"
 loguru = "^0.7.2"
 curl-cffi = "^0.6.2"
 better-proxy = "^1.1.5"
 aptos-sdk = "0.7.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `web3mt-0.0.1/web3mt/aptos/__pycache__/bluemove.cpython-311.pyc` & `web3mt-0.0.2/web3mt/aptos/__pycache__/bluemove.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `web3mt-0.0.1/web3mt/aptos/__pycache__/client.cpython-311.pyc` & `web3mt-0.0.2/web3mt/aptos/__pycache__/client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `web3mt-0.0.1/web3mt/aptos/bluemove.py` & `web3mt-0.0.2/web3mt/aptos/bluemove.py`

 * *Files identical despite different names*

### Comparing `web3mt-0.0.1/web3mt/aptos/client.py` & `web3mt-0.0.2/web3mt/aptos/client.py`

 * *Files identical despite different names*

### Comparing `web3mt-0.0.1/web3mt/evm/__pycache__/client.cpython-311.pyc` & `web3mt-0.0.2/web3mt/evm/__pycache__/client.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x4ac71a66 (Sat Apr 13 17:56:26 2024 UTC)
-files sz: 16922
+moddate:  0x1c301c66 (Sun Apr 14 19:35:56 2024 UTC)
+files sz: 17041
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
@@ -275,349 +275,349 @@
           38          88 LOAD_NAME               10 (str)
          
           26          90 BUILD_TUPLE             22
                       92 LOAD_CONST              17 (<code object __init__, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 26>)
                       94 MAKE_FUNCTION            5 (defaults, annotations)
                       96 STORE_NAME              13 (__init__)
          
-          62          98 LOAD_CONST              18 (<code object __aenter__, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 62>)
+          61          98 LOAD_CONST              18 (<code object __aenter__, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 61>)
                      100 MAKE_FUNCTION            0
                      102 STORE_NAME              14 (__aenter__)
          
-          65         104 LOAD_CONST              19 (<code object __aexit__, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 65>)
+          64         104 LOAD_CONST              19 (<code object __aexit__, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 64>)
                      106 MAKE_FUNCTION            0
                      108 STORE_NAME              15 (__aexit__)
          
-          68         110 LOAD_CONST              20 ('return')
+          67         110 LOAD_CONST              20 ('return')
                      112 LOAD_NAME               10 (str)
                      114 BUILD_TUPLE              2
-                     116 LOAD_CONST              21 (<code object sign, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 68>)
+                     116 LOAD_CONST              21 (<code object sign, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 67>)
                      118 MAKE_FUNCTION            4 (annotations)
                      120 STORE_NAME              16 (sign)
          
-          74         122 LOAD_CONST              20 ('return')
+          73         122 LOAD_CONST              20 ('return')
                      124 LOAD_NAME               11 (int)
                      126 BUILD_TUPLE              2
-                     128 LOAD_CONST              22 (<code object nonce, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 74>)
+                     128 LOAD_CONST              22 (<code object nonce, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 73>)
                      130 MAKE_FUNCTION            4 (annotations)
                      132 STORE_NAME              17 (nonce)
          
-          77         134 LOAD_CONST              56 ((None, None))
+          76         134 LOAD_CONST              56 ((None, None))
                      136 LOAD_CONST              23 ('contract')
                      138 LOAD_NAME               18 (AsyncContract)
                      140 LOAD_CONST              24 ('token_address')
                      142 LOAD_NAME               10 (str)
                      144 LOAD_CONST              20 ('return')
                      146 LOAD_NAME               11 (int)
                      148 BUILD_TUPLE              6
-                     150 LOAD_CONST              25 (<code object get_decimals, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 77>)
+                     150 LOAD_CONST              25 (<code object get_decimals, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 76>)
                      152 MAKE_FUNCTION            5 (defaults, annotations)
                      154 STORE_NAME              19 (get_decimals)
          
-          89         156 NOP
+          88         156 NOP
          
-          90         158 NOP
+          89         158 NOP
          
-          88         160 LOAD_CONST              57 ((None, None, None, False))
+          87         160 LOAD_CONST              57 ((None, None, None, False))
                      162 LOAD_CONST              23 ('contract')
          
-          89         164 LOAD_NAME               18 (AsyncContract)
+          88         164 LOAD_NAME               18 (AsyncContract)
          
-          88         166 LOAD_CONST              24 ('token_address')
+          87         166 LOAD_CONST              24 ('token_address')
          
-          89         168 LOAD_NAME               10 (str)
+          88         168 LOAD_NAME               10 (str)
          
-          88         170 LOAD_CONST              26 ('address')
+          87         170 LOAD_CONST              26 ('address')
          
-          90         172 LOAD_NAME               20 (Optional)
+          89         172 LOAD_NAME               20 (Optional)
                      174 LOAD_NAME               10 (str)
                      176 BINARY_SUBSCR
          
-          88         186 LOAD_CONST              27 ('echo')
+          87         186 LOAD_CONST              27 ('echo')
          
-          90         188 LOAD_NAME               12 (bool)
+          89         188 LOAD_NAME               12 (bool)
          
-          88         190 LOAD_CONST              20 ('return')
+          87         190 LOAD_CONST              20 ('return')
          
-          91         192 LOAD_NAME               21 (TokenAmount)
+          90         192 LOAD_NAME               21 (TokenAmount)
          
-          88         194 BUILD_TUPLE             10
-                     196 LOAD_CONST              28 (<code object balance_of, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 88>)
+          87         194 BUILD_TUPLE             10
+                     196 LOAD_CONST              28 (<code object balance_of, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 87>)
                      198 MAKE_FUNCTION            5 (defaults, annotations)
                      200 STORE_NAME              22 (balance_of)
          
-         110         202 NOP
+         109         202 NOP
          
-         111         204 NOP
+         110         204 NOP
          
-         109         206 LOAD_CONST              56 ((None, None))
+         108         206 LOAD_CONST              56 ((None, None))
                      208 LOAD_CONST              29 ('spender')
          
-         110         210 LOAD_NAME               10 (str)
+         109         210 LOAD_NAME               10 (str)
          
-         109         212 LOAD_CONST              23 ('contract')
+         108         212 LOAD_CONST              23 ('contract')
          
-         110         214 LOAD_NAME               18 (AsyncContract)
+         109         214 LOAD_NAME               18 (AsyncContract)
          
-         109         216 LOAD_CONST              24 ('token_address')
+         108         216 LOAD_CONST              24 ('token_address')
          
-         111         218 LOAD_NAME               10 (str)
+         110         218 LOAD_NAME               10 (str)
          
-         109         220 LOAD_CONST              20 ('return')
+         108         220 LOAD_CONST              20 ('return')
          
-         112         222 LOAD_NAME               21 (TokenAmount)
+         111         222 LOAD_NAME               21 (TokenAmount)
          
-         109         224 BUILD_TUPLE              8
-                     226 LOAD_CONST              30 (<code object get_allowance, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 109>)
+         108         224 BUILD_TUPLE              8
+                     226 LOAD_CONST              30 (<code object get_allowance, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 108>)
                      228 MAKE_FUNCTION            5 (defaults, annotations)
                      230 STORE_NAME              23 (get_allowance)
          
-         129         232 LOAD_NAME               24 (staticmethod)
+         128         232 LOAD_NAME               24 (staticmethod)
          
-         130         234 LOAD_CONST              31 ('w3')
+         129         234 LOAD_CONST              31 ('w3')
                      236 LOAD_NAME               25 (AsyncWeb3)
                      238 LOAD_CONST              32 ('block')
                      240 LOAD_NAME               26 (dict)
                      242 LOAD_CONST              20 ('return')
                      244 LOAD_NAME               11 (int)
                      246 BUILD_TUPLE              6
-                     248 LOAD_CONST              33 (<code object get_max_priority_fee_per_gas, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 129>)
+                     248 LOAD_CONST              33 (<code object get_max_priority_fee_per_gas, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 128>)
                      250 MAKE_FUNCTION            4 (annotations)
          
-         129         252 PRECALL                  0
+         128         252 PRECALL                  0
                      256 CALL                     0
          
-         130         266 STORE_NAME              27 (get_max_priority_fee_per_gas)
+         129         266 STORE_NAME              27 (get_max_priority_fee_per_gas)
          
-         152         268 NOP
+         151         268 NOP
          
-         153         270 NOP
+         152         270 NOP
          
-         154         272 NOP
+         153         272 NOP
          
-         155         274 NOP
+         154         274 NOP
          
-         156         276 NOP
+         155         276 NOP
          
-         157         278 NOP
+         156         278 NOP
          
-         149         280 LOAD_CONST              58 ((None, None, None, None, None, None))
+         148         280 LOAD_CONST              58 ((None, None, None, None, None, None))
                      282 LOAD_CONST              34 ('max_priority_fee_per_gas')
          
-         156         284 LOAD_NAME               20 (Optional)
+         155         284 LOAD_NAME               20 (Optional)
                      286 LOAD_NAME               11 (int)
                      288 BINARY_SUBSCR
          
-         149         298 LOAD_CONST              35 ('max_fee_per_gas')
+         148         298 LOAD_CONST              35 ('max_fee_per_gas')
          
-         157         300 LOAD_NAME               20 (Optional)
+         156         300 LOAD_NAME               20 (Optional)
                      302 LOAD_NAME               11 (int)
                      304 BINARY_SUBSCR
          
-         149         314 LOAD_CONST              20 ('return')
+         148         314 LOAD_CONST              20 ('return')
          
-         158         316 LOAD_NAME               28 (tuple)
+         157         316 LOAD_NAME               28 (tuple)
                      318 LOAD_NAME               12 (bool)
                      320 LOAD_NAME               29 (Exception)
                      322 LOAD_NAME               30 (HexBytes)
                      324 BINARY_OP                7 (|)
                      328 LOAD_NAME               10 (str)
                      330 BINARY_OP                7 (|)
                      334 BUILD_TUPLE              2
                      336 BINARY_SUBSCR
          
-         149         346 BUILD_TUPLE              6
-                     348 LOAD_CONST              36 (<code object send_transaction, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 149>)
+         148         346 BUILD_TUPLE              6
+                     348 LOAD_CONST              36 (<code object send_transaction, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 148>)
                      350 MAKE_FUNCTION            5 (defaults, annotations)
                      352 STORE_NAME              31 (send_transaction)
          
-         242         354 LOAD_CONST              37 ('tx_hash')
+         241         354 LOAD_CONST              37 ('tx_hash')
                      356 LOAD_NAME               10 (str)
                      358 LOAD_CONST              38 ('tx_name')
                      360 LOAD_NAME               10 (str)
                      362 LOAD_CONST              20 ('return')
                      364 LOAD_NAME               12 (bool)
                      366 BUILD_TUPLE              6
-                     368 LOAD_CONST              39 (<code object verify_transaction, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 242>)
+                     368 LOAD_CONST              39 (<code object verify_transaction, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 241>)
                      370 MAKE_FUNCTION            4 (annotations)
                      372 STORE_NAME              32 (verify_transaction)
          
-         266         374 LOAD_CONST              40 ('0x1249c58b')
+         265         374 LOAD_CONST              40 ('0x1249c58b')
          
-         267         376 PUSH_NULL
+         266         376 PUSH_NULL
                      378 LOAD_NAME               21 (TokenAmount)
                      380 LOAD_CONST               4 (0)
                      382 PRECALL                  1
                      386 CALL                     1
          
-         268         396 LOAD_CONST               1 (None)
+         267         396 LOAD_CONST               1 (None)
          
-         269         398 LOAD_CONST               1 (None)
+         268         398 LOAD_CONST               1 (None)
          
-         270         400 LOAD_CONST               1 (None)
+         269         400 LOAD_CONST               1 (None)
          
-         271         402 LOAD_CONST               5 (False)
+         270         402 LOAD_CONST               5 (False)
          
-         262         404 BUILD_TUPLE              6
+         261         404 BUILD_TUPLE              6
                      406 LOAD_CONST              41 ('to')
          
-         264         408 LOAD_NAME               10 (str)
+         263         408 LOAD_NAME               10 (str)
          
-         262         410 LOAD_CONST              42 ('name')
+         261         410 LOAD_CONST              42 ('name')
          
-         265         412 LOAD_NAME               10 (str)
+         264         412 LOAD_NAME               10 (str)
          
-         262         414 LOAD_CONST              43 ('data')
+         261         414 LOAD_CONST              43 ('data')
          
-         266         416 LOAD_NAME               10 (str)
+         265         416 LOAD_NAME               10 (str)
          
-         262         418 LOAD_CONST              44 ('value')
+         261         418 LOAD_CONST              44 ('value')
          
-         267         420 LOAD_NAME               21 (TokenAmount)
+         266         420 LOAD_NAME               21 (TokenAmount)
                      422 LOAD_NAME               11 (int)
                      424 BINARY_OP                7 (|)
          
-         262         428 LOAD_CONST              34 ('max_priority_fee_per_gas')
+         261         428 LOAD_CONST              34 ('max_priority_fee_per_gas')
          
-         268         430 LOAD_NAME               20 (Optional)
+         267         430 LOAD_NAME               20 (Optional)
                      432 LOAD_NAME               11 (int)
                      434 BINARY_SUBSCR
          
-         262         444 LOAD_CONST              35 ('max_fee_per_gas')
+         261         444 LOAD_CONST              35 ('max_fee_per_gas')
          
-         269         446 LOAD_NAME               20 (Optional)
+         268         446 LOAD_NAME               20 (Optional)
                      448 LOAD_NAME               11 (int)
                      450 BINARY_SUBSCR
          
-         262         460 LOAD_CONST              45 ('increase_gas_limit')
+         261         460 LOAD_CONST              45 ('increase_gas_limit')
          
-         270         462 LOAD_NAME               20 (Optional)
+         269         462 LOAD_NAME               20 (Optional)
                      464 LOAD_NAME               11 (int)
                      466 BINARY_SUBSCR
          
-         262         476 LOAD_CONST              46 ('check_existing')
+         261         476 LOAD_CONST              46 ('check_existing')
          
-         271         478 LOAD_NAME               12 (bool)
+         270         478 LOAD_NAME               12 (bool)
          
-         262         480 LOAD_CONST              20 ('return')
+         261         480 LOAD_CONST              20 ('return')
          
-         272         482 LOAD_NAME               12 (bool)
+         271         482 LOAD_NAME               12 (bool)
          
-         262         484 BUILD_TUPLE             18
-                     486 LOAD_CONST              47 (<code object tx, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 262>)
+         261         484 BUILD_TUPLE             18
+                     486 LOAD_CONST              47 (<code object tx, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 261>)
                      488 MAKE_FUNCTION            5 (defaults, annotations)
                      490 STORE_NAME              33 (tx)
          
-         302         492 NOP
+         301         492 NOP
          
-         303         494 NOP
+         302         494 NOP
          
-         301         496 LOAD_CONST              59 ((None, None, None, None))
+         300         496 LOAD_CONST              59 ((None, None, None, None))
                      498 LOAD_CONST              29 ('spender')
          
-         302         500 LOAD_NAME               10 (str)
+         301         500 LOAD_NAME               10 (str)
          
-         301         502 LOAD_CONST              23 ('contract')
+         300         502 LOAD_CONST              23 ('contract')
          
-         302         504 LOAD_NAME               18 (AsyncContract)
+         301         504 LOAD_NAME               18 (AsyncContract)
          
-         301         506 LOAD_CONST              24 ('token_address')
+         300         506 LOAD_CONST              24 ('token_address')
          
-         302         508 LOAD_NAME               10 (str)
+         301         508 LOAD_NAME               10 (str)
          
-         301         510 LOAD_CONST              48 ('amount')
+         300         510 LOAD_CONST              48 ('amount')
          
-         303         512 LOAD_NAME               21 (TokenAmount)
+         302         512 LOAD_NAME               21 (TokenAmount)
                      514 LOAD_NAME               11 (int)
                      516 BINARY_OP                7 (|)
          
-         301         520 LOAD_CONST              49 ('abi')
+         300         520 LOAD_CONST              49 ('abi')
          
-         303         522 LOAD_NAME               26 (dict)
+         302         522 LOAD_NAME               26 (dict)
          
-         301         524 LOAD_CONST              20 ('return')
+         300         524 LOAD_CONST              20 ('return')
          
-         304         526 LOAD_NAME               12 (bool)
+         303         526 LOAD_NAME               12 (bool)
          
-         301         528 BUILD_TUPLE             12
-                     530 LOAD_CONST              50 (<code object approve, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 301>)
+         300         528 BUILD_TUPLE             12
+                     530 LOAD_CONST              50 (<code object approve, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 300>)
                      532 MAKE_FUNCTION            5 (defaults, annotations)
                      534 STORE_NAME              34 (approve)
          
-         362         536 NOP
+         361         536 NOP
          
-         363         538 NOP
+         362         538 NOP
          
-         358         540 LOAD_CONST              56 ((None, None))
+         357         540 LOAD_CONST              56 ((None, None))
                      542 LOAD_CONST              41 ('to')
          
-         360         544 LOAD_NAME               10 (str)
+         359         544 LOAD_NAME               10 (str)
          
-         358         546 LOAD_CONST              48 ('amount')
+         357         546 LOAD_CONST              48 ('amount')
          
-         361         548 LOAD_NAME               21 (TokenAmount)
+         360         548 LOAD_NAME               21 (TokenAmount)
          
-         358         550 LOAD_CONST              23 ('contract')
+         357         550 LOAD_CONST              23 ('contract')
          
-         362         552 LOAD_NAME               18 (AsyncContract)
+         361         552 LOAD_NAME               18 (AsyncContract)
          
-         358         554 LOAD_CONST              24 ('token_address')
+         357         554 LOAD_CONST              24 ('token_address')
          
-         363         556 LOAD_NAME               10 (str)
+         362         556 LOAD_NAME               10 (str)
          
-         358         558 LOAD_CONST              20 ('return')
+         357         558 LOAD_CONST              20 ('return')
          
-         364         560 LOAD_NAME               28 (tuple)
+         363         560 LOAD_NAME               28 (tuple)
                      562 LOAD_NAME               12 (bool)
                      564 LOAD_NAME               29 (Exception)
                      566 LOAD_NAME               30 (HexBytes)
                      568 BINARY_OP                7 (|)
                      572 LOAD_NAME               10 (str)
                      574 BINARY_OP                7 (|)
                      578 BUILD_TUPLE              2
                      580 BINARY_SUBSCR
          
-         358         590 BUILD_TUPLE             10
-                     592 LOAD_CONST              51 (<code object transfer_token, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 358>)
+         357         590 BUILD_TUPLE             10
+                     592 LOAD_CONST              51 (<code object transfer_token, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 357>)
                      594 MAKE_FUNCTION            5 (defaults, annotations)
                      596 STORE_NAME              35 (transfer_token)
          
-         379         598 LOAD_CONST              60 (('ETH',))
+         378         598 LOAD_CONST              60 (('ETH',))
                      600 LOAD_CONST              20 ('return')
                      602 LOAD_NAME               36 (float)
                      604 BUILD_TUPLE              2
-                     606 LOAD_CONST              53 (<code object get_token_price, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 379>)
+                     606 LOAD_CONST              53 (<code object get_token_price, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 378>)
                      608 MAKE_FUNCTION            5 (defaults, annotations)
                      610 STORE_NAME              37 (get_token_price)
          
-         393         612 NOP
+         392         612 NOP
          
-         394         614 NOP
+         393         614 NOP
          
-         395         616 NOP
+         394         616 NOP
          
-         391         618 LOAD_CONST              61 ((None, False, False))
+         390         618 LOAD_CONST              61 ((None, False, False))
                      620 LOAD_CONST              26 ('address')
          
-         393         622 LOAD_NAME               10 (str)
+         392         622 LOAD_NAME               10 (str)
          
-         391         624 LOAD_CONST              27 ('echo')
+         390         624 LOAD_CONST              27 ('echo')
          
-         394         626 LOAD_NAME               12 (bool)
+         393         626 LOAD_NAME               12 (bool)
          
-         391         628 LOAD_CONST              54 ('get_usd_price')
+         390         628 LOAD_CONST              54 ('get_usd_price')
          
-         395         630 LOAD_NAME               12 (bool)
+         394         630 LOAD_NAME               12 (bool)
          
-         391         632 LOAD_CONST              20 ('return')
+         390         632 LOAD_CONST              20 ('return')
          
-         396         634 LOAD_NAME               21 (TokenAmount)
+         395         634 LOAD_NAME               21 (TokenAmount)
          
-         391         636 BUILD_TUPLE              8
-                     638 LOAD_CONST              55 (<code object get_native_balance, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 391>)
+         390         636 BUILD_TUPLE              8
+                     638 LOAD_CONST              55 (<code object get_native_balance, file "C:\Users\timer\Code\web3mt\web3mt\evm\client.py", line 390>)
                      640 MAKE_FUNCTION            5 (defaults, annotations)
                      642 STORE_NAME              38 (get_native_balance)
                      644 LOAD_CONST               1 (None)
                      646 RETURN_VALUE
          consts
             'Client'
             None
@@ -650,22 +650,22 @@
                   006a0800000000000000007c006a0600000000000000006a090000000000
                   00000064017c006a00000000000000000072117c006a0000000000000000
                   006a0a00000000000000006a0b00000000000000006e017c056901ac02a6
                   020000ab0200000000000000007418000000000000000000006601741a00
                   000000000000000000660164039c02741c000000000000000000006701ac
                   04a6030000ab0300000000000000007c005f0f00000000000000007c067c
                   005f1000000000000000007c077c005f1100000000000000007c087c005f
-                  12000000000000000064057c005f1300000000000000007c006a00000000
-                  0000000000721b7c0078016a1300000000000000007c006a000000000000
-                  0000006a1400000000000000009b007a0d000063025f1300000000000000
-                  007c006a050000000000000000722b7c0078016a13000000000000000064
-                  067c006a0500000000000000006a1500000000000000009b0064077c006a
-                  0600000000000000006a1600000000000000009b0064089d057a0d000063
-                  025f1300000000000000007c097c005f1700000000000000007c0a7c005f
-                  1800000000000000007c0b7c005f19000000000000000064005300
+                  12000000000000000064057c005f1300000000000000007c006a05000000
+                  0000000000722a7c0078016a1300000000000000007c006a050000000000
+                  0000006a1400000000000000009b0064067c006a0600000000000000006a
+                  1500000000000000009b0064079d047a0d000063025f1300000000000000
+                  007c006a000000000000000000721b7c006a0000000000000000006a1600
+                  000000000000009b0064087c006a1300000000000000009b009d037c005f
+                  1300000000000000007c097c005f1700000000000000007c0a7c005f1800
+                  000000000000007c0b7c005f19000000000000000064005300
                 26           0 RESUME                   0
                
                 40           2 LOAD_FAST                2 (profile)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (profile)
                
                 41          16 LOAD_FAST                2 (profile)
@@ -742,122 +742,122 @@
                            358 STORE_ATTR              18 (do_no_matter_what)
                
                 52         368 LOAD_CONST               5 ('')
                            370 LOAD_FAST                0 (self)
                            372 STORE_ATTR              19 (log_info)
                
                 53         382 LOAD_FAST                0 (self)
-                           384 LOAD_ATTR                0 (profile)
-                           394 POP_JUMP_FORWARD_IF_FALSE    27 (to 450)
+                           384 LOAD_ATTR                5 (account)
+                           394 POP_JUMP_FORWARD_IF_FALSE    42 (to 480)
                
                 54         396 LOAD_FAST                0 (self)
                            398 COPY                     1
                            400 LOAD_ATTR               19 (log_info)
                            410 LOAD_FAST                0 (self)
-                           412 LOAD_ATTR                0 (profile)
-                           422 LOAD_ATTR               20 (id)
+                           412 LOAD_ATTR                5 (account)
+                           422 LOAD_ATTR               20 (address)
                            432 FORMAT_VALUE             0
-                           434 BINARY_OP               13 (+=)
-                           438 SWAP                     2
-                           440 STORE_ATTR              19 (log_info)
-               
-                55     >>  450 LOAD_FAST                0 (self)
-                           452 LOAD_ATTR                5 (account)
-                           462 POP_JUMP_FORWARD_IF_FALSE    43 (to 550)
-               
-                56         464 LOAD_FAST                0 (self)
-                           466 COPY                     1
-                           468 LOAD_ATTR               19 (log_info)
-                           478 LOAD_CONST               6 (' | ')
-                           480 LOAD_FAST                0 (self)
-                           482 LOAD_ATTR                5 (account)
-                           492 LOAD_ATTR               21 (address)
-                           502 FORMAT_VALUE             0
-                           504 LOAD_CONST               7 (' (')
-                           506 LOAD_FAST                0 (self)
-                           508 LOAD_ATTR                6 (network)
-                           518 LOAD_ATTR               22 (name)
-                           528 FORMAT_VALUE             0
-                           530 LOAD_CONST               8 (')')
-                           532 BUILD_STRING             5
-                           534 BINARY_OP               13 (+=)
-                           538 SWAP                     2
-                           540 STORE_ATTR              19 (log_info)
-               
-                58     >>  550 LOAD_FAST                9 (okx_api_key)
-                           552 LOAD_FAST                0 (self)
-                           554 STORE_ATTR              23 (okx_api_key)
-               
-                59         564 LOAD_FAST               10 (okx_api_secret)
-                           566 LOAD_FAST                0 (self)
-                           568 STORE_ATTR              24 (okx_api_secret)
-               
-                60         578 LOAD_FAST               11 (okx_passphrase)
-                           580 LOAD_FAST                0 (self)
-                           582 STORE_ATTR              25 (okx_passphrase)
-                           592 LOAD_CONST               0 (None)
-                           594 RETURN_VALUE
+                           434 LOAD_CONST               6 (' (')
+                           436 LOAD_FAST                0 (self)
+                           438 LOAD_ATTR                6 (network)
+                           448 LOAD_ATTR               21 (name)
+                           458 FORMAT_VALUE             0
+                           460 LOAD_CONST               7 (')')
+                           462 BUILD_STRING             4
+                           464 BINARY_OP               13 (+=)
+                           468 SWAP                     2
+                           470 STORE_ATTR              19 (log_info)
+               
+                55     >>  480 LOAD_FAST                0 (self)
+                           482 LOAD_ATTR                0 (profile)
+                           492 POP_JUMP_FORWARD_IF_FALSE    27 (to 548)
+               
+                56         494 LOAD_FAST                0 (self)
+                           496 LOAD_ATTR                0 (profile)
+                           506 LOAD_ATTR               22 (id)
+                           516 FORMAT_VALUE             0
+                           518 LOAD_CONST               8 (' | ')
+                           520 LOAD_FAST                0 (self)
+                           522 LOAD_ATTR               19 (log_info)
+                           532 FORMAT_VALUE             0
+                           534 BUILD_STRING             3
+                           536 LOAD_FAST                0 (self)
+                           538 STORE_ATTR              19 (log_info)
+               
+                57     >>  548 LOAD_FAST                9 (okx_api_key)
+                           550 LOAD_FAST                0 (self)
+                           552 STORE_ATTR              23 (okx_api_key)
+               
+                58         562 LOAD_FAST               10 (okx_api_secret)
+                           564 LOAD_FAST                0 (self)
+                           566 STORE_ATTR              24 (okx_api_secret)
+               
+                59         576 LOAD_FAST               11 (okx_passphrase)
+                           578 LOAD_FAST                0 (self)
+                           580 STORE_ATTR              25 (okx_passphrase)
+                           590 LOAD_CONST               0 (None)
+                           592 RETURN_VALUE
                consts
                   None
                   'proxy'
                   ('request_kwargs',)
                   ('eth', 'net')
                   ('modules', 'middlewares')
                   ''
-                  ' | '
                   ' ('
                   ')'
-               names      ('profile', 'Account', 'from_key', 'decrypt', 'evm_private', 'account', 'network', 'Web3', 'AsyncHTTPProvider', 'rpc', 'proxy', 'proxy_string', 'AsyncEth', 'AsyncNet', 'async_geth_poa_middleware', 'w3', 'delay_between_requests', 'sleep_echo', 'do_no_matter_what', 'log_info', 'id', 'address', 'name', 'okx_api_key', 'okx_api_secret', 'okx_passphrase')
+                  ' | '
+               names      ('profile', 'Account', 'from_key', 'decrypt', 'evm_private', 'account', 'network', 'Web3', 'AsyncHTTPProvider', 'rpc', 'proxy', 'proxy_string', 'AsyncEth', 'AsyncNet', 'async_geth_poa_middleware', 'w3', 'delay_between_requests', 'sleep_echo', 'do_no_matter_what', 'log_info', 'address', 'name', 'id', 'okx_api_key', 'okx_api_secret', 'okx_passphrase')
                varnames   ('self', 'network', 'profile', 'account', 'encryption_password', 'proxy', 'delay_between_requests', 'sleep_echo', 'do_no_matter_what', 'okx_api_key', 'okx_api_secret', 'okx_passphrase')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\client.py'
                name       '__init__'
                firstlineno 26
                lnotab
                   0x020e0e0160010e010c012c0134ff120220010efc1c060e010e010e010e
-                  010e0136010e0156020e010e01
+                  010e0154010e0136010e010e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 131
                code 0x4b00010097007c005300
-                62           0 RETURN_GENERATOR
+                61           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                63           6 LOAD_FAST                0 (self)
+                62           6 LOAD_FAST                0 (self)
                              8 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\client.py'
                name       '__aenter__'
-               firstlineno 62
+               firstlineno 61
                lnotab 0x0601
             code
                argcount  : 4
                nlocals   : 4
                stacksize : 5
                flags     : 131
                code
                   0x4b00010097007c0172207401000000000000000000006a010000000000
                   0000007c006a0200000000000000009b0064017c029b009d03a6010000ab
                   0100000000000000000100640053007401000000000000000000006a0300
                   000000000000007c006a0200000000000000009b0064029d02a6010000ab
                   010000000000000000010064005300
-                65           0 RETURN_GENERATOR
+                64           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                66           6 LOAD_FAST                1 (exc_type)
+                65           6 LOAD_FAST                1 (exc_type)
                              8 POP_JUMP_FORWARD_IF_FALSE    32 (to 74)
                             10 LOAD_GLOBAL              1 (NULL + logger)
                             22 LOAD_ATTR                1 (error)
                             32 LOAD_FAST                0 (self)
                             34 LOAD_ATTR                2 (log_info)
                             44 FORMAT_VALUE             0
                             46 LOAD_CONST               1 (' | ')
@@ -887,15 +887,15 @@
                   ' | Tasks done'
                names      ('logger', 'error', 'log_info', 'success')
                varnames   ('self', 'exc_type', 'exc_val', 'exc_tb')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\client.py'
                name       '__aexit__'
-               firstlineno 65
+               firstlineno 64
                lnotab 0x0601
             'return'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 5
                flags     : 3
@@ -903,72 +903,72 @@
                   0x97007c006a0000000000000000006a0100000000000000006a02000000
                   0000000000a0030000000000000000000000000000000000000000740900
                   0000000000000000007c01ac01a6010000ab0100000000000000007c006a
                   0200000000000000006a050000000000000000a006000000000000000000
                   0000000000000000000000a6000000ab000000000000000000ac02a60200
                   00ab0200000000000000006a070000000000000000a00600000000000000
                   00000000000000000000000000a6000000ab0000000000000000005300
-                68           0 RESUME                   0
+                67           0 RESUME                   0
                
-                69           2 LOAD_FAST                0 (self)
+                68           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (w3)
                             14 LOAD_ATTR                1 (eth)
                             24 LOAD_ATTR                2 (account)
                             34 LOAD_METHOD              3 (sign_message)
                
-                70          56 LOAD_GLOBAL              9 (NULL + encode_defunct)
+                69          56 LOAD_GLOBAL              9 (NULL + encode_defunct)
                             68 LOAD_FAST                1 (text)
                             70 KW_NAMES                 1
                             72 PRECALL                  1
                             76 CALL                     1
                
-                71          86 LOAD_FAST                0 (self)
+                70          86 LOAD_FAST                0 (self)
                             88 LOAD_ATTR                2 (account)
                             98 LOAD_ATTR                5 (key)
                            108 LOAD_METHOD              6 (hex)
                            130 PRECALL                  0
                            134 CALL                     0
                
-                69         144 KW_NAMES                 2
+                68         144 KW_NAMES                 2
                            146 PRECALL                  2
                            150 CALL                     2
                
-                72         160 LOAD_ATTR                7 (signature)
+                71         160 LOAD_ATTR                7 (signature)
                            170 LOAD_METHOD              6 (hex)
                            192 PRECALL                  0
                            196 CALL                     0
                
-                69         206 RETURN_VALUE
+                68         206 RETURN_VALUE
                consts
                   None
                   ('text',)
                   ('private_key',)
                names      ('w3', 'eth', 'account', 'sign_message', 'encode_defunct', 'key', 'hex', 'signature')
                varnames   ('self', 'text')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\client.py'
                name       'sign'
-               firstlineno 68
+               firstlineno 67
                lnotab 0x020136011e013afe10032efd
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 131
                code
                   0x4b00010097007c006a0000000000000000006a010000000000000000a0
                   0200000000000000000000000000000000000000007c006a030000000000
                   0000006a040000000000000000a6010000ab010000000000000000830064
                   007b035600970386045300
-                74           0 RETURN_GENERATOR
+                73           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                75           6 LOAD_FAST                0 (self)
+                74           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (w3)
                             18 LOAD_ATTR                1 (eth)
                             28 LOAD_METHOD              2 (get_transaction_count)
                             50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                3 (account)
                             62 LOAD_ATTR                4 (address)
                             72 PRECALL                  1
@@ -984,15 +984,15 @@
                   None
                names      ('w3', 'eth', 'get_transaction_count', 'account', 'address')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\client.py'
                name       'nonce'
-               firstlineno 74
+               firstlineno 73
                lnotab 0x0601
             'contract'
             'token_address'
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 5
@@ -1005,43 +1005,43 @@
                   00ab0200000000000000007d010900740f000000000000000000007c016a
                   080000000000000000a00900000000000000000000000000000000000000
                   00a6000000ab000000000000000000a00a00000000000000000000000000
                   00000000000000a6000000ab000000000000000000830064007b03560097
                   038604a6010000ab01000000000000000053002300741600000000000000
                   00000074180000000000000000000066022400720b7d03590064007d037e
                   036402530064007d037e0377017700780359007701
-                77           0 RETURN_GENERATOR
+                76           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                78           6 LOAD_FAST                1 (contract)
+                77           6 LOAD_FAST                1 (contract)
                              8 POP_JUMP_FORWARD_IF_TRUE    61 (to 132)
                
-                79          10 LOAD_FAST                0 (self)
+                78          10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (w3)
                             22 LOAD_ATTR                1 (eth)
                             32 LOAD_METHOD              2 (contract)
                
-                80          54 LOAD_GLOBAL              7 (NULL + AsyncWeb3)
+                79          54 LOAD_GLOBAL              7 (NULL + AsyncWeb3)
                             66 LOAD_ATTR                4 (to_checksum_address)
                             76 LOAD_FAST                2 (token_address)
                             78 PRECALL                  1
                             82 CALL                     1
                
-                81          92 LOAD_GLOBAL             10 (DefaultABIs)
+                80          92 LOAD_GLOBAL             10 (DefaultABIs)
                            104 LOAD_ATTR                6 (Token)
                
-                79         114 KW_NAMES                 1
+                78         114 KW_NAMES                 1
                            116 PRECALL                  2
                            120 CALL                     2
                            130 STORE_FAST               1 (contract)
                
-                83     >>  132 NOP
+                82     >>  132 NOP
                
-                84         134 LOAD_GLOBAL             15 (NULL + int)
+                83         134 LOAD_GLOBAL             15 (NULL + int)
                            146 LOAD_FAST                1 (contract)
                            148 LOAD_ATTR                8 (functions)
                            158 LOAD_METHOD              9 (decimals)
                            180 PRECALL                  0
                            184 CALL                     0
                            194 LOAD_METHOD             10 (call)
                            216 PRECALL                  0
@@ -1053,33 +1053,33 @@
                            238 RESUME                   3
                            240 JUMP_BACKWARD_NO_INTERRUPT     4 (to 234)
                        >>  242 PRECALL                  1
                            246 CALL                     1
                            256 RETURN_VALUE
                        >>  258 PUSH_EXC_INFO
                
-                85         260 LOAD_GLOBAL             22 (ABIFunctionNotFound)
+                84         260 LOAD_GLOBAL             22 (ABIFunctionNotFound)
                            272 LOAD_GLOBAL             24 (ContractLogicError)
                            284 BUILD_TUPLE              2
                            286 CHECK_EXC_MATCH
                            288 POP_JUMP_FORWARD_IF_FALSE    11 (to 312)
                            290 STORE_FAST               3 (e)
                
-                86         292 POP_EXCEPT
+                85         292 POP_EXCEPT
                            294 LOAD_CONST               0 (None)
                            296 STORE_FAST               3 (e)
                            298 DELETE_FAST              3 (e)
                            300 LOAD_CONST               2 (0)
                            302 RETURN_VALUE
                            304 LOAD_CONST               0 (None)
                            306 STORE_FAST               3 (e)
                            308 DELETE_FAST              3 (e)
                            310 RERAISE                  1
                
-                85     >>  312 RERAISE                  0
+                84     >>  312 RERAISE                  0
                        >>  314 COPY                     3
                            316 POP_EXCEPT
                            318 RERAISE                  1
                ExceptionTable:
                  134 to 254 -> 258 [0]
                  258 to 290 -> 314 [1] lasti
                  304 to 312 -> 314 [1] lasti
@@ -1089,15 +1089,15 @@
                   0
                names      ('w3', 'eth', 'contract', 'AsyncWeb3', 'to_checksum_address', 'DefaultABIs', 'Token', 'int', 'functions', 'decimals', 'call', 'ABIFunctionNotFound', 'ContractLogicError')
                varnames   ('self', 'contract', 'token_address', 'e')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\client.py'
                name       'get_decimals'
-               firstlineno 77
+               firstlineno 76
                lnotab 0x060104012c01260116fe120402017e01200114ff
             'address'
             'echo'
             code
                argcount  : 5
                nlocals   : 9
                stacksize : 7
@@ -1121,30 +1121,30 @@
                   000000000000007d077c016a090000000000000000a01300000000000000
                   00000000000000000000000000a6000000ab000000000000000000a00b00
                   00000000000000000000000000000000000000a6000000ab000000000000
                   000000830064007b035600970386047d087c047221742900000000000000
                   0000006a1500000000000000007c006a1600000000000000009b0064067c
                   079b0064077c089b009d05a6010000ab01000000000000000001007c0753
                   00
-                88           0 RETURN_GENERATOR
+                87           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                92           6 LOAD_FAST                3 (address)
+                91           6 LOAD_FAST                3 (address)
                              8 POP_JUMP_FORWARD_IF_TRUE    12 (to 34)
                
-                93          10 LOAD_FAST                0 (self)
+                92          10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (account)
                             22 LOAD_ATTR                1 (address)
                             32 STORE_FAST               3 (address)
                
-                94     >>   34 LOAD_FAST                1 (contract)
+                93     >>   34 LOAD_FAST                1 (contract)
                             36 POP_JUMP_FORWARD_IF_TRUE    61 (to 160)
                
-                95          38 LOAD_FAST                0 (self)
+                94          38 LOAD_FAST                0 (self)
                             40 LOAD_ATTR                2 (w3)
                             50 LOAD_ATTR                3 (eth)
                             60 LOAD_METHOD              4 (contract)
                             82 LOAD_GLOBAL             11 (NULL + AsyncWeb3)
                             94 LOAD_ATTR                6 (to_checksum_address)
                            104 LOAD_FAST                2 (token_address)
                            106 PRECALL                  1
@@ -1152,15 +1152,15 @@
                            120 LOAD_GLOBAL             14 (DefaultABIs)
                            132 LOAD_ATTR                8 (Token)
                            142 KW_NAMES                 1
                            144 PRECALL                  2
                            148 CALL                     2
                            158 STORE_FAST               1 (contract)
                
-                96     >>  160 LOAD_FAST                1 (contract)
+                95     >>  160 LOAD_FAST                1 (contract)
                            162 LOAD_ATTR                9 (functions)
                            172 LOAD_METHOD             10 (balanceOf)
                            194 LOAD_FAST                3 (address)
                            196 PRECALL                  1
                            200 CALL                     1
                            210 LOAD_METHOD             11 (call)
                            232 PRECALL                  0
@@ -1169,66 +1169,66 @@
                            248 LOAD_CONST               0 (None)
                        >>  250 SEND                     3 (to 258)
                            252 YIELD_VALUE
                            254 RESUME                   3
                            256 JUMP_BACKWARD_NO_INTERRUPT     4 (to 250)
                        >>  258 STORE_FAST               5 (amount)
                
-                97         260 LOAD_GLOBAL             25 (NULL + sleep)
+                96         260 LOAD_GLOBAL             25 (NULL + sleep)
                
-                98         272 LOAD_FAST                0 (self)
+                97         272 LOAD_FAST                0 (self)
                            274 LOAD_ATTR               13 (delay_between_requests)
                
-                99         284 LOAD_FAST                0 (self)
+                98         284 LOAD_FAST                0 (self)
                            286 LOAD_ATTR               14 (profile)
                            296 POP_JUMP_FORWARD_IF_FALSE    12 (to 322)
                            298 LOAD_FAST                0 (self)
                            300 LOAD_ATTR               14 (profile)
                            310 LOAD_ATTR               15 (id)
                            320 JUMP_FORWARD             1 (to 324)
                        >>  322 LOAD_CONST               0 (None)
                
-               100     >>  324 LOAD_FAST                0 (self)
+                99     >>  324 LOAD_FAST                0 (self)
                            326 LOAD_ATTR               16 (sleep_echo)
                
-                97         336 KW_NAMES                 2
+                96         336 KW_NAMES                 2
                            338 PRECALL                  3
                            342 CALL                     3
                            352 GET_AWAITABLE            0
                            354 LOAD_CONST               0 (None)
                        >>  356 SEND                     3 (to 364)
                            358 YIELD_VALUE
                            360 RESUME                   3
                            362 JUMP_BACKWARD_NO_INTERRUPT     4 (to 356)
                        >>  364 POP_TOP
                
-               102         366 LOAD_FAST                0 (self)
+               101         366 LOAD_FAST                0 (self)
                            368 LOAD_METHOD             17 (get_decimals)
                            390 LOAD_FAST                1 (contract)
                            392 KW_NAMES                 3
                            394 PRECALL                  1
                            398 CALL                     1
                            408 GET_AWAITABLE            0
                            410 LOAD_CONST               0 (None)
                        >>  412 SEND                     3 (to 420)
                            414 YIELD_VALUE
                            416 RESUME                   3
                            418 JUMP_BACKWARD_NO_INTERRUPT     4 (to 412)
                        >>  420 STORE_FAST               6 (decimals)
                
-               103         422 LOAD_GLOBAL             37 (NULL + TokenAmount)
+               102         422 LOAD_GLOBAL             37 (NULL + TokenAmount)
                            434 LOAD_FAST                5 (amount)
                            436 LOAD_FAST                6 (decimals)
                            438 LOAD_CONST               4 (True)
                            440 KW_NAMES                 5
                            442 PRECALL                  3
                            446 CALL                     3
                            456 STORE_FAST               7 (balance)
                
-               104         458 LOAD_FAST                1 (contract)
+               103         458 LOAD_FAST                1 (contract)
                            460 LOAD_ATTR                9 (functions)
                            470 LOAD_METHOD             19 (symbol)
                            492 PRECALL                  0
                            496 CALL                     0
                            506 LOAD_METHOD             11 (call)
                            528 PRECALL                  0
                            532 CALL                     0
@@ -1236,18 +1236,18 @@
                            544 LOAD_CONST               0 (None)
                        >>  546 SEND                     3 (to 554)
                            548 YIELD_VALUE
                            550 RESUME                   3
                            552 JUMP_BACKWARD_NO_INTERRUPT     4 (to 546)
                        >>  554 STORE_FAST               8 (token_name)
                
-               105         556 LOAD_FAST                4 (echo)
+               104         556 LOAD_FAST                4 (echo)
                            558 POP_JUMP_FORWARD_IF_FALSE    33 (to 626)
                
-               106         560 LOAD_GLOBAL             41 (NULL + logger)
+               105         560 LOAD_GLOBAL             41 (NULL + logger)
                            572 LOAD_ATTR               21 (info)
                            582 LOAD_FAST                0 (self)
                            584 LOAD_ATTR               22 (log_info)
                            594 FORMAT_VALUE             0
                            596 LOAD_CONST               6 (' | Balance - ')
                            598 LOAD_FAST                7 (balance)
                            600 FORMAT_VALUE             0
@@ -1255,15 +1255,15 @@
                            604 LOAD_FAST                8 (token_name)
                            606 FORMAT_VALUE             0
                            608 BUILD_STRING             5
                            610 PRECALL                  1
                            614 CALL                     1
                            624 POP_TOP
                
-               107     >>  626 LOAD_FAST                7 (balance)
+               106     >>  626 LOAD_FAST                7 (balance)
                            628 RETURN_VALUE
                consts
                   None
                   ('address', 'abi')
                   ('profile_id', 'echo')
                   ('contract',)
                   True
@@ -1272,15 +1272,15 @@
                   ' '
                names      ('account', 'address', 'w3', 'eth', 'contract', 'AsyncWeb3', 'to_checksum_address', 'DefaultABIs', 'Token', 'functions', 'balanceOf', 'call', 'sleep', 'delay_between_requests', 'profile', 'id', 'sleep_echo', 'get_decimals', 'TokenAmount', 'symbol', 'logger', 'info', 'log_info')
                varnames   ('self', 'contract', 'token_address', 'address', 'echo', 'amount', 'decimals', 'balance', 'token_name')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\client.py'
                name       'balance_of'
-               firstlineno 88
+               firstlineno 87
                lnotab
                   0x06040401180104017a0164010c010c0128010cfd1e0538012401620104
                   014201
             'spender'
             code
                argcount  : 4
                nlocals   : 6
@@ -1302,22 +1302,22 @@
                   007c00a01100000000000000000000000000000000000000007c02ac03a6
                   010000ab010000000000000000830064007b035600970386047d05741900
                   0000000000000000007c006a0d00000000000000007c006a0e0000000000
                   000000720c7c006a0e00000000000000006a0f00000000000000006e0164
                   007c006a100000000000000000ac02a6030000ab03000000000000000083
                   0064007b0356009703860401007425000000000000000000007c047c0564
                   04ac05a6030000ab0300000000000000005300
-               109           0 RETURN_GENERATOR
+               108           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               113           6 LOAD_FAST                2 (contract)
+               112           6 LOAD_FAST                2 (contract)
                              8 POP_JUMP_FORWARD_IF_TRUE    61 (to 132)
                
-               114          10 LOAD_FAST                0 (self)
+               113          10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (w3)
                             22 LOAD_ATTR                1 (eth)
                             32 LOAD_METHOD              2 (contract)
                             54 LOAD_GLOBAL              7 (NULL + AsyncWeb3)
                             66 LOAD_ATTR                4 (to_checksum_address)
                             76 LOAD_FAST                3 (token_address)
                             78 PRECALL                  1
@@ -1325,15 +1325,15 @@
                             92 LOAD_GLOBAL             10 (DefaultABIs)
                            104 LOAD_ATTR                6 (Token)
                            114 KW_NAMES                 1
                            116 PRECALL                  2
                            120 CALL                     2
                            130 STORE_FAST               2 (contract)
                
-               115     >>  132 LOAD_FAST                2 (contract)
+               114     >>  132 LOAD_FAST                2 (contract)
                            134 LOAD_ATTR                7 (functions)
                            144 LOAD_METHOD              8 (allowance)
                            166 LOAD_FAST                0 (self)
                            168 LOAD_ATTR                9 (account)
                            178 LOAD_ATTR               10 (address)
                            188 LOAD_FAST                1 (spender)
                            190 PRECALL                  2
@@ -1345,85 +1345,85 @@
                            242 LOAD_CONST               0 (None)
                        >>  244 SEND                     3 (to 252)
                            246 YIELD_VALUE
                            248 RESUME                   3
                            250 JUMP_BACKWARD_NO_INTERRUPT     4 (to 244)
                        >>  252 STORE_FAST               4 (amount)
                
-               116         254 LOAD_GLOBAL             25 (NULL + sleep)
+               115         254 LOAD_GLOBAL             25 (NULL + sleep)
                
-               117         266 LOAD_FAST                0 (self)
+               116         266 LOAD_FAST                0 (self)
                            268 LOAD_ATTR               13 (delay_between_requests)
                
-               118         278 LOAD_FAST                0 (self)
+               117         278 LOAD_FAST                0 (self)
                            280 LOAD_ATTR               14 (profile)
                            290 POP_JUMP_FORWARD_IF_FALSE    12 (to 316)
                            292 LOAD_FAST                0 (self)
                            294 LOAD_ATTR               14 (profile)
                            304 LOAD_ATTR               15 (id)
                            314 JUMP_FORWARD             1 (to 318)
                        >>  316 LOAD_CONST               0 (None)
                
-               119     >>  318 LOAD_FAST                0 (self)
+               118     >>  318 LOAD_FAST                0 (self)
                            320 LOAD_ATTR               16 (sleep_echo)
                
-               116         330 KW_NAMES                 2
+               115         330 KW_NAMES                 2
                            332 PRECALL                  3
                            336 CALL                     3
                            346 GET_AWAITABLE            0
                            348 LOAD_CONST               0 (None)
                        >>  350 SEND                     3 (to 358)
                            352 YIELD_VALUE
                            354 RESUME                   3
                            356 JUMP_BACKWARD_NO_INTERRUPT     4 (to 350)
                        >>  358 POP_TOP
                
-               121         360 LOAD_FAST                0 (self)
+               120         360 LOAD_FAST                0 (self)
                            362 LOAD_METHOD             17 (get_decimals)
                            384 LOAD_FAST                2 (contract)
                            386 KW_NAMES                 3
                            388 PRECALL                  1
                            392 CALL                     1
                            402 GET_AWAITABLE            0
                            404 LOAD_CONST               0 (None)
                        >>  406 SEND                     3 (to 414)
                            408 YIELD_VALUE
                            410 RESUME                   3
                            412 JUMP_BACKWARD_NO_INTERRUPT     4 (to 406)
                        >>  414 STORE_FAST               5 (decimals)
                
-               122         416 LOAD_GLOBAL             25 (NULL + sleep)
+               121         416 LOAD_GLOBAL             25 (NULL + sleep)
                
-               123         428 LOAD_FAST                0 (self)
+               122         428 LOAD_FAST                0 (self)
                            430 LOAD_ATTR               13 (delay_between_requests)
                
-               124         440 LOAD_FAST                0 (self)
+               123         440 LOAD_FAST                0 (self)
                            442 LOAD_ATTR               14 (profile)
                            452 POP_JUMP_FORWARD_IF_FALSE    12 (to 478)
                            454 LOAD_FAST                0 (self)
                            456 LOAD_ATTR               14 (profile)
                            466 LOAD_ATTR               15 (id)
                            476 JUMP_FORWARD             1 (to 480)
                        >>  478 LOAD_CONST               0 (None)
                
-               125     >>  480 LOAD_FAST                0 (self)
+               124     >>  480 LOAD_FAST                0 (self)
                            482 LOAD_ATTR               16 (sleep_echo)
                
-               122         492 KW_NAMES                 2
+               121         492 KW_NAMES                 2
                            494 PRECALL                  3
                            498 CALL                     3
                            508 GET_AWAITABLE            0
                            510 LOAD_CONST               0 (None)
                        >>  512 SEND                     3 (to 520)
                            514 YIELD_VALUE
                            516 RESUME                   3
                            518 JUMP_BACKWARD_NO_INTERRUPT     4 (to 512)
                        >>  520 POP_TOP
                
-               127         522 LOAD_GLOBAL             37 (NULL + TokenAmount)
+               126         522 LOAD_GLOBAL             37 (NULL + TokenAmount)
                            534 LOAD_FAST                4 (amount)
                            536 LOAD_FAST                5 (decimals)
                            538 LOAD_CONST               4 (True)
                            540 KW_NAMES                 5
                            542 PRECALL                  3
                            546 CALL                     3
                            556 RETURN_VALUE
@@ -1436,15 +1436,15 @@
                   ('amount', 'decimals', 'wei')
                names      ('w3', 'eth', 'contract', 'AsyncWeb3', 'to_checksum_address', 'DefaultABIs', 'Token', 'functions', 'allowance', 'account', 'address', 'call', 'sleep', 'delay_between_requests', 'profile', 'id', 'sleep_echo', 'get_decimals', 'TokenAmount')
                varnames   ('self', 'spender', 'contract', 'token_address', 'amount', 'decimals')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\client.py'
                name       'get_allowance'
-               firstlineno 109
+               firstlineno 108
                lnotab
                   0x060404017a017a010c010c0128010cfd1e0538010c010c0128010cfd1e
                   05
             'w3'
             'block'
             code
                argcount  : 2
@@ -1461,108 +1461,108 @@
                   0400000000000000000000000000000000000000007c0664021900000000
                   0000000000a6010000ab01000000000000000001008c3e2300740a000000
                   0000000000000024007203010059008c4a77007803590077017c04730d7c
                   006a0000000000000000006a0600000000000000007d076e2c7c04a00700
                   00000000000000000000000000000000000000a6000000ab000000000000
                   00000001007c047411000000000000000000007c04a6010000ab01000000
                   000000000064037a020000190000000000000000007d077c075300
-               129           0 RETURN_GENERATOR
+               128           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               131           6 LOAD_FAST                1 (block)
+               130           6 LOAD_FAST                1 (block)
                              8 LOAD_CONST               1 ('number')
                             10 BINARY_SUBSCR
                             20 STORE_FAST               2 (block_number)
                
-               132          22 LOAD_FAST                0 (w3)
+               131          22 LOAD_FAST                0 (w3)
                             24 LOAD_ATTR                0 (eth)
                             34 LOAD_METHOD              1 (get_block_transaction_count)
                             56 LOAD_FAST                2 (block_number)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 STORE_FAST               3 (latest_block_transaction_count)
                
-               133          74 BUILD_LIST               0
+               132          74 BUILD_LIST               0
                             76 STORE_FAST               4 (max_priority_fee_per_gas_lst)
                
-               134          78 LOAD_GLOBAL              5 (NULL + range)
+               133          78 LOAD_GLOBAL              5 (NULL + range)
                             90 LOAD_FAST                3 (latest_block_transaction_count)
                             92 PRECALL                  1
                             96 CALL                     1
                            106 GET_ITER
                        >>  108 FOR_ITER                77 (to 264)
                            110 STORE_FAST               5 (i)
                
-               135         112 NOP
+               134         112 NOP
                
-               136         114 LOAD_FAST                0 (w3)
+               135         114 LOAD_FAST                0 (w3)
                            116 LOAD_ATTR                0 (eth)
                            126 LOAD_METHOD              3 (get_transaction_by_block)
                            148 LOAD_FAST                2 (block_number)
                            150 LOAD_FAST                5 (i)
                            152 PRECALL                  2
                            156 CALL                     2
                            166 STORE_FAST               6 (transaction)
                
-               137         168 LOAD_CONST               2 ('maxPriorityFeePerGas')
+               136         168 LOAD_CONST               2 ('maxPriorityFeePerGas')
                            170 LOAD_FAST                6 (transaction)
                            172 CONTAINS_OP              0
                            174 POP_JUMP_FORWARD_IF_FALSE    27 (to 230)
                
-               138         176 LOAD_FAST                4 (max_priority_fee_per_gas_lst)
+               137         176 LOAD_FAST                4 (max_priority_fee_per_gas_lst)
                            178 LOAD_METHOD              4 (append)
                            200 LOAD_FAST                6 (transaction)
                            202 LOAD_CONST               2 ('maxPriorityFeePerGas')
                            204 BINARY_SUBSCR
                            214 PRECALL                  1
                            218 CALL                     1
                            228 POP_TOP
                        >>  230 JUMP_BACKWARD           62 (to 108)
                        >>  232 PUSH_EXC_INFO
                
-               139         234 LOAD_GLOBAL             10 (Exception)
+               138         234 LOAD_GLOBAL             10 (Exception)
                            246 CHECK_EXC_MATCH
                            248 POP_JUMP_FORWARD_IF_FALSE     3 (to 256)
                            250 POP_TOP
                
-               140         252 POP_EXCEPT
+               139         252 POP_EXCEPT
                            254 JUMP_BACKWARD           74 (to 108)
                
-               139     >>  256 RERAISE                  0
+               138     >>  256 RERAISE                  0
                        >>  258 COPY                     3
                            260 POP_EXCEPT
                            262 RERAISE                  1
                
-               142     >>  264 LOAD_FAST                4 (max_priority_fee_per_gas_lst)
+               141     >>  264 LOAD_FAST                4 (max_priority_fee_per_gas_lst)
                            266 POP_JUMP_FORWARD_IF_TRUE    13 (to 294)
                
-               143         268 LOAD_FAST                0 (w3)
+               142         268 LOAD_FAST                0 (w3)
                            270 LOAD_ATTR                0 (eth)
                            280 LOAD_ATTR                6 (max_priority_fee)
                            290 STORE_FAST               7 (max_priority_fee_per_gas)
                            292 JUMP_FORWARD            44 (to 382)
                
-               145     >>  294 LOAD_FAST                4 (max_priority_fee_per_gas_lst)
+               144     >>  294 LOAD_FAST                4 (max_priority_fee_per_gas_lst)
                            296 LOAD_METHOD              7 (sort)
                            318 PRECALL                  0
                            322 CALL                     0
                            332 POP_TOP
                
-               146         334 LOAD_FAST                4 (max_priority_fee_per_gas_lst)
+               145         334 LOAD_FAST                4 (max_priority_fee_per_gas_lst)
                            336 LOAD_GLOBAL             17 (NULL + len)
                            348 LOAD_FAST                4 (max_priority_fee_per_gas_lst)
                            350 PRECALL                  1
                            354 CALL                     1
                            364 LOAD_CONST               3 (2)
                            366 BINARY_OP                2 (//)
                            370 BINARY_SUBSCR
                            380 STORE_FAST               7 (max_priority_fee_per_gas)
                
-               147     >>  382 LOAD_FAST                7 (max_priority_fee_per_gas)
+               146     >>  382 LOAD_FAST                7 (max_priority_fee_per_gas)
                            384 RETURN_VALUE
                ExceptionTable:
                  114 to 228 -> 232 [1]
                  232 to 250 -> 258 [2] lasti
                  256 to 256 -> 258 [2] lasti
                consts
                   None
@@ -1571,15 +1571,15 @@
                   2
                names      ('eth', 'get_block_transaction_count', 'range', 'get_transaction_by_block', 'append', 'Exception', 'max_priority_fee', 'sort', 'len')
                varnames   ('w3', 'block', 'block_number', 'latest_block_transaction_count', 'max_priority_fee_per_gas_lst', 'i', 'transaction', 'max_priority_fee_per_gas')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\client.py'
                name       'get_max_priority_fee_per_gas'
-               firstlineno 129
+               firstlineno 128
                lnotab
                   0x060210013401040122010201360108013a01120104ff080304011a0228
                   013001
             'max_priority_fee_per_gas'
             'max_fee_per_gas'
             code
                argcount  : 8
@@ -1595,178 +1595,180 @@
                   010000ab010000000000000000740d000000000000000000006a07000000
                   00000000007c01a6010000ab01000000000000000064019c047d08741100
                   0000000000000000007c006a0900000000000000007c006a0a0000000000
                   000000720c7c006a0a00000000000000006a0b00000000000000006e0164
                   007c006a0c0000000000000000ac02a6030000ab03000000000000000083
                   0064007b0356009703860401007c0272057c027c0864033c0000007c0572
                   057c057c0864043c0000007c006a0300000000000000006a0d0000000000
-                  000000728509007c006a0e0000000000000000a00f000000000000000000
+                  00000072a009007c006a0e0000000000000000a00f000000000000000000
                   00000000000000000000007c006a0e00000000000000006a100000000000
                   0000006a110000000000000000830064007b035600970386046406a60200
                   00ab0200000000000000007d097c097c006a0300000000000000006a0d00
-                  000000000000006b040000000072427425000000000000000000006a1300
+                  000000000000006b0400000000725d7425000000000000000000006a1300
                   000000000000007c006a1400000000000000009b0064077c099b0064087c
                   006a0300000000000000006a0d00000000000000009b0064099d06a60100
-                  00ab0100000000000000000100741100000000000000000000640aa60100
-                  00ab010000000000000000830064007b0356009703860401006e016e018c
-                  847c006a0300000000000000006a15000000000000000072de7c006a0e00
-                  000000000000006a100000000000000000a0160000000000000000000000
-                  000000000000000000640ba6010000ab010000000000000000830064007b
-                  035600970386047d0a7411000000000000000000007c006a090000000000
+                  00ab0100000000000000000100741100000000000000000000640a7c006a
+                  0a0000000000000000720c7c006a0a00000000000000006a0b0000000000
+                  0000006e0164007c006a0c0000000000000000ac02a6030000ab03000000
+                  0000000000830064007b0356009703860401006e016e018c9f7c006a0300
+                  000000000000006a15000000000000000072de7c006a0e00000000000000
+                  006a100000000000000000a0160000000000000000000000000000000000
+                  000000640ba6010000ab010000000000000000830064007b035600970386
+                  047d0a7411000000000000000000007c006a0900000000000000007c006a
+                  0a0000000000000000720c7c006a0a00000000000000006a0b0000000000
+                  0000006e0164007c006a0c0000000000000000ac02a6030000ab03000000
+                  0000000000830064007b0356009703860401007c06804c7c006a0e000000
+                  00000000006a1000000000000000006a170000000000000000830064007b
+                  035600970386047d067411000000000000000000007c006a090000000000
                   0000007c006a0a0000000000000000720c7c006a0a00000000000000006a
                   0b00000000000000006e0164007c006a0c0000000000000000ac02a60300
-                  00ab030000000000000000830064007b0356009703860401007c06804c7c
-                  006a0e00000000000000006a1000000000000000006a1700000000000000
-                  00830064007b035600970386047d067411000000000000000000007c006a
-                  0900000000000000007c006a0a0000000000000000720c7c006a0a000000
-                  00000000006a0b00000000000000006e0164007c006a0c00000000000000
-                  00ac02a6030000ab030000000000000000830064007b0356009703860401
-                  007c067c08640c3c0000007c07700a7c0a640d190000000000000000007c
-                  067a0000007c08640e3c0000007431000000000000000000007c08640e19
-                  0000000000000000007c006a1900000000000000007a050000a6010000ab
-                  0100000000000000007c08640e3c0000006e1a7c006a0e00000000000000
-                  006a1000000000000000006a110000000000000000830064007b03560097
-                  0386047c08640f3c00000009007c006a0e00000000000000006a10000000
-                  0000000000a01a00000000000000000000000000000000000000007c08a6
-                  010000ab010000000000000000830064007b035600970386047d0b743100
-                  0000000000000000007c0b7c047a050000a6010000ab0100000000000000
-                  007c0864103c0000007411000000000000000000007c006a090000000000
-                  0000007c006a0a0000000000000000720c7c006a0a00000000000000006a
-                  0b00000000000000006e0164007c006a0c0000000000000000ac02a60300
-                  00ab030000000000000000830064007b0356009703860401006e40230074
-                  360000000000000000000074380000000000000000000066022400722c7d
-                  0c7425000000000000000000006a1d00000000000000007c006a14000000
-                  00000000009b0064117c0c9b009d03a6010000ab01000000000000000001
-                  0064127c0c66026302590064007d0c7e0c530064007d0c7e0c7701770078
-                  035900770109007c006a0e00000000000000006a1000000000000000006a
-                  000000000000000000a01e00000000000000000000000000000000000000
-                  007c087c006a0000000000000000006a1f0000000000000000a020000000
-                  0000000000000000000000000000000000a6000000ab0000000000000000
-                  00a6020000ab0200000000000000007d0d09007c006a0e00000000000000
-                  006a100000000000000000a0210000000000000000000000000000000000
-                  0000007c0d6a220000000000000000a6010000ab01000000000000000083
-                  0064007b03560097038604a0200000000000000000000000000000000000
-                  000000a6000000ab0000000000000000007d0e6ebd230074380000000000
-                  00000000002400727c7d0f64137c0f6a2300000000000000006414190000
-                  000000000000006415190000000000000000007600731564167c0f6a2300
-                  000000000000006414190000000000000000006415190000000000000000
-                  00760072157c086417780278021900000000000000000064187a0d000063
-                  0363023c000000590064007d0f7e0f8cc97425000000000000000000006a
-                  2400000000000000007c006a1400000000000000009b0064197c0f6a2300
-                  000000000000006414190000000000000000006415190000000000000000
-                  009b009d03a6010000ab010000000000000000010064127c0f6602630259
-                  0064007d0f7e0f530064007d0f7e0f7701744a0000000000000000000024
-                  00722c7d0f7425000000000000000000006a2400000000000000007c006a
-                  1400000000000000009b0064197c0f9b009d03a6010000ab010000000000
-                  000000010064127c0f66026302590064007d0f7e0f530064007d0f7e0f77
-                  0177007803590077017425000000000000000000006a2600000000000000
-                  007c006a1400000000000000009b00641a7c0e9b00641b9d04a6010000ab
-                  010000000000000000010064057c0e66025300
-               149           0 RETURN_GENERATOR
+                  00ab030000000000000000830064007b0356009703860401007c067c0864
+                  0c3c0000007c07700a7c0a640d190000000000000000007c067a0000007c
+                  08640e3c0000007431000000000000000000007c08640e19000000000000
+                  0000007c006a1900000000000000007a050000a6010000ab010000000000
+                  0000007c08640e3c0000006e1a7c006a0e00000000000000006a10000000
+                  00000000006a110000000000000000830064007b035600970386047c0864
+                  0f3c00000009007c006a0e00000000000000006a100000000000000000a0
+                  1a00000000000000000000000000000000000000007c08a6010000ab0100
+                  00000000000000830064007b035600970386047d0b743100000000000000
+                  0000007c0b7c047a050000a6010000ab0100000000000000007c0864103c
+                  0000007411000000000000000000007c006a0900000000000000007c006a
+                  0a0000000000000000720c7c006a0a00000000000000006a0b0000000000
+                  0000006e0164007c006a0c0000000000000000ac02a6030000ab03000000
+                  0000000000830064007b0356009703860401006e40230074360000000000
+                  000000000074380000000000000000000066022400722c7d0c7425000000
+                  000000000000006a1d00000000000000007c006a1400000000000000009b
+                  0064117c0c9b009d03a6010000ab010000000000000000010064127c0c66
+                  026302590064007d0c7e0c530064007d0c7e0c7701770078035900770109
+                  007c006a0e00000000000000006a1000000000000000006a000000000000
+                  000000a01e00000000000000000000000000000000000000007c087c006a
+                  0000000000000000006a1f0000000000000000a020000000000000000000
+                  0000000000000000000000a6000000ab000000000000000000a6020000ab
+                  0200000000000000007d0d09007c006a0e00000000000000006a10000000
+                  0000000000a02100000000000000000000000000000000000000007c0d6a
+                  220000000000000000a6010000ab010000000000000000830064007b0356
+                  0097038604a0200000000000000000000000000000000000000000a60000
+                  00ab0000000000000000007d0e6ebd230074380000000000000000000024
+                  00727c7d0f64137c0f6a2300000000000000006414190000000000000000
+                  006415190000000000000000007600731564167c0f6a2300000000000000
+                  00641419000000000000000000641519000000000000000000760072157c
+                  086417780278021900000000000000000064187a0d0000630363023c0000
+                  00590064007d0f7e0f8cc97425000000000000000000006a240000000000
+                  0000007c006a1400000000000000009b0064197c0f6a2300000000000000
+                  006414190000000000000000006415190000000000000000009b009d03a6
+                  010000ab010000000000000000010064127c0f66026302590064007d0f7e
+                  0f530064007d0f7e0f7701744a000000000000000000002400722c7d0f74
+                  25000000000000000000006a2400000000000000007c006a140000000000
+                  0000009b0064197c0f9b009d03a6010000ab010000000000000000010064
+                  127c0f66026302590064007d0f7e0f530064007d0f7e0f77017700780359
+                  0077017425000000000000000000006a2600000000000000007c006a1400
+                  000000000000009b00641a7c0e9b00641b9d04a6010000ab010000000000
+                  000000010064057c0e66025300
+               148           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               159           6 LOAD_FAST                3 (from_)
+               158           6 LOAD_FAST                3 (from_)
                              8 POP_JUMP_FORWARD_IF_TRUE    12 (to 34)
                
-               160          10 LOAD_FAST                0 (self)
+               159          10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (account)
                             22 LOAD_ATTR                1 (address)
                             32 STORE_FAST               3 (from_)
                
-               161     >>   34 LOAD_FAST                4 (increase_gas_limit)
+               160     >>   34 LOAD_FAST                4 (increase_gas_limit)
                             36 POP_JUMP_FORWARD_IF_TRUE     7 (to 52)
                
-               162          38 LOAD_FAST                0 (self)
+               161          38 LOAD_FAST                0 (self)
                             40 LOAD_ATTR                2 (INCREASE_GAS_LIMIT)
                             50 STORE_FAST               4 (increase_gas_limit)
                
-               165     >>   52 LOAD_FAST                0 (self)
+               164     >>   52 LOAD_FAST                0 (self)
                             54 LOAD_ATTR                3 (network)
                             64 LOAD_ATTR                4 (chain_id)
                
-               166          74 LOAD_FAST                0 (self)
+               165          74 LOAD_FAST                0 (self)
                             76 LOAD_METHOD              5 (nonce)
                             98 PRECALL                  0
                            102 CALL                     0
                            112 GET_AWAITABLE            0
                            114 LOAD_CONST               0 (None)
                        >>  116 SEND                     3 (to 124)
                            118 YIELD_VALUE
                            120 RESUME                   3
                            122 JUMP_BACKWARD_NO_INTERRUPT     4 (to 116)
                
-               167     >>  124 LOAD_GLOBAL             13 (NULL + AsyncWeb3)
+               166     >>  124 LOAD_GLOBAL             13 (NULL + AsyncWeb3)
                            136 LOAD_ATTR                7 (to_checksum_address)
                            146 LOAD_FAST                3 (from_)
                            148 PRECALL                  1
                            152 CALL                     1
                
-               168         162 LOAD_GLOBAL             13 (NULL + AsyncWeb3)
+               167         162 LOAD_GLOBAL             13 (NULL + AsyncWeb3)
                            174 LOAD_ATTR                7 (to_checksum_address)
                            184 LOAD_FAST                1 (to)
                            186 PRECALL                  1
                            190 CALL                     1
                
-               164         200 LOAD_CONST               1 (('chainId', 'nonce', 'from', 'to'))
+               163         200 LOAD_CONST               1 (('chainId', 'nonce', 'from', 'to'))
                            202 BUILD_CONST_KEY_MAP      4
                            204 STORE_FAST               8 (tx_params)
                
-               170         206 LOAD_GLOBAL             17 (NULL + sleep)
+               169         206 LOAD_GLOBAL             17 (NULL + sleep)
                
-               171         218 LOAD_FAST                0 (self)
+               170         218 LOAD_FAST                0 (self)
                            220 LOAD_ATTR                9 (delay_between_requests)
                
-               172         230 LOAD_FAST                0 (self)
+               171         230 LOAD_FAST                0 (self)
                            232 LOAD_ATTR               10 (profile)
                            242 POP_JUMP_FORWARD_IF_FALSE    12 (to 268)
                            244 LOAD_FAST                0 (self)
                            246 LOAD_ATTR               10 (profile)
                            256 LOAD_ATTR               11 (id)
                            266 JUMP_FORWARD             1 (to 270)
                        >>  268 LOAD_CONST               0 (None)
                
-               173     >>  270 LOAD_FAST                0 (self)
+               172     >>  270 LOAD_FAST                0 (self)
                            272 LOAD_ATTR               12 (sleep_echo)
                
-               170         282 KW_NAMES                 2
+               169         282 KW_NAMES                 2
                            284 PRECALL                  3
                            288 CALL                     3
                            298 GET_AWAITABLE            0
                            300 LOAD_CONST               0 (None)
                        >>  302 SEND                     3 (to 310)
                            304 YIELD_VALUE
                            306 RESUME                   3
                            308 JUMP_BACKWARD_NO_INTERRUPT     4 (to 302)
                        >>  310 POP_TOP
                
-               175         312 LOAD_FAST                2 (data)
+               174         312 LOAD_FAST                2 (data)
                            314 POP_JUMP_FORWARD_IF_FALSE     5 (to 326)
                
-               176         316 LOAD_FAST                2 (data)
+               175         316 LOAD_FAST                2 (data)
                            318 LOAD_FAST                8 (tx_params)
                            320 LOAD_CONST               3 ('data')
                            322 STORE_SUBSCR
                
-               177     >>  326 LOAD_FAST                5 (value)
+               176     >>  326 LOAD_FAST                5 (value)
                            328 POP_JUMP_FORWARD_IF_FALSE     5 (to 340)
                
-               178         330 LOAD_FAST                5 (value)
+               177         330 LOAD_FAST                5 (value)
                            332 LOAD_FAST                8 (tx_params)
                            334 LOAD_CONST               4 ('value')
                            336 STORE_SUBSCR
                
-               180     >>  340 LOAD_FAST                0 (self)
+               179     >>  340 LOAD_FAST                0 (self)
                            342 LOAD_ATTR                3 (network)
                            352 LOAD_ATTR               13 (max_gwei)
-                           362 POP_JUMP_FORWARD_IF_FALSE   133 (to 630)
+                           362 POP_JUMP_FORWARD_IF_FALSE   160 (to 684)
                
-               181         364 NOP
+               180         364 NOP
                
-               182     >>  366 LOAD_FAST                0 (self)
+               181     >>  366 LOAD_FAST                0 (self)
                            368 LOAD_ATTR               14 (w3)
                            378 LOAD_METHOD             15 (from_wei)
                            400 LOAD_FAST                0 (self)
                            402 LOAD_ATTR               14 (w3)
                            412 LOAD_ATTR               16 (eth)
                            422 LOAD_ATTR               17 (gas_price)
                            432 GET_AWAITABLE            0
@@ -1776,475 +1778,486 @@
                            440 RESUME                   3
                            442 JUMP_BACKWARD_NO_INTERRUPT     4 (to 436)
                        >>  444 LOAD_CONST               6 ('gwei')
                            446 PRECALL                  2
                            450 CALL                     2
                            460 STORE_FAST               9 (gas_price)
                
-               183         462 LOAD_FAST                9 (gas_price)
+               182         462 LOAD_FAST                9 (gas_price)
                            464 LOAD_FAST                0 (self)
                            466 LOAD_ATTR                3 (network)
                            476 LOAD_ATTR               13 (max_gwei)
                            486 COMPARE_OP               4 (>)
-                           492 POP_JUMP_FORWARD_IF_FALSE    66 (to 626)
+                           492 POP_JUMP_FORWARD_IF_FALSE    93 (to 680)
                
-               184         494 LOAD_GLOBAL             37 (NULL + logger)
+               183         494 LOAD_GLOBAL             37 (NULL + logger)
                            506 LOAD_ATTR               19 (debug)
                
-               185         516 LOAD_FAST                0 (self)
+               184         516 LOAD_FAST                0 (self)
                            518 LOAD_ATTR               20 (log_info)
                            528 FORMAT_VALUE             0
                            530 LOAD_CONST               7 (' | Current GWEI: ')
                            532 LOAD_FAST                9 (gas_price)
                            534 FORMAT_VALUE             0
                            536 LOAD_CONST               8 (' > ')
                            538 LOAD_FAST                0 (self)
                            540 LOAD_ATTR                3 (network)
                            550 LOAD_ATTR               13 (max_gwei)
                            560 FORMAT_VALUE             0
                            562 LOAD_CONST               9 ('. Waiting for gwei...')
                            564 BUILD_STRING             6
                
-               184         566 PRECALL                  1
+               183         566 PRECALL                  1
                            570 CALL                     1
                            580 POP_TOP
                
-               187         582 LOAD_GLOBAL             17 (NULL + sleep)
+               186         582 LOAD_GLOBAL             17 (NULL + sleep)
                            594 LOAD_CONST              10 (15)
-                           596 PRECALL                  1
-                           600 CALL                     1
-                           610 GET_AWAITABLE            0
-                           612 LOAD_CONST               0 (None)
-                       >>  614 SEND                     3 (to 622)
-                           616 YIELD_VALUE
-                           618 RESUME                   3
-                           620 JUMP_BACKWARD_NO_INTERRUPT     4 (to 614)
-                       >>  622 POP_TOP
-                           624 JUMP_FORWARD             1 (to 628)
-               
-               189     >>  626 JUMP_FORWARD             1 (to 630)
-               
-               181     >>  628 JUMP_BACKWARD          132 (to 366)
-               
-               191     >>  630 LOAD_FAST                0 (self)
-                           632 LOAD_ATTR                3 (network)
-                           642 LOAD_ATTR               21 (eip1559_tx)
-                           652 POP_JUMP_FORWARD_IF_FALSE   222 (to 1098)
-               
-               192         654 LOAD_FAST                0 (self)
-                           656 LOAD_ATTR               14 (w3)
-                           666 LOAD_ATTR               16 (eth)
-                           676 LOAD_METHOD             22 (get_block)
-                           698 LOAD_CONST              11 ('latest')
-                           700 PRECALL                  1
-                           704 CALL                     1
-                           714 GET_AWAITABLE            0
-                           716 LOAD_CONST               0 (None)
-                       >>  718 SEND                     3 (to 726)
-                           720 YIELD_VALUE
-                           722 RESUME                   3
-                           724 JUMP_BACKWARD_NO_INTERRUPT     4 (to 718)
-                       >>  726 STORE_FAST              10 (last_block)
-               
-               193         728 LOAD_GLOBAL             17 (NULL + sleep)
-               
-               194         740 LOAD_FAST                0 (self)
-                           742 LOAD_ATTR                9 (delay_between_requests)
-               
-               195         752 LOAD_FAST                0 (self)
-                           754 LOAD_ATTR               10 (profile)
-                           764 POP_JUMP_FORWARD_IF_FALSE    12 (to 790)
-                           766 LOAD_FAST                0 (self)
-                           768 LOAD_ATTR               10 (profile)
-                           778 LOAD_ATTR               11 (id)
-                           788 JUMP_FORWARD             1 (to 792)
-                       >>  790 LOAD_CONST               0 (None)
-               
-               196     >>  792 LOAD_FAST                0 (self)
-                           794 LOAD_ATTR               12 (sleep_echo)
-               
-               193         804 KW_NAMES                 2
-                           806 PRECALL                  3
-                           810 CALL                     3
-                           820 GET_AWAITABLE            0
-                           822 LOAD_CONST               0 (None)
-                       >>  824 SEND                     3 (to 832)
-                           826 YIELD_VALUE
-                           828 RESUME                   3
-                           830 JUMP_BACKWARD_NO_INTERRUPT     4 (to 824)
-                       >>  832 POP_TOP
-               
-               198         834 LOAD_FAST                6 (max_priority_fee_per_gas)
-                           836 POP_JUMP_FORWARD_IF_NOT_NONE    76 (to 990)
-               
-               200         838 LOAD_FAST                0 (self)
-                           840 LOAD_ATTR               14 (w3)
-                           850 LOAD_ATTR               16 (eth)
-                           860 LOAD_ATTR               23 (max_priority_fee)
-                           870 GET_AWAITABLE            0
-                           872 LOAD_CONST               0 (None)
-                       >>  874 SEND                     3 (to 882)
-                           876 YIELD_VALUE
-                           878 RESUME                   3
-                           880 JUMP_BACKWARD_NO_INTERRUPT     4 (to 874)
-                       >>  882 STORE_FAST               6 (max_priority_fee_per_gas)
-               
-               201         884 LOAD_GLOBAL             17 (NULL + sleep)
-               
-               202         896 LOAD_FAST                0 (self)
-                           898 LOAD_ATTR                9 (delay_between_requests)
-               
-               203         908 LOAD_FAST                0 (self)
-                           910 LOAD_ATTR               10 (profile)
-                           920 POP_JUMP_FORWARD_IF_FALSE    12 (to 946)
-                           922 LOAD_FAST                0 (self)
-                           924 LOAD_ATTR               10 (profile)
-                           934 LOAD_ATTR               11 (id)
-                           944 JUMP_FORWARD             1 (to 948)
-                       >>  946 LOAD_CONST               0 (None)
-               
-               204     >>  948 LOAD_FAST                0 (self)
-                           950 LOAD_ATTR               12 (sleep_echo)
-               
-               201         960 KW_NAMES                 2
-                           962 PRECALL                  3
-                           966 CALL                     3
-                           976 GET_AWAITABLE            0
-                           978 LOAD_CONST               0 (None)
-                       >>  980 SEND                     3 (to 988)
-                           982 YIELD_VALUE
-                           984 RESUME                   3
-                           986 JUMP_BACKWARD_NO_INTERRUPT     4 (to 980)
-                       >>  988 POP_TOP
-               
-               206     >>  990 LOAD_FAST                6 (max_priority_fee_per_gas)
-                           992 LOAD_FAST                8 (tx_params)
-                           994 LOAD_CONST              12 ('maxPriorityFeePerGas')
-                           996 STORE_SUBSCR
-               
-               207        1000 LOAD_FAST                7 (max_fee_per_gas)
-                          1002 JUMP_IF_TRUE_OR_POP     10 (to 1024)
-                          1004 LOAD_FAST               10 (last_block)
-                          1006 LOAD_CONST              13 ('baseFeePerGas')
-                          1008 BINARY_SUBSCR
-                          1018 LOAD_FAST                6 (max_priority_fee_per_gas)
-                          1020 BINARY_OP                0 (+)
-                       >> 1024 LOAD_FAST                8 (tx_params)
-                          1026 LOAD_CONST              14 ('maxFeePerGas')
-                          1028 STORE_SUBSCR
-               
-               208        1032 LOAD_GLOBAL             49 (NULL + int)
-                          1044 LOAD_FAST                8 (tx_params)
-                          1046 LOAD_CONST              14 ('maxFeePerGas')
-                          1048 BINARY_SUBSCR
-                          1058 LOAD_FAST                0 (self)
-                          1060 LOAD_ATTR               25 (INCREASE_GWEI)
-                          1070 BINARY_OP                5 (*)
-                          1074 PRECALL                  1
-                          1078 CALL                     1
-                          1088 LOAD_FAST                8 (tx_params)
-                          1090 LOAD_CONST              14 ('maxFeePerGas')
-                          1092 STORE_SUBSCR
-                          1096 JUMP_FORWARD            26 (to 1150)
-               
-               211     >> 1098 LOAD_FAST                0 (self)
-                          1100 LOAD_ATTR               14 (w3)
-                          1110 LOAD_ATTR               16 (eth)
-                          1120 LOAD_ATTR               17 (gas_price)
-                          1130 GET_AWAITABLE            0
-                          1132 LOAD_CONST               0 (None)
-                       >> 1134 SEND                     3 (to 1142)
-                          1136 YIELD_VALUE
-                          1138 RESUME                   3
-                          1140 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1134)
-                       >> 1142 LOAD_FAST                8 (tx_params)
-                          1144 LOAD_CONST              15 ('gasPrice')
+                           596 LOAD_FAST                0 (self)
+                           598 LOAD_ATTR               10 (profile)
+                           608 POP_JUMP_FORWARD_IF_FALSE    12 (to 634)
+                           610 LOAD_FAST                0 (self)
+                           612 LOAD_ATTR               10 (profile)
+                           622 LOAD_ATTR               11 (id)
+                           632 JUMP_FORWARD             1 (to 636)
+                       >>  634 LOAD_CONST               0 (None)
+                       >>  636 LOAD_FAST                0 (self)
+                           638 LOAD_ATTR               12 (sleep_echo)
+                           648 KW_NAMES                 2
+                           650 PRECALL                  3
+                           654 CALL                     3
+                           664 GET_AWAITABLE            0
+                           666 LOAD_CONST               0 (None)
+                       >>  668 SEND                     3 (to 676)
+                           670 YIELD_VALUE
+                           672 RESUME                   3
+                           674 JUMP_BACKWARD_NO_INTERRUPT     4 (to 668)
+                       >>  676 POP_TOP
+                           678 JUMP_FORWARD             1 (to 682)
+               
+               188     >>  680 JUMP_FORWARD             1 (to 684)
+               
+               180     >>  682 JUMP_BACKWARD          159 (to 366)
+               
+               190     >>  684 LOAD_FAST                0 (self)
+                           686 LOAD_ATTR                3 (network)
+                           696 LOAD_ATTR               21 (eip1559_tx)
+                           706 POP_JUMP_FORWARD_IF_FALSE   222 (to 1152)
+               
+               191         708 LOAD_FAST                0 (self)
+                           710 LOAD_ATTR               14 (w3)
+                           720 LOAD_ATTR               16 (eth)
+                           730 LOAD_METHOD             22 (get_block)
+                           752 LOAD_CONST              11 ('latest')
+                           754 PRECALL                  1
+                           758 CALL                     1
+                           768 GET_AWAITABLE            0
+                           770 LOAD_CONST               0 (None)
+                       >>  772 SEND                     3 (to 780)
+                           774 YIELD_VALUE
+                           776 RESUME                   3
+                           778 JUMP_BACKWARD_NO_INTERRUPT     4 (to 772)
+                       >>  780 STORE_FAST              10 (last_block)
+               
+               192         782 LOAD_GLOBAL             17 (NULL + sleep)
+               
+               193         794 LOAD_FAST                0 (self)
+                           796 LOAD_ATTR                9 (delay_between_requests)
+               
+               194         806 LOAD_FAST                0 (self)
+                           808 LOAD_ATTR               10 (profile)
+                           818 POP_JUMP_FORWARD_IF_FALSE    12 (to 844)
+                           820 LOAD_FAST                0 (self)
+                           822 LOAD_ATTR               10 (profile)
+                           832 LOAD_ATTR               11 (id)
+                           842 JUMP_FORWARD             1 (to 846)
+                       >>  844 LOAD_CONST               0 (None)
+               
+               195     >>  846 LOAD_FAST                0 (self)
+                           848 LOAD_ATTR               12 (sleep_echo)
+               
+               192         858 KW_NAMES                 2
+                           860 PRECALL                  3
+                           864 CALL                     3
+                           874 GET_AWAITABLE            0
+                           876 LOAD_CONST               0 (None)
+                       >>  878 SEND                     3 (to 886)
+                           880 YIELD_VALUE
+                           882 RESUME                   3
+                           884 JUMP_BACKWARD_NO_INTERRUPT     4 (to 878)
+                       >>  886 POP_TOP
+               
+               197         888 LOAD_FAST                6 (max_priority_fee_per_gas)
+                           890 POP_JUMP_FORWARD_IF_NOT_NONE    76 (to 1044)
+               
+               199         892 LOAD_FAST                0 (self)
+                           894 LOAD_ATTR               14 (w3)
+                           904 LOAD_ATTR               16 (eth)
+                           914 LOAD_ATTR               23 (max_priority_fee)
+                           924 GET_AWAITABLE            0
+                           926 LOAD_CONST               0 (None)
+                       >>  928 SEND                     3 (to 936)
+                           930 YIELD_VALUE
+                           932 RESUME                   3
+                           934 JUMP_BACKWARD_NO_INTERRUPT     4 (to 928)
+                       >>  936 STORE_FAST               6 (max_priority_fee_per_gas)
+               
+               200         938 LOAD_GLOBAL             17 (NULL + sleep)
+               
+               201         950 LOAD_FAST                0 (self)
+                           952 LOAD_ATTR                9 (delay_between_requests)
+               
+               202         962 LOAD_FAST                0 (self)
+                           964 LOAD_ATTR               10 (profile)
+                           974 POP_JUMP_FORWARD_IF_FALSE    12 (to 1000)
+                           976 LOAD_FAST                0 (self)
+                           978 LOAD_ATTR               10 (profile)
+                           988 LOAD_ATTR               11 (id)
+                           998 JUMP_FORWARD             1 (to 1002)
+                       >> 1000 LOAD_CONST               0 (None)
+               
+               203     >> 1002 LOAD_FAST                0 (self)
+                          1004 LOAD_ATTR               12 (sleep_echo)
+               
+               200        1014 KW_NAMES                 2
+                          1016 PRECALL                  3
+                          1020 CALL                     3
+                          1030 GET_AWAITABLE            0
+                          1032 LOAD_CONST               0 (None)
+                       >> 1034 SEND                     3 (to 1042)
+                          1036 YIELD_VALUE
+                          1038 RESUME                   3
+                          1040 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1034)
+                       >> 1042 POP_TOP
+               
+               205     >> 1044 LOAD_FAST                6 (max_priority_fee_per_gas)
+                          1046 LOAD_FAST                8 (tx_params)
+                          1048 LOAD_CONST              12 ('maxPriorityFeePerGas')
+                          1050 STORE_SUBSCR
+               
+               206        1054 LOAD_FAST                7 (max_fee_per_gas)
+                          1056 JUMP_IF_TRUE_OR_POP     10 (to 1078)
+                          1058 LOAD_FAST               10 (last_block)
+                          1060 LOAD_CONST              13 ('baseFeePerGas')
+                          1062 BINARY_SUBSCR
+                          1072 LOAD_FAST                6 (max_priority_fee_per_gas)
+                          1074 BINARY_OP                0 (+)
+                       >> 1078 LOAD_FAST                8 (tx_params)
+                          1080 LOAD_CONST              14 ('maxFeePerGas')
+                          1082 STORE_SUBSCR
+               
+               207        1086 LOAD_GLOBAL             49 (NULL + int)
+                          1098 LOAD_FAST                8 (tx_params)
+                          1100 LOAD_CONST              14 ('maxFeePerGas')
+                          1102 BINARY_SUBSCR
+                          1112 LOAD_FAST                0 (self)
+                          1114 LOAD_ATTR               25 (INCREASE_GWEI)
+                          1124 BINARY_OP                5 (*)
+                          1128 PRECALL                  1
+                          1132 CALL                     1
+                          1142 LOAD_FAST                8 (tx_params)
+                          1144 LOAD_CONST              14 ('maxFeePerGas')
                           1146 STORE_SUBSCR
+                          1150 JUMP_FORWARD            26 (to 1204)
                
-               213     >> 1150 NOP
-               
-               214        1152 LOAD_FAST                0 (self)
+               210     >> 1152 LOAD_FAST                0 (self)
                           1154 LOAD_ATTR               14 (w3)
                           1164 LOAD_ATTR               16 (eth)
-                          1174 LOAD_METHOD             26 (estimate_gas)
-                          1196 LOAD_FAST                8 (tx_params)
-                          1198 PRECALL                  1
-                          1202 CALL                     1
-                          1212 GET_AWAITABLE            0
-                          1214 LOAD_CONST               0 (None)
-                       >> 1216 SEND                     3 (to 1224)
-                          1218 YIELD_VALUE
-                          1220 RESUME                   3
-                          1222 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1216)
-                       >> 1224 STORE_FAST              11 (estimated_gas_limit)
-               
-               215        1226 LOAD_GLOBAL             49 (NULL + int)
-                          1238 LOAD_FAST               11 (estimated_gas_limit)
-                          1240 LOAD_FAST                4 (increase_gas_limit)
-                          1242 BINARY_OP                5 (*)
-                          1246 PRECALL                  1
-                          1250 CALL                     1
-                          1260 LOAD_FAST                8 (tx_params)
-                          1262 LOAD_CONST              16 ('gas')
-                          1264 STORE_SUBSCR
-               
-               216        1268 LOAD_GLOBAL             17 (NULL + sleep)
-               
-               217        1280 LOAD_FAST                0 (self)
-                          1282 LOAD_ATTR                9 (delay_between_requests)
-               
-               218        1292 LOAD_FAST                0 (self)
-                          1294 LOAD_ATTR               10 (profile)
-                          1304 POP_JUMP_FORWARD_IF_FALSE    12 (to 1330)
-                          1306 LOAD_FAST                0 (self)
-                          1308 LOAD_ATTR               10 (profile)
-                          1318 LOAD_ATTR               11 (id)
-                          1328 JUMP_FORWARD             1 (to 1332)
-                       >> 1330 LOAD_CONST               0 (None)
-               
-               219     >> 1332 LOAD_FAST                0 (self)
-                          1334 LOAD_ATTR               12 (sleep_echo)
-               
-               216        1344 KW_NAMES                 2
-                          1346 PRECALL                  3
-                          1350 CALL                     3
-                          1360 GET_AWAITABLE            0
-                          1362 LOAD_CONST               0 (None)
-                       >> 1364 SEND                     3 (to 1372)
-                          1366 YIELD_VALUE
-                          1368 RESUME                   3
-                          1370 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1364)
-                       >> 1372 POP_TOP
-                          1374 JUMP_FORWARD            64 (to 1504)
-                       >> 1376 PUSH_EXC_INFO
-               
-               221        1378 LOAD_GLOBAL             54 (ContractLogicError)
-                          1390 LOAD_GLOBAL             56 (ValueError)
-                          1402 BUILD_TUPLE              2
-                          1404 CHECK_EXC_MATCH
-                          1406 POP_JUMP_FORWARD_IF_FALSE    44 (to 1496)
-                          1408 STORE_FAST              12 (err)
-               
-               222        1410 LOAD_GLOBAL             37 (NULL + logger)
-                          1422 LOAD_ATTR               29 (warning)
-                          1432 LOAD_FAST                0 (self)
-                          1434 LOAD_ATTR               20 (log_info)
-                          1444 FORMAT_VALUE             0
-                          1446 LOAD_CONST              17 (" | Couldn't estimate gas. Transaction wasn't send - ")
-                          1448 LOAD_FAST               12 (err)
-                          1450 FORMAT_VALUE             0
-                          1452 BUILD_STRING             3
-                          1454 PRECALL                  1
-                          1458 CALL                     1
-                          1468 POP_TOP
-               
-               223        1470 LOAD_CONST              18 (False)
-                          1472 LOAD_FAST               12 (err)
-                          1474 BUILD_TUPLE              2
-                          1476 SWAP                     2
-                          1478 POP_EXCEPT
-                          1480 LOAD_CONST               0 (None)
-                          1482 STORE_FAST              12 (err)
-                          1484 DELETE_FAST             12 (err)
-                          1486 RETURN_VALUE
-                       >> 1488 LOAD_CONST               0 (None)
-                          1490 STORE_FAST              12 (err)
-                          1492 DELETE_FAST             12 (err)
-                          1494 RERAISE                  1
-               
-               221     >> 1496 RERAISE                  0
-                       >> 1498 COPY                     3
-                          1500 POP_EXCEPT
-                          1502 RERAISE                  1
-               
-               224     >> 1504 NOP
-               
-               225        1506 LOAD_FAST                0 (self)
-                          1508 LOAD_ATTR               14 (w3)
-                          1518 LOAD_ATTR               16 (eth)
-                          1528 LOAD_ATTR                0 (account)
-                          1538 LOAD_METHOD             30 (sign_transaction)
-                          1560 LOAD_FAST                8 (tx_params)
-                          1562 LOAD_FAST                0 (self)
-                          1564 LOAD_ATTR                0 (account)
-                          1574 LOAD_ATTR               31 (key)
-                          1584 LOAD_METHOD             32 (hex)
-                          1606 PRECALL                  0
-                          1610 CALL                     0
-                          1620 PRECALL                  2
-                          1624 CALL                     2
-                          1634 STORE_FAST              13 (sign)
-               
-               227        1636 NOP
-               
-               228        1638 LOAD_FAST                0 (self)
-                          1640 LOAD_ATTR               14 (w3)
-                          1650 LOAD_ATTR               16 (eth)
-                          1660 LOAD_METHOD             33 (send_raw_transaction)
-                          1682 LOAD_FAST               13 (sign)
-                          1684 LOAD_ATTR               34 (rawTransaction)
-                          1694 PRECALL                  1
-                          1698 CALL                     1
-                          1708 GET_AWAITABLE            0
-                          1710 LOAD_CONST               0 (None)
-                       >> 1712 SEND                     3 (to 1720)
-                          1714 YIELD_VALUE
-                          1716 RESUME                   3
-                          1718 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1712)
-                       >> 1720 LOAD_METHOD             32 (hex)
-                          1742 PRECALL                  0
-                          1746 CALL                     0
-                          1756 STORE_FAST              14 (tx_hash)
-               
-               229        1758 JUMP_FORWARD           189 (to 2138)
-                       >> 1760 PUSH_EXC_INFO
-               
-               230        1762 LOAD_GLOBAL             56 (ValueError)
-                          1774 CHECK_EXC_MATCH
-                          1776 POP_JUMP_FORWARD_IF_FALSE   124 (to 2026)
-                          1778 STORE_FAST              15 (e)
-               
-               231        1780 LOAD_CONST              19 ('invalid nonce')
-                          1782 LOAD_FAST               15 (e)
-                          1784 LOAD_ATTR               35 (args)
-                          1794 LOAD_CONST              20 (0)
-                          1796 BINARY_SUBSCR
-                          1806 LOAD_CONST              21 ('message')
-                          1808 BINARY_SUBSCR
-                          1818 CONTAINS_OP              0
-                          1820 POP_JUMP_FORWARD_IF_TRUE    21 (to 1864)
-                          1822 LOAD_CONST              22 ('nonce too low')
-                          1824 LOAD_FAST               15 (e)
-                          1826 LOAD_ATTR               35 (args)
-                          1836 LOAD_CONST              20 (0)
-                          1838 BINARY_SUBSCR
-                          1848 LOAD_CONST              21 ('message')
+                          1174 LOAD_ATTR               17 (gas_price)
+                          1184 GET_AWAITABLE            0
+                          1186 LOAD_CONST               0 (None)
+                       >> 1188 SEND                     3 (to 1196)
+                          1190 YIELD_VALUE
+                          1192 RESUME                   3
+                          1194 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1188)
+                       >> 1196 LOAD_FAST                8 (tx_params)
+                          1198 LOAD_CONST              15 ('gasPrice')
+                          1200 STORE_SUBSCR
+               
+               212     >> 1204 NOP
+               
+               213        1206 LOAD_FAST                0 (self)
+                          1208 LOAD_ATTR               14 (w3)
+                          1218 LOAD_ATTR               16 (eth)
+                          1228 LOAD_METHOD             26 (estimate_gas)
+                          1250 LOAD_FAST                8 (tx_params)
+                          1252 PRECALL                  1
+                          1256 CALL                     1
+                          1266 GET_AWAITABLE            0
+                          1268 LOAD_CONST               0 (None)
+                       >> 1270 SEND                     3 (to 1278)
+                          1272 YIELD_VALUE
+                          1274 RESUME                   3
+                          1276 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1270)
+                       >> 1278 STORE_FAST              11 (estimated_gas_limit)
+               
+               214        1280 LOAD_GLOBAL             49 (NULL + int)
+                          1292 LOAD_FAST               11 (estimated_gas_limit)
+                          1294 LOAD_FAST                4 (increase_gas_limit)
+                          1296 BINARY_OP                5 (*)
+                          1300 PRECALL                  1
+                          1304 CALL                     1
+                          1314 LOAD_FAST                8 (tx_params)
+                          1316 LOAD_CONST              16 ('gas')
+                          1318 STORE_SUBSCR
+               
+               215        1322 LOAD_GLOBAL             17 (NULL + sleep)
+               
+               216        1334 LOAD_FAST                0 (self)
+                          1336 LOAD_ATTR                9 (delay_between_requests)
+               
+               217        1346 LOAD_FAST                0 (self)
+                          1348 LOAD_ATTR               10 (profile)
+                          1358 POP_JUMP_FORWARD_IF_FALSE    12 (to 1384)
+                          1360 LOAD_FAST                0 (self)
+                          1362 LOAD_ATTR               10 (profile)
+                          1372 LOAD_ATTR               11 (id)
+                          1382 JUMP_FORWARD             1 (to 1386)
+                       >> 1384 LOAD_CONST               0 (None)
+               
+               218     >> 1386 LOAD_FAST                0 (self)
+                          1388 LOAD_ATTR               12 (sleep_echo)
+               
+               215        1398 KW_NAMES                 2
+                          1400 PRECALL                  3
+                          1404 CALL                     3
+                          1414 GET_AWAITABLE            0
+                          1416 LOAD_CONST               0 (None)
+                       >> 1418 SEND                     3 (to 1426)
+                          1420 YIELD_VALUE
+                          1422 RESUME                   3
+                          1424 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1418)
+                       >> 1426 POP_TOP
+                          1428 JUMP_FORWARD            64 (to 1558)
+                       >> 1430 PUSH_EXC_INFO
+               
+               220        1432 LOAD_GLOBAL             54 (ContractLogicError)
+                          1444 LOAD_GLOBAL             56 (ValueError)
+                          1456 BUILD_TUPLE              2
+                          1458 CHECK_EXC_MATCH
+                          1460 POP_JUMP_FORWARD_IF_FALSE    44 (to 1550)
+                          1462 STORE_FAST              12 (err)
+               
+               221        1464 LOAD_GLOBAL             37 (NULL + logger)
+                          1476 LOAD_ATTR               29 (warning)
+                          1486 LOAD_FAST                0 (self)
+                          1488 LOAD_ATTR               20 (log_info)
+                          1498 FORMAT_VALUE             0
+                          1500 LOAD_CONST              17 (" | Couldn't estimate gas. Transaction wasn't send - ")
+                          1502 LOAD_FAST               12 (err)
+                          1504 FORMAT_VALUE             0
+                          1506 BUILD_STRING             3
+                          1508 PRECALL                  1
+                          1512 CALL                     1
+                          1522 POP_TOP
+               
+               222        1524 LOAD_CONST              18 (False)
+                          1526 LOAD_FAST               12 (err)
+                          1528 BUILD_TUPLE              2
+                          1530 SWAP                     2
+                          1532 POP_EXCEPT
+                          1534 LOAD_CONST               0 (None)
+                          1536 STORE_FAST              12 (err)
+                          1538 DELETE_FAST             12 (err)
+                          1540 RETURN_VALUE
+                       >> 1542 LOAD_CONST               0 (None)
+                          1544 STORE_FAST              12 (err)
+                          1546 DELETE_FAST             12 (err)
+                          1548 RERAISE                  1
+               
+               220     >> 1550 RERAISE                  0
+                       >> 1552 COPY                     3
+                          1554 POP_EXCEPT
+                          1556 RERAISE                  1
+               
+               223     >> 1558 NOP
+               
+               224        1560 LOAD_FAST                0 (self)
+                          1562 LOAD_ATTR               14 (w3)
+                          1572 LOAD_ATTR               16 (eth)
+                          1582 LOAD_ATTR                0 (account)
+                          1592 LOAD_METHOD             30 (sign_transaction)
+                          1614 LOAD_FAST                8 (tx_params)
+                          1616 LOAD_FAST                0 (self)
+                          1618 LOAD_ATTR                0 (account)
+                          1628 LOAD_ATTR               31 (key)
+                          1638 LOAD_METHOD             32 (hex)
+                          1660 PRECALL                  0
+                          1664 CALL                     0
+                          1674 PRECALL                  2
+                          1678 CALL                     2
+                          1688 STORE_FAST              13 (sign)
+               
+               226        1690 NOP
+               
+               227        1692 LOAD_FAST                0 (self)
+                          1694 LOAD_ATTR               14 (w3)
+                          1704 LOAD_ATTR               16 (eth)
+                          1714 LOAD_METHOD             33 (send_raw_transaction)
+                          1736 LOAD_FAST               13 (sign)
+                          1738 LOAD_ATTR               34 (rawTransaction)
+                          1748 PRECALL                  1
+                          1752 CALL                     1
+                          1762 GET_AWAITABLE            0
+                          1764 LOAD_CONST               0 (None)
+                       >> 1766 SEND                     3 (to 1774)
+                          1768 YIELD_VALUE
+                          1770 RESUME                   3
+                          1772 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1766)
+                       >> 1774 LOAD_METHOD             32 (hex)
+                          1796 PRECALL                  0
+                          1800 CALL                     0
+                          1810 STORE_FAST              14 (tx_hash)
+               
+               228        1812 JUMP_FORWARD           189 (to 2192)
+                       >> 1814 PUSH_EXC_INFO
+               
+               229        1816 LOAD_GLOBAL             56 (ValueError)
+                          1828 CHECK_EXC_MATCH
+                          1830 POP_JUMP_FORWARD_IF_FALSE   124 (to 2080)
+                          1832 STORE_FAST              15 (e)
+               
+               230        1834 LOAD_CONST              19 ('invalid nonce')
+                          1836 LOAD_FAST               15 (e)
+                          1838 LOAD_ATTR               35 (args)
+                          1848 LOAD_CONST              20 (0)
                           1850 BINARY_SUBSCR
-                          1860 CONTAINS_OP              0
-                          1862 POP_JUMP_FORWARD_IF_FALSE    21 (to 1906)
-               
-               232     >> 1864 LOAD_FAST                8 (tx_params)
-                          1866 LOAD_CONST              23 ('nonce')
-                          1868 COPY                     2
-                          1870 COPY                     2
-                          1872 BINARY_SUBSCR
-                          1882 LOAD_CONST              24 (1)
-                          1884 BINARY_OP               13 (+=)
-                          1888 SWAP                     3
-                          1890 SWAP                     2
-                          1892 STORE_SUBSCR
-               
-               233        1896 POP_EXCEPT
-                          1898 LOAD_CONST               0 (None)
-                          1900 STORE_FAST              15 (e)
-                          1902 DELETE_FAST             15 (e)
-                          1904 JUMP_BACKWARD          201 (to 1504)
-               
-               234     >> 1906 LOAD_GLOBAL             37 (NULL + logger)
-                          1918 LOAD_ATTR               36 (error)
-                          1928 LOAD_FAST                0 (self)
-                          1930 LOAD_ATTR               20 (log_info)
-                          1940 FORMAT_VALUE             0
-                          1942 LOAD_CONST              25 (' | ')
-                          1944 LOAD_FAST               15 (e)
-                          1946 LOAD_ATTR               35 (args)
-                          1956 LOAD_CONST              20 (0)
-                          1958 BINARY_SUBSCR
-                          1968 LOAD_CONST              21 ('message')
-                          1970 BINARY_SUBSCR
-                          1980 FORMAT_VALUE             0
-                          1982 BUILD_STRING             3
-                          1984 PRECALL                  1
-                          1988 CALL                     1
-                          1998 POP_TOP
-               
-               235        2000 LOAD_CONST              18 (False)
-                          2002 LOAD_FAST               15 (e)
-                          2004 BUILD_TUPLE              2
-                          2006 SWAP                     2
-                          2008 POP_EXCEPT
-                          2010 LOAD_CONST               0 (None)
-                          2012 STORE_FAST              15 (e)
-                          2014 DELETE_FAST             15 (e)
-                          2016 RETURN_VALUE
-                       >> 2018 LOAD_CONST               0 (None)
-                          2020 STORE_FAST              15 (e)
-                          2022 DELETE_FAST             15 (e)
-                          2024 RERAISE                  1
-               
-               236     >> 2026 LOAD_GLOBAL             74 (Exception)
-                          2038 CHECK_EXC_MATCH
-                          2040 POP_JUMP_FORWARD_IF_FALSE    44 (to 2130)
-                          2042 STORE_FAST              15 (e)
-               
-               237        2044 LOAD_GLOBAL             37 (NULL + logger)
-                          2056 LOAD_ATTR               36 (error)
-                          2066 LOAD_FAST                0 (self)
-                          2068 LOAD_ATTR               20 (log_info)
-                          2078 FORMAT_VALUE             0
-                          2080 LOAD_CONST              25 (' | ')
-                          2082 LOAD_FAST               15 (e)
-                          2084 FORMAT_VALUE             0
-                          2086 BUILD_STRING             3
-                          2088 PRECALL                  1
-                          2092 CALL                     1
-                          2102 POP_TOP
-               
-               238        2104 LOAD_CONST              18 (False)
-                          2106 LOAD_FAST               15 (e)
-                          2108 BUILD_TUPLE              2
-                          2110 SWAP                     2
-                          2112 POP_EXCEPT
-                          2114 LOAD_CONST               0 (None)
-                          2116 STORE_FAST              15 (e)
-                          2118 DELETE_FAST             15 (e)
-                          2120 RETURN_VALUE
-                       >> 2122 LOAD_CONST               0 (None)
-                          2124 STORE_FAST              15 (e)
-                          2126 DELETE_FAST             15 (e)
-                          2128 RERAISE                  1
-               
-               236     >> 2130 RERAISE                  0
-                       >> 2132 COPY                     3
-                          2134 POP_EXCEPT
-                          2136 RERAISE                  1
-               
-               239     >> 2138 LOAD_GLOBAL             37 (NULL + logger)
-                          2150 LOAD_ATTR               38 (info)
-                          2160 LOAD_FAST                0 (self)
-                          2162 LOAD_ATTR               20 (log_info)
-                          2172 FORMAT_VALUE             0
-                          2174 LOAD_CONST              26 (' | Transaction ')
-                          2176 LOAD_FAST               14 (tx_hash)
-                          2178 FORMAT_VALUE             0
-                          2180 LOAD_CONST              27 (' sent')
-                          2182 BUILD_STRING             4
-                          2184 PRECALL                  1
-                          2188 CALL                     1
-                          2198 POP_TOP
-               
-               240        2200 LOAD_CONST               5 (True)
-                          2202 LOAD_FAST               14 (tx_hash)
-                          2204 BUILD_TUPLE              2
-                          2206 RETURN_VALUE
+                          1860 LOAD_CONST              21 ('message')
+                          1862 BINARY_SUBSCR
+                          1872 CONTAINS_OP              0
+                          1874 POP_JUMP_FORWARD_IF_TRUE    21 (to 1918)
+                          1876 LOAD_CONST              22 ('nonce too low')
+                          1878 LOAD_FAST               15 (e)
+                          1880 LOAD_ATTR               35 (args)
+                          1890 LOAD_CONST              20 (0)
+                          1892 BINARY_SUBSCR
+                          1902 LOAD_CONST              21 ('message')
+                          1904 BINARY_SUBSCR
+                          1914 CONTAINS_OP              0
+                          1916 POP_JUMP_FORWARD_IF_FALSE    21 (to 1960)
+               
+               231     >> 1918 LOAD_FAST                8 (tx_params)
+                          1920 LOAD_CONST              23 ('nonce')
+                          1922 COPY                     2
+                          1924 COPY                     2
+                          1926 BINARY_SUBSCR
+                          1936 LOAD_CONST              24 (1)
+                          1938 BINARY_OP               13 (+=)
+                          1942 SWAP                     3
+                          1944 SWAP                     2
+                          1946 STORE_SUBSCR
+               
+               232        1950 POP_EXCEPT
+                          1952 LOAD_CONST               0 (None)
+                          1954 STORE_FAST              15 (e)
+                          1956 DELETE_FAST             15 (e)
+                          1958 JUMP_BACKWARD          201 (to 1558)
+               
+               233     >> 1960 LOAD_GLOBAL             37 (NULL + logger)
+                          1972 LOAD_ATTR               36 (error)
+                          1982 LOAD_FAST                0 (self)
+                          1984 LOAD_ATTR               20 (log_info)
+                          1994 FORMAT_VALUE             0
+                          1996 LOAD_CONST              25 (' | ')
+                          1998 LOAD_FAST               15 (e)
+                          2000 LOAD_ATTR               35 (args)
+                          2010 LOAD_CONST              20 (0)
+                          2012 BINARY_SUBSCR
+                          2022 LOAD_CONST              21 ('message')
+                          2024 BINARY_SUBSCR
+                          2034 FORMAT_VALUE             0
+                          2036 BUILD_STRING             3
+                          2038 PRECALL                  1
+                          2042 CALL                     1
+                          2052 POP_TOP
+               
+               234        2054 LOAD_CONST              18 (False)
+                          2056 LOAD_FAST               15 (e)
+                          2058 BUILD_TUPLE              2
+                          2060 SWAP                     2
+                          2062 POP_EXCEPT
+                          2064 LOAD_CONST               0 (None)
+                          2066 STORE_FAST              15 (e)
+                          2068 DELETE_FAST             15 (e)
+                          2070 RETURN_VALUE
+                       >> 2072 LOAD_CONST               0 (None)
+                          2074 STORE_FAST              15 (e)
+                          2076 DELETE_FAST             15 (e)
+                          2078 RERAISE                  1
+               
+               235     >> 2080 LOAD_GLOBAL             74 (Exception)
+                          2092 CHECK_EXC_MATCH
+                          2094 POP_JUMP_FORWARD_IF_FALSE    44 (to 2184)
+                          2096 STORE_FAST              15 (e)
+               
+               236        2098 LOAD_GLOBAL             37 (NULL + logger)
+                          2110 LOAD_ATTR               36 (error)
+                          2120 LOAD_FAST                0 (self)
+                          2122 LOAD_ATTR               20 (log_info)
+                          2132 FORMAT_VALUE             0
+                          2134 LOAD_CONST              25 (' | ')
+                          2136 LOAD_FAST               15 (e)
+                          2138 FORMAT_VALUE             0
+                          2140 BUILD_STRING             3
+                          2142 PRECALL                  1
+                          2146 CALL                     1
+                          2156 POP_TOP
+               
+               237        2158 LOAD_CONST              18 (False)
+                          2160 LOAD_FAST               15 (e)
+                          2162 BUILD_TUPLE              2
+                          2164 SWAP                     2
+                          2166 POP_EXCEPT
+                          2168 LOAD_CONST               0 (None)
+                          2170 STORE_FAST              15 (e)
+                          2172 DELETE_FAST             15 (e)
+                          2174 RETURN_VALUE
+                       >> 2176 LOAD_CONST               0 (None)
+                          2178 STORE_FAST              15 (e)
+                          2180 DELETE_FAST             15 (e)
+                          2182 RERAISE                  1
+               
+               235     >> 2184 RERAISE                  0
+                       >> 2186 COPY                     3
+                          2188 POP_EXCEPT
+                          2190 RERAISE                  1
+               
+               238     >> 2192 LOAD_GLOBAL             37 (NULL + logger)
+                          2204 LOAD_ATTR               38 (info)
+                          2214 LOAD_FAST                0 (self)
+                          2216 LOAD_ATTR               20 (log_info)
+                          2226 FORMAT_VALUE             0
+                          2228 LOAD_CONST              26 (' | Transaction ')
+                          2230 LOAD_FAST               14 (tx_hash)
+                          2232 FORMAT_VALUE             0
+                          2234 LOAD_CONST              27 (' sent')
+                          2236 BUILD_STRING             4
+                          2238 PRECALL                  1
+                          2242 CALL                     1
+                          2252 POP_TOP
+               
+               239        2254 LOAD_CONST               5 (True)
+                          2256 LOAD_FAST               14 (tx_hash)
+                          2258 BUILD_TUPLE              2
+                          2260 RETURN_VALUE
                ExceptionTable:
-                 1152 to 1372 -> 1376 [0]
-                 1376 to 1408 -> 1498 [1] lasti
-                 1410 to 1474 -> 1488 [1] lasti
-                 1476 to 1476 -> 1498 [1] lasti
-                 1488 to 1496 -> 1498 [1] lasti
-                 1638 to 1756 -> 1760 [0]
-                 1760 to 1778 -> 2132 [1] lasti
-                 1780 to 1894 -> 2018 [1] lasti
-                 1906 to 2004 -> 2018 [1] lasti
-                 2006 to 2006 -> 2132 [1] lasti
-                 2018 to 2042 -> 2132 [1] lasti
-                 2044 to 2108 -> 2122 [1] lasti
-                 2110 to 2110 -> 2132 [1] lasti
-                 2122 to 2130 -> 2132 [1] lasti
+                 1206 to 1426 -> 1430 [0]
+                 1430 to 1462 -> 1552 [1] lasti
+                 1464 to 1528 -> 1542 [1] lasti
+                 1530 to 1530 -> 1552 [1] lasti
+                 1542 to 1550 -> 1552 [1] lasti
+                 1692 to 1810 -> 1814 [0]
+                 1814 to 1832 -> 2186 [1] lasti
+                 1834 to 1948 -> 2072 [1] lasti
+                 1960 to 2058 -> 2072 [1] lasti
+                 2060 to 2060 -> 2186 [1] lasti
+                 2072 to 2096 -> 2186 [1] lasti
+                 2098 to 2162 -> 2176 [1] lasti
+                 2164 to 2164 -> 2186 [1] lasti
+                 2176 to 2184 -> 2186 [1] lasti
                consts
                   None
                   ('chainId', 'nonce', 'from', 'to')
                   ('profile_id', 'echo')
                   'data'
                   'value'
                   True
@@ -2272,18 +2285,18 @@
                   ' sent'
                names      ('account', 'address', 'INCREASE_GAS_LIMIT', 'network', 'chain_id', 'nonce', 'AsyncWeb3', 'to_checksum_address', 'sleep', 'delay_between_requests', 'profile', 'id', 'sleep_echo', 'max_gwei', 'w3', 'from_wei', 'eth', 'gas_price', 'logger', 'debug', 'log_info', 'eip1559_tx', 'get_block', 'max_priority_fee', 'int', 'INCREASE_GWEI', 'estimate_gas', 'ContractLogicError', 'ValueError', 'warning', 'sign_transaction', 'key', 'hex', 'send_raw_transaction', 'rawTransaction', 'args', 'error', 'Exception', 'info')
                varnames   ('self', 'to', 'data', 'from_', 'increase_gas_limit', 'value', 'max_priority_fee_per_gas', 'max_fee_per_gas', 'tx_params', 'gas_price', 'last_block', 'estimated_gas_limit', 'err', 'sign', 'tx_hash', 'e')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\client.py'
                name       'send_transaction'
-               firstlineno 149
+               firstlineno 148
                lnotab
                   0x060a0401180104010e0316013201260126fc06060c010c0128010cfd1e
-                  0504010a0104010a021801020160012001160132ff10032c0202f8020a18
+                  0504010a0104010a021801020160012001160132ff1003620202f8020a18
                   014a010c010c0128010cfd1e0504022e010c010c0128010cfd1e050a0120
                   014203340202014a012a010c010c0128010cfd220520013c011afe080302
                   0182020201780104011201540120010a015e011a0112013c011afe08033e
                   01
             'tx_hash'
             'tx_name'
             code
@@ -2308,49 +2321,49 @@
                   010000ab01000000000000000001007c006a0a0000000000000000730659
                   0064007d047e0464095300590064007d047e046e3f64007d047e04770174
                   16000000000000000000002400722f7d057407000000000000000000006a
                   0900000000000000007c006a0500000000000000009b0064047c029b0064
                   057c019b0064077c059b009d07a6010000ab010000000000000000010059
                   0064007d057e056409530064007d057e057701770078035900770190018c
                   19
-               242           0 RETURN_GENERATOR
+               241           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               243           6 NOP
+               242           6 NOP
                
-               244     >>    8 NOP
+               243     >>    8 NOP
                
-               245          10 LOAD_FAST                0 (self)
+               244          10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (w3)
                             22 LOAD_ATTR                1 (eth)
                             32 LOAD_METHOD              2 (wait_for_transaction_receipt)
                             54 LOAD_FAST                1 (tx_hash)
                             56 PRECALL                  1
                             60 CALL                     1
                             70 GET_AWAITABLE            0
                             72 LOAD_CONST               0 (None)
                        >>   74 SEND                     3 (to 82)
                             76 YIELD_VALUE
                             78 RESUME                   3
                             80 JUMP_BACKWARD_NO_INTERRUPT     4 (to 74)
                        >>   82 STORE_FAST               3 (data)
                
-               246          84 LOAD_CONST               2 ('status')
+               245          84 LOAD_CONST               2 ('status')
                             86 LOAD_FAST                3 (data)
                             88 CONTAINS_OP              0
                             90 POP_JUMP_FORWARD_IF_FALSE    48 (to 188)
                             92 LOAD_FAST                3 (data)
                             94 LOAD_CONST               2 ('status')
                             96 BINARY_SUBSCR
                            106 LOAD_CONST               3 (1)
                            108 COMPARE_OP               2 (==)
                            114 POP_JUMP_FORWARD_IF_FALSE    36 (to 188)
                
-               247         116 LOAD_GLOBAL              7 (NULL + logger)
+               246         116 LOAD_GLOBAL              7 (NULL + logger)
                            128 LOAD_ATTR                4 (info)
                            138 LOAD_FAST                0 (self)
                            140 LOAD_ATTR                5 (log_info)
                            150 FORMAT_VALUE             0
                            152 LOAD_CONST               4 (' | Transaction ')
                            154 LOAD_FAST                2 (tx_name)
                            156 FORMAT_VALUE             0
@@ -2359,21 +2372,21 @@
                            162 FORMAT_VALUE             0
                            164 LOAD_CONST               6 (') was successful')
                            166 BUILD_STRING             6
                            168 PRECALL                  1
                            172 CALL                     1
                            182 POP_TOP
                
-               248         184 LOAD_CONST               1 (True)
+               247         184 LOAD_CONST               1 (True)
                            186 RETURN_VALUE
                
-               250     >>  188 LOAD_GLOBAL              7 (NULL + logger)
+               249     >>  188 LOAD_GLOBAL              7 (NULL + logger)
                            200 LOAD_ATTR                6 (error)
                
-               251         210 LOAD_FAST                0 (self)
+               250         210 LOAD_FAST                0 (self)
                            212 LOAD_ATTR                5 (log_info)
                            222 FORMAT_VALUE             0
                            224 LOAD_CONST               4 (' | Transaction ')
                            226 LOAD_FAST                2 (tx_name)
                            228 FORMAT_VALUE             0
                            230 LOAD_CONST               5 (' (')
                            232 LOAD_FAST                1 (tx_hash)
@@ -2384,28 +2397,28 @@
                            242 BINARY_SUBSCR
                            252 LOAD_METHOD              7 (hex)
                            274 PRECALL                  0
                            278 CALL                     0
                            288 FORMAT_VALUE             0
                            290 BUILD_STRING             7
                
-               250         292 PRECALL                  1
+               249         292 PRECALL                  1
                            296 CALL                     1
                            306 POP_TOP
                
-               253         308 LOAD_CONST               9 (False)
+               252         308 LOAD_CONST               9 (False)
                            310 RETURN_VALUE
                        >>  312 PUSH_EXC_INFO
                
-               254         314 LOAD_GLOBAL             16 (TimeExhausted)
+               253         314 LOAD_GLOBAL             16 (TimeExhausted)
                            326 CHECK_EXC_MATCH
                            328 POP_JUMP_FORWARD_IF_FALSE    59 (to 448)
                            330 STORE_FAST               4 (e)
                
-               255         332 LOAD_GLOBAL              7 (NULL + logger)
+               254         332 LOAD_GLOBAL              7 (NULL + logger)
                            344 LOAD_ATTR                9 (warning)
                            354 LOAD_FAST                0 (self)
                            356 LOAD_ATTR                5 (log_info)
                            366 FORMAT_VALUE             0
                            368 LOAD_CONST               4 (' | Transaction ')
                            370 LOAD_FAST                2 (tx_name)
                            372 FORMAT_VALUE             0
@@ -2416,41 +2429,41 @@
                            382 LOAD_FAST                4 (e)
                            384 FORMAT_VALUE             0
                            386 BUILD_STRING             7
                            388 PRECALL                  1
                            392 CALL                     1
                            402 POP_TOP
                
-               256         404 LOAD_FAST                0 (self)
+               255         404 LOAD_FAST                0 (self)
                            406 LOAD_ATTR               10 (do_no_matter_what)
                            416 POP_JUMP_FORWARD_IF_TRUE     6 (to 430)
                
-               257         418 POP_EXCEPT
+               256         418 POP_EXCEPT
                            420 LOAD_CONST               0 (None)
                            422 STORE_FAST               4 (e)
                            424 DELETE_FAST              4 (e)
                            426 LOAD_CONST               9 (False)
                            428 RETURN_VALUE
                
-               256     >>  430 POP_EXCEPT
+               255     >>  430 POP_EXCEPT
                            432 LOAD_CONST               0 (None)
                            434 STORE_FAST               4 (e)
                            436 DELETE_FAST              4 (e)
                            438 JUMP_FORWARD            63 (to 566)
                        >>  440 LOAD_CONST               0 (None)
                            442 STORE_FAST               4 (e)
                            444 DELETE_FAST              4 (e)
                            446 RERAISE                  1
                
-               258     >>  448 LOAD_GLOBAL             22 (Exception)
+               257     >>  448 LOAD_GLOBAL             22 (Exception)
                            460 CHECK_EXC_MATCH
                            462 POP_JUMP_FORWARD_IF_FALSE    47 (to 558)
                            464 STORE_FAST               5 (err)
                
-               259         466 LOAD_GLOBAL              7 (NULL + logger)
+               258         466 LOAD_GLOBAL              7 (NULL + logger)
                            478 LOAD_ATTR                9 (warning)
                            488 LOAD_FAST                0 (self)
                            490 LOAD_ATTR                5 (log_info)
                            500 FORMAT_VALUE             0
                            502 LOAD_CONST               4 (' | Transaction ')
                            504 LOAD_FAST                2 (tx_name)
                            506 FORMAT_VALUE             0
@@ -2461,31 +2474,31 @@
                            516 LOAD_FAST                5 (err)
                            518 FORMAT_VALUE             0
                            520 BUILD_STRING             7
                            522 PRECALL                  1
                            526 CALL                     1
                            536 POP_TOP
                
-               260         538 POP_EXCEPT
+               259         538 POP_EXCEPT
                            540 LOAD_CONST               0 (None)
                            542 STORE_FAST               5 (err)
                            544 DELETE_FAST              5 (err)
                            546 LOAD_CONST               9 (False)
                            548 RETURN_VALUE
                        >>  550 LOAD_CONST               0 (None)
                            552 STORE_FAST               5 (err)
                            554 DELETE_FAST              5 (err)
                            556 RERAISE                  1
                
-               258     >>  558 RERAISE                  0
+               257     >>  558 RERAISE                  0
                        >>  560 COPY                     3
                            562 POP_EXCEPT
                            564 RERAISE                  1
                
-               243     >>  566 EXTENDED_ARG             1
+               242     >>  566 EXTENDED_ARG             1
                            568 JUMP_BACKWARD          281 (to 8)
                ExceptionTable:
                  10 to 182 -> 312 [0]
                  188 to 306 -> 312 [0]
                  312 to 330 -> 560 [1] lasti
                  332 to 416 -> 440 [1] lasti
                  440 to 464 -> 560 [1] lasti
@@ -2504,15 +2517,15 @@
                   False
                names      ('w3', 'eth', 'wait_for_transaction_receipt', 'logger', 'info', 'log_info', 'error', 'hex', 'TimeExhausted', 'warning', 'do_no_matter_what', 'Exception')
                varnames   ('self', 'tx_hash', 'tx_name', 'data', 'e', 'err')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\client.py'
                name       'verify_transaction'
-               firstlineno 242
+               firstlineno 241
                lnotab
                   0x0601020102014a01200144010402160152ff10030601120148010e010c
                   ff12021201480114fe08f1
             '0x1249c58b'
             'to'
             'name'
             'data'
@@ -2545,45 +2558,45 @@
                   000000000000006a0d00000000000000006e0164007c006a0e0000000000
                   000000ac07a6030000ab030000000000000000830064007b035600970386
                   0401007c00a01100000000000000000000000000000000000000007c0a7c
                   02a6020000ab020000000000000000830064007b035600970386047d0b7c
                   0b721f740f000000000000000000006a0800000000000000007c006a0900
                   000000000000009b0064057c029b0064099d04a6010000ab010000000000
                   00000001007c0b5300
-               262           0 RETURN_GENERATOR
+               261           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               273           6 LOAD_GLOBAL              1 (NULL + isinstance)
+               272           6 LOAD_GLOBAL              1 (NULL + isinstance)
                             18 LOAD_FAST                4 (value)
                             20 LOAD_GLOBAL              2 (int)
                             32 PRECALL                  2
                             36 CALL                     2
                             46 POP_JUMP_FORWARD_IF_FALSE    17 (to 82)
                
-               274          48 LOAD_GLOBAL              5 (NULL + TokenAmount)
+               273          48 LOAD_GLOBAL              5 (NULL + TokenAmount)
                             60 LOAD_FAST                4 (value)
                             62 LOAD_CONST               1 (True)
                             64 KW_NAMES                 2
                             66 PRECALL                  2
                             70 CALL                     2
                             80 STORE_FAST               4 (value)
                
-               275     >>   82 LOAD_FAST                0 (self)
+               274     >>   82 LOAD_FAST                0 (self)
                             84 LOAD_ATTR                3 (w3)
                             94 LOAD_METHOD              4 (to_checksum_address)
                            116 LOAD_FAST                1 (to)
                            118 PRECALL                  1
                            122 CALL                     1
                            132 STORE_FAST               1 (to)
                
-               276         134 LOAD_FAST                8 (check_existing)
+               275         134 LOAD_FAST                8 (check_existing)
                            136 POP_JUMP_FORWARD_IF_FALSE   123 (to 384)
                
-               277         138 LOAD_FAST                0 (self)
+               276         138 LOAD_FAST                0 (self)
                            140 LOAD_METHOD              5 (balance_of)
                            162 LOAD_FAST                1 (to)
                            164 KW_NAMES                 3
                            166 PRECALL                  1
                            170 CALL                     1
                            180 GET_AWAITABLE            0
                            182 LOAD_CONST               0 (None)
@@ -2592,146 +2605,146 @@
                            188 RESUME                   3
                            190 JUMP_BACKWARD_NO_INTERRUPT     4 (to 184)
                        >>  192 LOAD_ATTR                6 (Ether)
                            202 LOAD_CONST               4 (0)
                            204 COMPARE_OP               4 (>)
                            210 POP_JUMP_FORWARD_IF_FALSE    33 (to 278)
                
-               278         212 LOAD_GLOBAL             15 (NULL + logger)
+               277         212 LOAD_GLOBAL             15 (NULL + logger)
                            224 LOAD_ATTR                8 (success)
                            234 LOAD_FAST                0 (self)
                            236 LOAD_ATTR                9 (log_info)
                            246 FORMAT_VALUE             0
                            248 LOAD_CONST               5 (' | ')
                            250 LOAD_FAST                2 (name)
                            252 FORMAT_VALUE             0
                            254 LOAD_CONST               6 (' already minted')
                            256 BUILD_STRING             4
                            258 PRECALL                  1
                            262 CALL                     1
                            272 POP_TOP
                
-               279         274 LOAD_CONST               1 (True)
+               278         274 LOAD_CONST               1 (True)
                            276 RETURN_VALUE
                
-               280     >>  278 LOAD_GLOBAL             21 (NULL + sleep)
+               279     >>  278 LOAD_GLOBAL             21 (NULL + sleep)
                
-               281         290 LOAD_FAST                0 (self)
+               280         290 LOAD_FAST                0 (self)
                            292 LOAD_ATTR               11 (delay_between_requests)
                
-               282         302 LOAD_FAST                0 (self)
+               281         302 LOAD_FAST                0 (self)
                            304 LOAD_ATTR               12 (profile)
                            314 POP_JUMP_FORWARD_IF_FALSE    12 (to 340)
                            316 LOAD_FAST                0 (self)
                            318 LOAD_ATTR               12 (profile)
                            328 LOAD_ATTR               13 (id)
                            338 JUMP_FORWARD             1 (to 342)
                        >>  340 LOAD_CONST               0 (None)
                
-               283     >>  342 LOAD_FAST                0 (self)
+               282     >>  342 LOAD_FAST                0 (self)
                            344 LOAD_ATTR               14 (sleep_echo)
                
-               280         354 KW_NAMES                 7
+               279         354 KW_NAMES                 7
                            356 PRECALL                  3
                            360 CALL                     3
                            370 GET_AWAITABLE            0
                            372 LOAD_CONST               0 (None)
                        >>  374 SEND                     3 (to 382)
                            376 YIELD_VALUE
                            378 RESUME                   3
                            380 JUMP_BACKWARD_NO_INTERRUPT     4 (to 374)
                        >>  382 POP_TOP
                
-               285     >>  384 LOAD_FAST                0 (self)
+               284     >>  384 LOAD_FAST                0 (self)
                            386 LOAD_METHOD             15 (send_transaction)
                
-               286         408 LOAD_FAST                1 (to)
+               285         408 LOAD_FAST                1 (to)
                            410 LOAD_FAST                3 (data)
                            412 LOAD_FAST                4 (value)
                            414 LOAD_ATTR               16 (Wei)
                
-               287         424 LOAD_FAST                5 (max_priority_fee_per_gas)
+               286         424 LOAD_FAST                5 (max_priority_fee_per_gas)
                
-               288         426 LOAD_FAST                6 (max_fee_per_gas)
+               287         426 LOAD_FAST                6 (max_fee_per_gas)
                
-               289         428 LOAD_FAST                7 (increase_gas_limit)
+               288         428 LOAD_FAST                7 (increase_gas_limit)
                
-               285         430 KW_NAMES                 8
+               284         430 KW_NAMES                 8
                            432 PRECALL                  6
                            436 CALL                     6
                            446 GET_AWAITABLE            0
                            448 LOAD_CONST               0 (None)
                        >>  450 SEND                     3 (to 458)
                            452 YIELD_VALUE
                            454 RESUME                   3
                            456 JUMP_BACKWARD_NO_INTERRUPT     4 (to 450)
                        >>  458 UNPACK_SEQUENCE          2
                            462 STORE_FAST               9 (ok)
                            464 STORE_FAST              10 (tx_hash_or_err)
                
-               291         466 LOAD_GLOBAL             21 (NULL + sleep)
+               290         466 LOAD_GLOBAL             21 (NULL + sleep)
                
-               292         478 LOAD_FAST                0 (self)
+               291         478 LOAD_FAST                0 (self)
                            480 LOAD_ATTR               11 (delay_between_requests)
                
-               293         490 LOAD_FAST                0 (self)
+               292         490 LOAD_FAST                0 (self)
                            492 LOAD_ATTR               12 (profile)
                            502 POP_JUMP_FORWARD_IF_FALSE    12 (to 528)
                            504 LOAD_FAST                0 (self)
                            506 LOAD_ATTR               12 (profile)
                            516 LOAD_ATTR               13 (id)
                            526 JUMP_FORWARD             1 (to 530)
                        >>  528 LOAD_CONST               0 (None)
                
-               294     >>  530 LOAD_FAST                0 (self)
+               293     >>  530 LOAD_FAST                0 (self)
                            532 LOAD_ATTR               14 (sleep_echo)
                
-               291         542 KW_NAMES                 7
+               290         542 KW_NAMES                 7
                            544 PRECALL                  3
                            548 CALL                     3
                            558 GET_AWAITABLE            0
                            560 LOAD_CONST               0 (None)
                        >>  562 SEND                     3 (to 570)
                            564 YIELD_VALUE
                            566 RESUME                   3
                            568 JUMP_BACKWARD_NO_INTERRUPT     4 (to 562)
                        >>  570 POP_TOP
                
-               296         572 LOAD_FAST                0 (self)
+               295         572 LOAD_FAST                0 (self)
                            574 LOAD_METHOD             17 (verify_transaction)
                            596 LOAD_FAST               10 (tx_hash_or_err)
                            598 LOAD_FAST                2 (name)
                            600 PRECALL                  2
                            604 CALL                     2
                            614 GET_AWAITABLE            0
                            616 LOAD_CONST               0 (None)
                        >>  618 SEND                     3 (to 626)
                            620 YIELD_VALUE
                            622 RESUME                   3
                            624 JUMP_BACKWARD_NO_INTERRUPT     4 (to 618)
                        >>  626 STORE_FAST              11 (res)
                
-               297         628 LOAD_FAST               11 (res)
+               296         628 LOAD_FAST               11 (res)
                            630 POP_JUMP_FORWARD_IF_FALSE    31 (to 694)
                
-               298         632 LOAD_GLOBAL             15 (NULL + logger)
+               297         632 LOAD_GLOBAL             15 (NULL + logger)
                            644 LOAD_ATTR                8 (success)
                            654 LOAD_FAST                0 (self)
                            656 LOAD_ATTR                9 (log_info)
                            666 FORMAT_VALUE             0
                            668 LOAD_CONST               5 (' | ')
                            670 LOAD_FAST                2 (name)
                            672 FORMAT_VALUE             0
                            674 LOAD_CONST               9 (' done')
                            676 BUILD_STRING             4
                            678 PRECALL                  1
                            682 CALL                     1
                            692 POP_TOP
                
-               299     >>  694 LOAD_FAST               11 (res)
+               298     >>  694 LOAD_FAST               11 (res)
                            696 RETURN_VALUE
                consts
                   None
                   True
                   ('wei',)
                   ('token_address',)
                   0
@@ -2742,15 +2755,15 @@
                   ' done'
                names      ('isinstance', 'int', 'TokenAmount', 'w3', 'to_checksum_address', 'balance_of', 'Ether', 'logger', 'success', 'log_info', 'sleep', 'delay_between_requests', 'profile', 'id', 'sleep_echo', 'send_transaction', 'Wei', 'verify_transaction')
                varnames   ('self', 'to', 'name', 'data', 'value', 'max_priority_fee_per_gas', 'max_fee_per_gas', 'increase_gas_limit', 'check_existing', 'ok', 'tx_hash_or_err', 'res')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\client.py'
                name       'tx'
-               firstlineno 262
+               firstlineno 261
                lnotab
                   0x060b2a012201340104014a013e0104010c010c0128010cfd1e05180110
                   010201020102fc24060c010c0128010cfd1e05380104013e01
             'amount'
             'abi'
             code
                argcount  : 6
@@ -2797,100 +2810,100 @@
                   000000ac0fa6020000ab020000000000000000830064007b035600970386
                   045c0200007d097d0a7417000000000000000000007c006a0c0000000000
                   0000007c006a0d0000000000000000720c7c006a0d00000000000000006a
                   0e00000000000000006e0164007c006a0f0000000000000000ac05a60300
                   00ab030000000000000000830064007b0356009703860401007c00a01c00
                   000000000000000000000000000000000000007c0a64107c079b009d02a6
                   020000ab020000000000000000830064007b035600970386045300
-               301           0 RETURN_GENERATOR
+               300           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               305           6 LOAD_GLOBAL              1 (NULL + isinstance)
+               304           6 LOAD_GLOBAL              1 (NULL + isinstance)
                             18 LOAD_FAST                4 (amount)
                             20 LOAD_GLOBAL              2 (int)
                             32 PRECALL                  2
                             36 CALL                     2
                             46 POP_JUMP_FORWARD_IF_FALSE    17 (to 82)
                
-               306          48 LOAD_GLOBAL              5 (NULL + TokenAmount)
+               305          48 LOAD_GLOBAL              5 (NULL + TokenAmount)
                             60 LOAD_FAST                4 (amount)
                             62 LOAD_CONST               1 (True)
                             64 KW_NAMES                 2
                             66 PRECALL                  2
                             70 CALL                     2
                             80 STORE_FAST               4 (amount)
                
-               307     >>   82 LOAD_FAST                2 (contract)
+               306     >>   82 LOAD_FAST                2 (contract)
                             84 POP_JUMP_FORWARD_IF_TRUE    63 (to 212)
                
-               308          86 LOAD_FAST                0 (self)
+               307          86 LOAD_FAST                0 (self)
                             88 LOAD_ATTR                3 (w3)
                             98 LOAD_ATTR                4 (eth)
                            108 LOAD_METHOD              5 (contract)
                
-               309         130 LOAD_GLOBAL             13 (NULL + AsyncWeb3)
+               308         130 LOAD_GLOBAL             13 (NULL + AsyncWeb3)
                            142 LOAD_ATTR                7 (to_checksum_address)
                            152 LOAD_FAST                3 (token_address)
                            154 PRECALL                  1
                            158 CALL                     1
                
-               310         168 LOAD_FAST                5 (abi)
+               309         168 LOAD_FAST                5 (abi)
                            170 JUMP_IF_TRUE_OR_POP     11 (to 194)
                            172 LOAD_GLOBAL             16 (DefaultABIs)
                            184 LOAD_ATTR                9 (Token)
                
-               308     >>  194 KW_NAMES                 3
+               307     >>  194 KW_NAMES                 3
                            196 PRECALL                  2
                            200 CALL                     2
                            210 STORE_FAST               2 (contract)
                
-               312     >>  212 LOAD_FAST                0 (self)
+               311     >>  212 LOAD_FAST                0 (self)
                            214 LOAD_METHOD             10 (balance_of)
                            236 LOAD_FAST                2 (contract)
                            238 KW_NAMES                 4
                            240 PRECALL                  1
                            244 CALL                     1
                            254 GET_AWAITABLE            0
                            256 LOAD_CONST               0 (None)
                        >>  258 SEND                     3 (to 266)
                            260 YIELD_VALUE
                            262 RESUME                   3
                            264 JUMP_BACKWARD_NO_INTERRUPT     4 (to 258)
                        >>  266 STORE_FAST               6 (balance)
                
-               313         268 LOAD_GLOBAL             23 (NULL + sleep)
+               312         268 LOAD_GLOBAL             23 (NULL + sleep)
                
-               314         280 LOAD_FAST                0 (self)
+               313         280 LOAD_FAST                0 (self)
                            282 LOAD_ATTR               12 (delay_between_requests)
                
-               315         292 LOAD_FAST                0 (self)
+               314         292 LOAD_FAST                0 (self)
                            294 LOAD_ATTR               13 (profile)
                            304 POP_JUMP_FORWARD_IF_FALSE    12 (to 330)
                            306 LOAD_FAST                0 (self)
                            308 LOAD_ATTR               13 (profile)
                            318 LOAD_ATTR               14 (id)
                            328 JUMP_FORWARD             1 (to 332)
                        >>  330 LOAD_CONST               0 (None)
                
-               316     >>  332 LOAD_FAST                0 (self)
+               315     >>  332 LOAD_FAST                0 (self)
                            334 LOAD_ATTR               15 (sleep_echo)
                
-               313         344 KW_NAMES                 5
+               312         344 KW_NAMES                 5
                            346 PRECALL                  3
                            350 CALL                     3
                            360 GET_AWAITABLE            0
                            362 LOAD_CONST               0 (None)
                        >>  364 SEND                     3 (to 372)
                            366 YIELD_VALUE
                            368 RESUME                   3
                            370 JUMP_BACKWARD_NO_INTERRUPT     4 (to 364)
                        >>  372 POP_TOP
                
-               318         374 LOAD_FAST                2 (contract)
+               317         374 LOAD_FAST                2 (contract)
                            376 LOAD_ATTR               16 (functions)
                            386 LOAD_METHOD             17 (symbol)
                            408 PRECALL                  0
                            412 CALL                     0
                            422 LOAD_METHOD             18 (call)
                            444 PRECALL                  0
                            448 CALL                     0
@@ -2898,49 +2911,49 @@
                            460 LOAD_CONST               0 (None)
                        >>  462 SEND                     3 (to 470)
                            464 YIELD_VALUE
                            466 RESUME                   3
                            468 JUMP_BACKWARD_NO_INTERRUPT     4 (to 462)
                        >>  470 STORE_FAST               7 (token_symbol)
                
-               319         472 LOAD_GLOBAL             23 (NULL + sleep)
+               318         472 LOAD_GLOBAL             23 (NULL + sleep)
                
-               320         484 LOAD_FAST                0 (self)
+               319         484 LOAD_FAST                0 (self)
                            486 LOAD_ATTR               12 (delay_between_requests)
                
-               321         496 LOAD_FAST                0 (self)
+               320         496 LOAD_FAST                0 (self)
                            498 LOAD_ATTR               13 (profile)
                            508 POP_JUMP_FORWARD_IF_FALSE    12 (to 534)
                            510 LOAD_FAST                0 (self)
                            512 LOAD_ATTR               13 (profile)
                            522 LOAD_ATTR               14 (id)
                            532 JUMP_FORWARD             1 (to 536)
                        >>  534 LOAD_CONST               0 (None)
                
-               322     >>  536 LOAD_FAST                0 (self)
+               321     >>  536 LOAD_FAST                0 (self)
                            538 LOAD_ATTR               15 (sleep_echo)
                
-               319         548 KW_NAMES                 5
+               318         548 KW_NAMES                 5
                            550 PRECALL                  3
                            554 CALL                     3
                            564 GET_AWAITABLE            0
                            566 LOAD_CONST               0 (None)
                        >>  568 SEND                     3 (to 576)
                            570 YIELD_VALUE
                            572 RESUME                   3
                            574 JUMP_BACKWARD_NO_INTERRUPT     4 (to 568)
                        >>  576 POP_TOP
                
-               325         578 LOAD_FAST                6 (balance)
+               324         578 LOAD_FAST                6 (balance)
                            580 LOAD_ATTR               19 (Wei)
                            590 LOAD_CONST               6 (0)
                            592 COMPARE_OP               1 (<=)
                            598 POP_JUMP_FORWARD_IF_FALSE    41 (to 682)
                
-               326         600 LOAD_GLOBAL             41 (NULL + logger)
+               325         600 LOAD_GLOBAL             41 (NULL + logger)
                            612 LOAD_ATTR               21 (warning)
                            622 LOAD_FAST                0 (self)
                            624 LOAD_ATTR               22 (log_info)
                            634 FORMAT_VALUE             0
                            636 LOAD_CONST               7 (' | ')
                            638 LOAD_FAST                6 (balance)
                            640 LOAD_ATTR               19 (Wei)
@@ -2950,52 +2963,52 @@
                            656 FORMAT_VALUE             0
                            658 LOAD_CONST               9 (". Can't approve zero balance")
                            660 BUILD_STRING             6
                            662 PRECALL                  1
                            666 CALL                     1
                            676 POP_TOP
                
-               327         678 LOAD_CONST              10 (False)
+               326         678 LOAD_CONST              10 (False)
                            680 RETURN_VALUE
                
-               329     >>  682 LOAD_FAST                4 (amount)
+               328     >>  682 LOAD_FAST                4 (amount)
                            684 POP_JUMP_FORWARD_IF_FALSE    16 (to 718)
                            686 LOAD_FAST                4 (amount)
                            688 LOAD_ATTR               19 (Wei)
                            698 LOAD_FAST                6 (balance)
                            700 LOAD_ATTR               19 (Wei)
                            710 COMPARE_OP               4 (>)
                            716 POP_JUMP_FORWARD_IF_FALSE     2 (to 722)
                
-               330     >>  718 LOAD_FAST                6 (balance)
+               329     >>  718 LOAD_FAST                6 (balance)
                            720 STORE_FAST               4 (amount)
                
-               332     >>  722 LOAD_FAST                0 (self)
+               331     >>  722 LOAD_FAST                0 (self)
                            724 LOAD_METHOD             23 (get_allowance)
                            746 LOAD_FAST                2 (contract)
                            748 LOAD_FAST                1 (spender)
                            750 KW_NAMES                11
                            752 PRECALL                  2
                            756 CALL                     2
                            766 GET_AWAITABLE            0
                            768 LOAD_CONST               0 (None)
                        >>  770 SEND                     3 (to 778)
                            772 YIELD_VALUE
                            774 RESUME                   3
                            776 JUMP_BACKWARD_NO_INTERRUPT     4 (to 770)
                        >>  778 STORE_FAST               8 (approved)
                
-               334         780 LOAD_FAST                4 (amount)
+               333         780 LOAD_FAST                4 (amount)
                            782 LOAD_ATTR               19 (Wei)
                            792 LOAD_FAST                8 (approved)
                            794 LOAD_ATTR               19 (Wei)
                            804 COMPARE_OP               1 (<=)
                            810 POP_JUMP_FORWARD_IF_FALSE    40 (to 892)
                
-               335         812 LOAD_GLOBAL             41 (NULL + logger)
+               334         812 LOAD_GLOBAL             41 (NULL + logger)
                            824 LOAD_ATTR               24 (info)
                            834 LOAD_FAST                0 (self)
                            836 LOAD_ATTR               22 (log_info)
                            846 FORMAT_VALUE             0
                            848 LOAD_CONST              12 (' | Already approved ')
                            850 LOAD_FAST                8 (approved)
                            852 LOAD_ATTR               25 (Ether)
@@ -3004,107 +3017,107 @@
                            866 LOAD_FAST                7 (token_symbol)
                            868 FORMAT_VALUE             0
                            870 BUILD_STRING             5
                            872 PRECALL                  1
                            876 CALL                     1
                            886 POP_TOP
                
-               336         888 LOAD_CONST               1 (True)
+               335         888 LOAD_CONST               1 (True)
                            890 RETURN_VALUE
                
-               338     >>  892 LOAD_GLOBAL             23 (NULL + sleep)
+               337     >>  892 LOAD_GLOBAL             23 (NULL + sleep)
                
-               339         904 LOAD_FAST                0 (self)
+               338         904 LOAD_FAST                0 (self)
                            906 LOAD_ATTR               12 (delay_between_requests)
                
-               340         916 LOAD_FAST                0 (self)
+               339         916 LOAD_FAST                0 (self)
                            918 LOAD_ATTR               13 (profile)
                            928 POP_JUMP_FORWARD_IF_FALSE    12 (to 954)
                            930 LOAD_FAST                0 (self)
                            932 LOAD_ATTR               13 (profile)
                            942 LOAD_ATTR               14 (id)
                            952 JUMP_FORWARD             1 (to 956)
                        >>  954 LOAD_CONST               0 (None)
                
-               341     >>  956 LOAD_FAST                0 (self)
+               340     >>  956 LOAD_FAST                0 (self)
                            958 LOAD_ATTR               15 (sleep_echo)
                
-               338         968 KW_NAMES                 5
+               337         968 KW_NAMES                 5
                            970 PRECALL                  3
                            974 CALL                     3
                            984 GET_AWAITABLE            0
                            986 LOAD_CONST               0 (None)
                        >>  988 SEND                     3 (to 996)
                            990 YIELD_VALUE
                            992 RESUME                   3
                            994 JUMP_BACKWARD_NO_INTERRUPT     4 (to 988)
                        >>  996 POP_TOP
                
-               343         998 LOAD_FAST                0 (self)
+               342         998 LOAD_FAST                0 (self)
                           1000 LOAD_METHOD             26 (send_transaction)
                
-               344        1022 LOAD_FAST                3 (token_address)
+               343        1022 LOAD_FAST                3 (token_address)
                
-               345        1024 LOAD_FAST                2 (contract)
+               344        1024 LOAD_FAST                2 (contract)
                           1026 LOAD_METHOD             27 (encodeABI)
                           1048 LOAD_CONST              13 ('approve')
                
-               347        1050 LOAD_FAST                1 (spender)
+               346        1050 LOAD_FAST                1 (spender)
                
-               348        1052 LOAD_FAST                4 (amount)
+               347        1052 LOAD_FAST                4 (amount)
                           1054 LOAD_ATTR               19 (Wei)
                
-               346        1064 BUILD_TUPLE              2
+               345        1064 BUILD_TUPLE              2
                
-               345        1066 KW_NAMES                14
+               344        1066 KW_NAMES                14
                           1068 PRECALL                  2
                           1072 CALL                     2
                
-               343        1082 KW_NAMES                15
+               342        1082 KW_NAMES                15
                           1084 PRECALL                  2
                           1088 CALL                     2
                           1098 GET_AWAITABLE            0
                           1100 LOAD_CONST               0 (None)
                        >> 1102 SEND                     3 (to 1110)
                           1104 YIELD_VALUE
                           1106 RESUME                   3
                           1108 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1102)
                        >> 1110 UNPACK_SEQUENCE          2
                           1114 STORE_FAST               9 (ok)
                           1116 STORE_FAST              10 (tx_hash)
                
-               351        1118 LOAD_GLOBAL             23 (NULL + sleep)
+               350        1118 LOAD_GLOBAL             23 (NULL + sleep)
                
-               352        1130 LOAD_FAST                0 (self)
+               351        1130 LOAD_FAST                0 (self)
                           1132 LOAD_ATTR               12 (delay_between_requests)
                
-               353        1142 LOAD_FAST                0 (self)
+               352        1142 LOAD_FAST                0 (self)
                           1144 LOAD_ATTR               13 (profile)
                           1154 POP_JUMP_FORWARD_IF_FALSE    12 (to 1180)
                           1156 LOAD_FAST                0 (self)
                           1158 LOAD_ATTR               13 (profile)
                           1168 LOAD_ATTR               14 (id)
                           1178 JUMP_FORWARD             1 (to 1182)
                        >> 1180 LOAD_CONST               0 (None)
                
-               354     >> 1182 LOAD_FAST                0 (self)
+               353     >> 1182 LOAD_FAST                0 (self)
                           1184 LOAD_ATTR               15 (sleep_echo)
                
-               351        1194 KW_NAMES                 5
+               350        1194 KW_NAMES                 5
                           1196 PRECALL                  3
                           1200 CALL                     3
                           1210 GET_AWAITABLE            0
                           1212 LOAD_CONST               0 (None)
                        >> 1214 SEND                     3 (to 1222)
                           1216 YIELD_VALUE
                           1218 RESUME                   3
                           1220 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1214)
                        >> 1222 POP_TOP
                
-               356        1224 LOAD_FAST                0 (self)
+               355        1224 LOAD_FAST                0 (self)
                           1226 LOAD_METHOD             28 (verify_transaction)
                           1248 LOAD_FAST               10 (tx_hash)
                           1250 LOAD_CONST              16 ('Approve ')
                           1252 LOAD_FAST                7 (token_symbol)
                           1254 FORMAT_VALUE             0
                           1256 BUILD_STRING             2
                           1258 PRECALL                  2
@@ -3136,15 +3149,15 @@
                   'Approve '
                names      ('isinstance', 'int', 'TokenAmount', 'w3', 'eth', 'contract', 'AsyncWeb3', 'to_checksum_address', 'DefaultABIs', 'Token', 'balance_of', 'sleep', 'delay_between_requests', 'profile', 'id', 'sleep_echo', 'functions', 'symbol', 'call', 'Wei', 'logger', 'warning', 'log_info', 'get_allowance', 'info', 'Ether', 'send_transaction', 'encodeABI', 'verify_transaction')
                varnames   ('self', 'spender', 'contract', 'token_address', 'amount', 'abi', 'balance', 'token_symbol', 'approved', 'ok', 'tx_hash')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\client.py'
                name       'approve'
-               firstlineno 301
+               firstlineno 300
                lnotab
                   0x06042a01220104012c0126011afe120438010c010c0128010cfd1e0562
                   010c010c0128010cfd1e0616014e010402240104023a0220014c0104020c
                   010c0128010cfd1e05180102011a0202010cfe02ff10fe24080c010c0128
                   010cfd1e05
             code
                argcount  : 5
@@ -3165,102 +3178,102 @@
                   0064047c006a000000000000000000a00400000000000000000000000000
                   000000000000007c01a6010000ab0100000000000000007c026a08000000
                   00000000006702ac05a6020000ab020000000000000000ac06a6020000ab
                   020000000000000000830064007b03560097038604530074190000000000
                   00000000006a0d00000000000000007c006a0e00000000000000009b0064
                   077c056a0f00000000000000009b0064087c026a0f00000000000000009b
                   009d05a6010000ab010000000000000000010064095300
-               358           0 RETURN_GENERATOR
+               357           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               365           6 LOAD_FAST                3 (contract)
+               364           6 LOAD_FAST                3 (contract)
                              8 POP_JUMP_FORWARD_IF_TRUE    61 (to 132)
                
-               366          10 LOAD_FAST                0 (self)
+               365          10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (w3)
                             22 LOAD_ATTR                1 (eth)
                             32 LOAD_METHOD              2 (contract)
                
-               367          54 LOAD_GLOBAL              7 (NULL + AsyncWeb3)
+               366          54 LOAD_GLOBAL              7 (NULL + AsyncWeb3)
                             66 LOAD_ATTR                4 (to_checksum_address)
                             76 LOAD_FAST                4 (token_address)
                             78 PRECALL                  1
                             82 CALL                     1
                
-               368          92 LOAD_GLOBAL             10 (DefaultABIs)
+               367          92 LOAD_GLOBAL             10 (DefaultABIs)
                            104 LOAD_ATTR                6 (Token)
                
-               366         114 KW_NAMES                 1
+               365         114 KW_NAMES                 1
                            116 PRECALL                  2
                            120 CALL                     2
                            130 STORE_FAST               3 (contract)
                
-               370     >>  132 LOAD_FAST                0 (self)
+               369     >>  132 LOAD_FAST                0 (self)
                            134 LOAD_METHOD              7 (balance_of)
                            156 LOAD_FAST                3 (contract)
                            158 KW_NAMES                 2
                            160 PRECALL                  1
                            164 CALL                     1
                            174 GET_AWAITABLE            0
                            176 LOAD_CONST               0 (None)
                        >>  178 SEND                     3 (to 186)
                            180 YIELD_VALUE
                            182 RESUME                   3
                            184 JUMP_BACKWARD_NO_INTERRUPT     4 (to 178)
                        >>  186 STORE_FAST               5 (balance)
                
-               371         188 LOAD_FAST                5 (balance)
+               370         188 LOAD_FAST                5 (balance)
                            190 LOAD_ATTR                8 (Wei)
                            200 LOAD_FAST                2 (amount)
                            202 LOAD_ATTR                8 (Wei)
                            212 SWAP                     2
                            214 COPY                     2
                            216 COMPARE_OP               5 (>=)
                            222 POP_JUMP_FORWARD_IF_FALSE     6 (to 236)
                            224 LOAD_CONST               3 (0)
                            226 COMPARE_OP               4 (>)
                            232 POP_JUMP_FORWARD_IF_FALSE    89 (to 412)
                            234 JUMP_FORWARD             2 (to 240)
                        >>  236 POP_TOP
                            238 JUMP_FORWARD            86 (to 412)
                
-               372     >>  240 LOAD_FAST                0 (self)
+               371     >>  240 LOAD_FAST                0 (self)
                            242 LOAD_METHOD              9 (send_transaction)
                            264 LOAD_FAST                3 (contract)
                            266 LOAD_ATTR               10 (address)
                            276 LOAD_FAST                3 (contract)
                            278 LOAD_METHOD             11 (encodeABI)
                            300 LOAD_CONST               4 ('transfer')
                
-               373         302 LOAD_FAST                0 (self)
+               372         302 LOAD_FAST                0 (self)
                            304 LOAD_ATTR                0 (w3)
                            314 LOAD_METHOD              4 (to_checksum_address)
                            336 LOAD_FAST                1 (to)
                            338 PRECALL                  1
                            342 CALL                     1
                            352 LOAD_FAST                2 (amount)
                            354 LOAD_ATTR                8 (Wei)
                
-               372         364 BUILD_LIST               2
+               371         364 BUILD_LIST               2
                            366 KW_NAMES                 5
                            368 PRECALL                  2
                            372 CALL                     2
                            382 KW_NAMES                 6
                            384 PRECALL                  2
                            388 CALL                     2
                            398 GET_AWAITABLE            0
                            400 LOAD_CONST               0 (None)
                        >>  402 SEND                     3 (to 410)
                            404 YIELD_VALUE
                            406 RESUME                   3
                            408 JUMP_BACKWARD_NO_INTERRUPT     4 (to 402)
                        >>  410 RETURN_VALUE
                
-               376     >>  412 LOAD_GLOBAL             25 (NULL + logger)
+               375     >>  412 LOAD_GLOBAL             25 (NULL + logger)
                            424 LOAD_ATTR               13 (warning)
                            434 LOAD_FAST                0 (self)
                            436 LOAD_ATTR               14 (log_info)
                            446 FORMAT_VALUE             0
                            448 LOAD_CONST               7 (' | Amount is too high. Balance - ')
                            450 LOAD_FAST                5 (balance)
                            452 LOAD_ATTR               15 (Ether)
@@ -3270,15 +3283,15 @@
                            468 LOAD_ATTR               15 (Ether)
                            478 FORMAT_VALUE             0
                            480 BUILD_STRING             5
                            482 PRECALL                  1
                            486 CALL                     1
                            496 POP_TOP
                
-               377         498 LOAD_CONST               9 ((False, ''))
+               376         498 LOAD_CONST               9 ((False, ''))
                            500 RETURN_VALUE
                consts
                   None
                   ('address', 'abi')
                   ('contract',)
                   0
                   'transfer'
@@ -3289,15 +3302,15 @@
                   (False, '')
                names      ('w3', 'eth', 'contract', 'AsyncWeb3', 'to_checksum_address', 'DefaultABIs', 'Token', 'balance_of', 'Wei', 'send_transaction', 'address', 'encodeABI', 'logger', 'warning', 'log_info', 'Ether')
                varnames   ('self', 'to', 'amount', 'contract', 'token_address', 'balance')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\client.py'
                name       'transfer_token'
-               firstlineno 358
+               firstlineno 357
                lnotab 0x060704012c01260116fe1204380134013e013eff30045601
             'ETH'
             code
                argcount  : 2
                nlocals   : 5
                stacksize : 7
                flags     : 131
@@ -3306,45 +3319,45 @@
                   00a6000000ab0000000000000000007d027403000000000000000000007c
                   006a0200000000000000007c006a0300000000000000007c006a04000000
                   000000000064016402ac03a6050000ab0500000000000000007d03740b00
                   0000000000000000007c03a0060000000000000000000000000000000000
                   0000007c029b0064049d02a6010000ab0100000000000000006405190000
                   000000000000006406190000000000000000006407190000000000000000
                   00a6010000ab0100000000000000007d047c045300
-               379           0 RETURN_GENERATOR
+               378           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               380           6 LOAD_FAST                1 (token)
+               379           6 LOAD_FAST                1 (token)
                              8 LOAD_METHOD              0 (upper)
                             30 PRECALL                  0
                             34 CALL                     0
                             44 STORE_FAST               2 (ticker)
                
-               381          46 LOAD_GLOBAL              3 (NULL + MarketAPI)
+               380          46 LOAD_GLOBAL              3 (NULL + MarketAPI)
                
-               382          58 LOAD_FAST                0 (self)
+               381          58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                2 (okx_api_key)
                
-               383          70 LOAD_FAST                0 (self)
+               382          70 LOAD_FAST                0 (self)
                             72 LOAD_ATTR                3 (okx_api_secret)
                
-               384          82 LOAD_FAST                0 (self)
+               383          82 LOAD_FAST                0 (self)
                             84 LOAD_ATTR                4 (okx_passphrase)
                
-               385          94 LOAD_CONST               1 ('0')
+               384          94 LOAD_CONST               1 ('0')
                
-               386          96 LOAD_CONST               2 (False)
+               385          96 LOAD_CONST               2 (False)
                
-               381          98 KW_NAMES                 3
+               380          98 KW_NAMES                 3
                            100 PRECALL                  5
                            104 CALL                     5
                            114 STORE_FAST               3 (okx_market)
                
-               388         116 LOAD_GLOBAL             11 (NULL + float)
+               387         116 LOAD_GLOBAL             11 (NULL + float)
                            128 LOAD_FAST                3 (okx_market)
                            130 LOAD_METHOD              6 (get_ticker)
                            152 LOAD_FAST                2 (ticker)
                            154 FORMAT_VALUE             0
                            156 LOAD_CONST               4 ('-USDT')
                            158 BUILD_STRING             2
                            160 PRECALL                  1
@@ -3355,15 +3368,15 @@
                            188 BINARY_SUBSCR
                            198 LOAD_CONST               7 ('askPx')
                            200 BINARY_SUBSCR
                            210 PRECALL                  1
                            214 CALL                     1
                            224 STORE_FAST               4 (price)
                
-               389         226 LOAD_FAST                4 (price)
+               388         226 LOAD_FAST                4 (price)
                            228 RETURN_VALUE
                consts
                   None
                   '0'
                   False
                   ('api_key', 'api_secret_key', 'passphrase', 'flag', 'debug')
                   '-USDT'
@@ -3372,46 +3385,46 @@
                   'askPx'
                names      ('upper', 'MarketAPI', 'okx_api_key', 'okx_api_secret', 'okx_passphrase', 'float', 'get_ticker')
                varnames   ('self', 'token', 'ticker', 'okx_market', 'price')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\client.py'
                name       'get_token_price'
-               firstlineno 379
+               firstlineno 378
                lnotab 0x060128010c010c010c010c01020102fb12076e01
             'get_usd_price'
             code
                argcount  : 4
                nlocals   : 5
                stacksize : 12
                flags     : 131
                code
                   0x4b00010097007401000000000000000000007c006a0100000000000000
                   006a020000000000000000a0030000000000000000000000000000000000
                   0000007c01700b7c006a0400000000000000006a050000000000000000a6
                   010000ab010000000000000000830064007b035600970386046401ac02a6
-                  020000ab0200000000000000007d04740c000000000000000000006a0700
-                  0000000000000070257c00a0080000000000000000000000000000000000
-                  0000007c006a0900000000000000006a0a0000000000000000ac03a60100
-                  00ab010000000000000000830064007b03560097038604740c0000000000
-                  00000000005f0700000000000000007c0272677417000000000000000000
-                  006a0c00000000000000007c006a0d00000000000000009b006404741d00
-                  0000000000000000007c046a0f0000000000000000a6010000ab01000000
-                  00000000009b0064057c006a0900000000000000006a0a00000000000000
-                  009b007c0372266405740c000000000000000000006a0700000000000000
-                  00741d000000000000000000007c046a0f0000000000000000a6010000ab
-                  0100000000000000007a05000064069b0464079d036e0164089b009d06a6
-                  010000ab01000000000000000001007c045300
-               391           0 RETURN_GENERATOR
+                  020000ab0200000000000000007d047c03723c740c000000000000000000
+                  006a07000000000000000070257c00a00800000000000000000000000000
+                  000000000000007c006a0900000000000000006a0a0000000000000000ac
+                  03a6010000ab010000000000000000830064007b03560097038604740c00
+                  0000000000000000005f0700000000000000007c02726774170000000000
+                  00000000006a0c00000000000000007c006a0d00000000000000009b0064
+                  04741d000000000000000000007c046a0f0000000000000000a6010000ab
+                  0100000000000000009b0064057c006a0900000000000000006a0a000000
+                  00000000009b007c0372266405740c000000000000000000006a07000000
+                  0000000000741d000000000000000000007c046a0f0000000000000000a6
+                  010000ab0100000000000000007a05000064069b0464079d036e0164089b
+                  009d06a6010000ab01000000000000000001007c045300
+               390           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               397           6 LOAD_GLOBAL              1 (NULL + TokenAmount)
+               396           6 LOAD_GLOBAL              1 (NULL + TokenAmount)
                
-               398          18 LOAD_FAST                0 (self)
+               397          18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (w3)
                             30 LOAD_ATTR                2 (eth)
                             40 LOAD_METHOD              3 (get_balance)
                             62 LOAD_FAST                1 (address)
                             64 JUMP_IF_TRUE_OR_POP     11 (to 88)
                             66 LOAD_FAST                0 (self)
                             68 LOAD_ATTR                4 (account)
@@ -3421,90 +3434,93 @@
                            102 GET_AWAITABLE            0
                            104 LOAD_CONST               0 (None)
                        >>  106 SEND                     3 (to 114)
                            108 YIELD_VALUE
                            110 RESUME                   3
                            112 JUMP_BACKWARD_NO_INTERRUPT     4 (to 106)
                
-               399     >>  114 LOAD_CONST               1 (True)
+               398     >>  114 LOAD_CONST               1 (True)
                
-               397         116 KW_NAMES                 2
+               396         116 KW_NAMES                 2
                            118 PRECALL                  2
                            122 CALL                     2
                            132 STORE_FAST               4 (balance)
                
-               401         134 LOAD_GLOBAL             12 (Client)
-                           146 LOAD_ATTR                7 (NATIVE_PRICE)
-                           156 JUMP_IF_TRUE_OR_POP     37 (to 232)
-                           158 LOAD_FAST                0 (self)
-                           160 LOAD_METHOD              8 (get_token_price)
-                           182 LOAD_FAST                0 (self)
-                           184 LOAD_ATTR                9 (network)
-                           194 LOAD_ATTR               10 (coin_symbol)
-                           204 KW_NAMES                 3
-                           206 PRECALL                  1
-                           210 CALL                     1
-                           220 GET_AWAITABLE            0
-                           222 LOAD_CONST               0 (None)
-                       >>  224 SEND                     3 (to 232)
-                           226 YIELD_VALUE
-                           228 RESUME                   3
-                           230 JUMP_BACKWARD_NO_INTERRUPT     4 (to 224)
-                       >>  232 LOAD_GLOBAL             12 (Client)
-                           244 STORE_ATTR               7 (NATIVE_PRICE)
-               
-               402         254 LOAD_FAST                2 (echo)
-                           256 POP_JUMP_FORWARD_IF_FALSE   103 (to 464)
-               
-               403         258 LOAD_GLOBAL             23 (NULL + logger)
-                           270 LOAD_ATTR               12 (info)
-               
-               404         280 LOAD_FAST                0 (self)
-                           282 LOAD_ATTR               13 (log_info)
-                           292 FORMAT_VALUE             0
-                           294 LOAD_CONST               4 (' | Balance - ')
-                           296 LOAD_GLOBAL             29 (NULL + float)
-                           308 LOAD_FAST                4 (balance)
-                           310 LOAD_ATTR               15 (Ether)
-                           320 PRECALL                  1
-                           324 CALL                     1
-                           334 FORMAT_VALUE             0
-                           336 LOAD_CONST               5 (' ')
-                           338 LOAD_FAST                0 (self)
-                           340 LOAD_ATTR                9 (network)
-                           350 LOAD_ATTR               10 (coin_symbol)
-                           360 FORMAT_VALUE             0
-               
-               405         362 LOAD_FAST                3 (get_usd_price)
-                           364 POP_JUMP_FORWARD_IF_FALSE    38 (to 442)
-                           366 LOAD_CONST               5 (' ')
-                           368 LOAD_GLOBAL             12 (Client)
-                           380 LOAD_ATTR                7 (NATIVE_PRICE)
-                           390 LOAD_GLOBAL             29 (NULL + float)
-                           402 LOAD_FAST                4 (balance)
-                           404 LOAD_ATTR               15 (Ether)
-                           414 PRECALL                  1
-                           418 CALL                     1
-                           428 BINARY_OP                5 (*)
-                           432 LOAD_CONST               6 ('2f')
-                           434 FORMAT_VALUE             4 (with format)
-                           436 LOAD_CONST               7 ('$')
-                           438 BUILD_STRING             3
-                           440 JUMP_FORWARD             1 (to 444)
-                       >>  442 LOAD_CONST               8 ('')
-               
-               404     >>  444 FORMAT_VALUE             0
-                           446 BUILD_STRING             6
-               
-               403         448 PRECALL                  1
-                           452 CALL                     1
-                           462 POP_TOP
+               400         134 LOAD_FAST                3 (get_usd_price)
+                           136 POP_JUMP_FORWARD_IF_FALSE    60 (to 258)
+               
+               401         138 LOAD_GLOBAL             12 (Client)
+                           150 LOAD_ATTR                7 (NATIVE_PRICE)
+                           160 JUMP_IF_TRUE_OR_POP     37 (to 236)
+                           162 LOAD_FAST                0 (self)
+                           164 LOAD_METHOD              8 (get_token_price)
+                           186 LOAD_FAST                0 (self)
+                           188 LOAD_ATTR                9 (network)
+                           198 LOAD_ATTR               10 (coin_symbol)
+                           208 KW_NAMES                 3
+                           210 PRECALL                  1
+                           214 CALL                     1
+                           224 GET_AWAITABLE            0
+                           226 LOAD_CONST               0 (None)
+                       >>  228 SEND                     3 (to 236)
+                           230 YIELD_VALUE
+                           232 RESUME                   3
+                           234 JUMP_BACKWARD_NO_INTERRUPT     4 (to 228)
+                       >>  236 LOAD_GLOBAL             12 (Client)
+                           248 STORE_ATTR               7 (NATIVE_PRICE)
+               
+               402     >>  258 LOAD_FAST                2 (echo)
+                           260 POP_JUMP_FORWARD_IF_FALSE   103 (to 468)
+               
+               403         262 LOAD_GLOBAL             23 (NULL + logger)
+                           274 LOAD_ATTR               12 (info)
+               
+               404         284 LOAD_FAST                0 (self)
+                           286 LOAD_ATTR               13 (log_info)
+                           296 FORMAT_VALUE             0
+                           298 LOAD_CONST               4 (' | Balance - ')
+                           300 LOAD_GLOBAL             29 (NULL + float)
+                           312 LOAD_FAST                4 (balance)
+                           314 LOAD_ATTR               15 (Ether)
+                           324 PRECALL                  1
+                           328 CALL                     1
+                           338 FORMAT_VALUE             0
+                           340 LOAD_CONST               5 (' ')
+                           342 LOAD_FAST                0 (self)
+                           344 LOAD_ATTR                9 (network)
+                           354 LOAD_ATTR               10 (coin_symbol)
+                           364 FORMAT_VALUE             0
+               
+               405         366 LOAD_FAST                3 (get_usd_price)
+                           368 POP_JUMP_FORWARD_IF_FALSE    38 (to 446)
+                           370 LOAD_CONST               5 (' ')
+                           372 LOAD_GLOBAL             12 (Client)
+                           384 LOAD_ATTR                7 (NATIVE_PRICE)
+                           394 LOAD_GLOBAL             29 (NULL + float)
+                           406 LOAD_FAST                4 (balance)
+                           408 LOAD_ATTR               15 (Ether)
+                           418 PRECALL                  1
+                           422 CALL                     1
+                           432 BINARY_OP                5 (*)
+                           436 LOAD_CONST               6 ('2f')
+                           438 FORMAT_VALUE             4 (with format)
+                           440 LOAD_CONST               7 ('$')
+                           442 BUILD_STRING             3
+                           444 JUMP_FORWARD             1 (to 448)
+                       >>  446 LOAD_CONST               8 ('')
+               
+               404     >>  448 FORMAT_VALUE             0
+                           450 BUILD_STRING             6
+               
+               403         452 PRECALL                  1
+                           456 CALL                     1
+                           466 POP_TOP
                
-               407     >>  464 LOAD_FAST                4 (balance)
-                           466 RETURN_VALUE
+               407     >>  468 LOAD_FAST                4 (balance)
+                           470 RETURN_VALUE
                consts
                   None
                   True
                   ('amount', 'wei')
                   ('token',)
                   ' | Balance - '
                   ' '
@@ -3513,16 +3529,16 @@
                   ''
                names      ('TokenAmount', 'w3', 'eth', 'get_balance', 'account', 'address', 'Client', 'NATIVE_PRICE', 'get_token_price', 'network', 'coin_symbol', 'logger', 'info', 'log_info', 'float', 'Ether')
                varnames   ('self', 'address', 'echo', 'get_usd_price', 'balance')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\client.py'
                name       'get_native_balance'
-               firstlineno 391
-               lnotab 0x06060c01600102fe1204780104011601520152ff04ff1004
+               firstlineno 390
+               lnotab 0x06060c01600102fe12040401780104011601520152ff04ff1004
             (None, None)
             (None, None, None, False)
             (None, None, None, None, None, None)
             (None, None, None, None)
             ('ETH',)
             (None, False, False)
          names      ('__name__', '__module__', '__qualname__', 'NATIVE_PRICE', 'INCREASE_GWEI', 'INCREASE_GAS_LIMIT', 'Ethereum', 'Chain', 'Profile', 'Account', 'str', 'int', 'bool', '__init__', '__aenter__', '__aexit__', 'sign', 'nonce', 'AsyncContract', 'get_decimals', 'Optional', 'TokenAmount', 'balance_of', 'get_allowance', 'staticmethod', 'AsyncWeb3', 'dict', 'get_max_priority_fee_per_gas', 'tuple', 'Exception', 'HexBytes', 'send_transaction', 'verify_transaction', 'tx', 'approve', 'transfer_token', 'float', 'get_token_price', 'get_native_balance')
@@ -3531,15 +3547,15 @@
          cellvars   ()
          filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\client.py'
          name       'Client'
          firstlineno 21
          lnotab
             0x0a01040104010404020102010201020102010201020102010201020102
             f4040202fe020302fd020402fc020502fb020602fa020702f9020802f802
-            0902f7020a02f6020b02f5020c02f40824060306030c060c03160c020102
+            0902f7020a02f6020b02f5020c02f40823060306030c060c03160c020102
             fe040102ff020102ff02020efe020202fe020302fd0816020102fe040102
             ff020102ff020202fe020302fd0814020112ff0e01021602010201020102
             01020102f804070ef902080ef802091ef7085d1418020114010201020102
             0102f7040202fe020302fd020402fc020508fb02060efa02070ef902080e
             f8020902f7020a02f60828020102fe040102ff020102ff020102ff020208
             fe020202fe020302fd083d020102fb040202fe020302fd020402fc020502
             fb02061efa08150e0e0201020102fc040202fe020302fd020402fc020502
```

### Comparing `web3mt-0.0.1/web3mt/evm/__pycache__/models.cpython-311.pyc` & `web3mt-0.0.2/web3mt/evm/__pycache__/models.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,38 +1,39 @@
 magic:    0xa70d0d0a
-moddate:  0x25451966 (Fri Apr 12 14:28:53 2024 UTC)
-files sz: 6819
+moddate:  0x00242966 (Wed Apr 24 15:23:44 2024 UTC)
+files sz: 7041
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 9
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
       036c046d055a050100650102004700640484006405a6020000ab02000000
       0000000000a6000000ab0000000000000000005a06020047006406840064
       07a6020000ab0200000000000000005a0702004700640884006409a60200
       00ab0200000000000000005a0802006508640a640b640c640d640e640f64
       10ac11a6070000ab0700000000000000005a090200650864126413641464
       0d640e6415ac16a6060000ab0600000000000000005a0a02006508641764
       186419640d640e641aac16a6060000ab0600000000000000005a0b020065
-      08641b641c641d640d641e641fac16a6060000ab0600000000000000005a
-      0c02006508642064216422640d641e6423ac16a6060000ab060000000000
-      0000005a0d02006508642464256426640d64276428ac16a6060000ab0600
-      000000000000005a0e020065086429642a642b640d642c642dac16a60600
-      00ab0600000000000000005a0f02006508642e642f6430640d64316432ac
-      16a6060000ab0600000000000000005a1002006508643164336434640d64
-      316432ac16a6060000ab0600000000000000005a11020065086435643664
-      37640d640e6438ac16a6060000ab0600000000000000005a120200650864
+      08641b641c641d640d640e641eac16a6060000ab0600000000000000005a
+      0c02006508641f64206421640d64226423ac16a6060000ab060000000000
+      0000005a0d02006508642464256426640d64226427ac16a6060000ab0600
+      000000000000005a0e0200650864286429642a640d642b642cac16a60600
+      00ab0600000000000000005a0f02006508642d642e642f640d64306431ac
+      16a6060000ab0600000000000000005a1002006508643264336434640d64
+      356436ac16a6060000ab0600000000000000005a11020065086435643764
+      38640d64356436ac16a6060000ab0600000000000000005a120200650864
       39643a643b640d640e643cac16a6060000ab0600000000000000005a1302
-      006508643d643e643f640d64406441ac16a6060000ab0600000000000000
-      005a1402006508644264436444640d640e6445ac16a6060000ab06000000
+      006508643d643e643f640d640e6440ac16a6060000ab0600000000000000
+      005a1402006508644164426443640d64446445ac16a6060000ab06000000
       00000000005a1502006508644664476448640d640e6449ac16a6060000ab
       0600000000000000005a1602006508644a644b644c640d640e644dac16a6
-      060000ab0600000000000000005a17644e5300
+      060000ab0600000000000000005a1702006508644e644f6450640d640e64
+      51ac16a6060000ab0600000000000000005a1864525300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('dataclass',))
                  6 IMPORT_NAME              0 (dataclasses)
                  8 IMPORT_FROM              1 (dataclass)
                 10 STORE_NAME               1 (dataclass)
@@ -52,37 +53,37 @@
                 34 STORE_NAME               5 (Union)
                 36 POP_TOP
    
      6          38 LOAD_NAME                1 (dataclass)
    
      7          40 PUSH_NULL
                 42 LOAD_BUILD_CLASS
-                44 LOAD_CONST               4 (<code object DefaultABIs, file "C:\Users\timer\Code\crypto_multitool\evm\models.py", line 6>)
+                44 LOAD_CONST               4 (<code object DefaultABIs, file "C:\Users\timer\Code\web3mt\web3mt\evm\models.py", line 6>)
                 46 MAKE_FUNCTION            0
                 48 LOAD_CONST               5 ('DefaultABIs')
                 50 PRECALL                  2
                 54 CALL                     2
    
      6          64 PRECALL                  0
                 68 CALL                     0
    
      7          78 STORE_NAME               6 (DefaultABIs)
    
     85          80 PUSH_NULL
                 82 LOAD_BUILD_CLASS
-                84 LOAD_CONST               6 (<code object TokenAmount, file "C:\Users\timer\Code\crypto_multitool\evm\models.py", line 85>)
+                84 LOAD_CONST               6 (<code object TokenAmount, file "C:\Users\timer\Code\web3mt\web3mt\evm\models.py", line 85>)
                 86 MAKE_FUNCTION            0
                 88 LOAD_CONST               7 ('TokenAmount')
                 90 PRECALL                  2
                 94 CALL                     2
                104 STORE_NAME               7 (TokenAmount)
    
    111         106 PUSH_NULL
                108 LOAD_BUILD_CLASS
-               110 LOAD_CONST               8 (<code object Chain, file "C:\Users\timer\Code\crypto_multitool\evm\models.py", line 111>)
+               110 LOAD_CONST               8 (<code object Chain, file "C:\Users\timer\Code\web3mt\web3mt\evm\models.py", line 111>)
                112 MAKE_FUNCTION            0
                114 LOAD_CONST               9 ('Chain')
                116 PRECALL                  2
                120 CALL                     2
                130 STORE_NAME               8 (Chain)
    
    136         132 PUSH_NULL
@@ -143,255 +144,275 @@
    161         216 LOAD_CONST              26 ('https://optimistic.etherscan.io/')
    
    155         218 KW_NAMES                22
                220 PRECALL                  6
                224 CALL                     6
                234 STORE_NAME              11 (Optimism)
    
-   164         236 PUSH_NULL
+   163         236 PUSH_NULL
                238 LOAD_NAME                8 (Chain)
    
-   165         240 LOAD_CONST              27 ('Polygon')
+   164         240 LOAD_CONST              27 ('Optimism Sepolia')
    
-   166         242 LOAD_CONST              28 ('https://polygon-rpc.com/')
+   165         242 LOAD_CONST              28 ('https://sepolia.optimism.io')
    
-   167         244 LOAD_CONST              29 (137)
+   166         244 LOAD_CONST              29 (11155420)
    
-   168         246 LOAD_CONST              13 (True)
+   167         246 LOAD_CONST              13 (True)
    
-   169         248 LOAD_CONST              30 ('MATIC')
+   168         248 LOAD_CONST              14 ('ETH')
    
-   170         250 LOAD_CONST              31 ('https://polygonscan.com/')
+   169         250 LOAD_CONST              30 ('https://optimism-sepolia.blockscout.com/')
    
-   164         252 KW_NAMES                22
+   163         252 KW_NAMES                22
                254 PRECALL                  6
                258 CALL                     6
-               268 STORE_NAME              12 (Polygon)
+               268 STORE_NAME              12 (OP_Sepolia)
    
    172         270 PUSH_NULL
                272 LOAD_NAME                8 (Chain)
    
-   173         274 LOAD_CONST              32 ('Mumbai')
+   173         274 LOAD_CONST              31 ('Polygon')
    
-   174         276 LOAD_CONST              33 ('https://polygon-mumbai-bor-rpc.publicnode.com')
+   174         276 LOAD_CONST              32 ('https://polygon-rpc.com/')
    
-   175         278 LOAD_CONST              34 (80001)
+   175         278 LOAD_CONST              33 (137)
    
    176         280 LOAD_CONST              13 (True)
    
-   177         282 LOAD_CONST              30 ('MATIC')
+   177         282 LOAD_CONST              34 ('MATIC')
    
-   178         284 LOAD_CONST              35 ('https://mumbai.polygonscan.com/')
+   178         284 LOAD_CONST              35 ('https://polygonscan.com/')
    
    172         286 KW_NAMES                22
                288 PRECALL                  6
                292 CALL                     6
-               302 STORE_NAME              13 (Mumbai)
+               302 STORE_NAME              13 (Polygon)
    
-   181         304 PUSH_NULL
+   180         304 PUSH_NULL
                306 LOAD_NAME                8 (Chain)
    
-   182         308 LOAD_CONST              36 ('Avalanche')
+   181         308 LOAD_CONST              36 ('Mumbai')
    
-   183         310 LOAD_CONST              37 ('https://rpc.ankr.com/avalanche/')
+   182         310 LOAD_CONST              37 ('https://polygon-mumbai-bor-rpc.publicnode.com')
    
-   184         312 LOAD_CONST              38 (43114)
+   183         312 LOAD_CONST              38 (80001)
    
-   185         314 LOAD_CONST              13 (True)
+   184         314 LOAD_CONST              13 (True)
    
-   186         316 LOAD_CONST              39 ('AVAX')
+   185         316 LOAD_CONST              34 ('MATIC')
    
-   187         318 LOAD_CONST              40 ('https://snowtrace.io/')
+   186         318 LOAD_CONST              39 ('https://mumbai.polygonscan.com/')
    
-   181         320 KW_NAMES                22
+   180         320 KW_NAMES                22
                322 PRECALL                  6
                326 CALL                     6
-               336 STORE_NAME              14 (Avalanche)
+               336 STORE_NAME              14 (Mumbai)
    
-   190         338 PUSH_NULL
+   189         338 PUSH_NULL
                340 LOAD_NAME                8 (Chain)
    
-   191         342 LOAD_CONST              41 ('Fantom')
+   190         342 LOAD_CONST              40 ('Avalanche')
    
-   192         344 LOAD_CONST              42 ('https://rpc.ankr.com/fantom/')
+   191         344 LOAD_CONST              41 ('https://rpc.ankr.com/avalanche/')
    
-   193         346 LOAD_CONST              43 (250)
+   192         346 LOAD_CONST              42 (43114)
    
-   194         348 LOAD_CONST              13 (True)
+   193         348 LOAD_CONST              13 (True)
    
-   195         350 LOAD_CONST              44 ('FTM')
+   194         350 LOAD_CONST              43 ('AVAX')
    
-   196         352 LOAD_CONST              45 ('https://ftmscan.com/')
+   195         352 LOAD_CONST              44 ('https://snowtrace.io/')
    
-   190         354 KW_NAMES                22
+   189         354 KW_NAMES                22
                356 PRECALL                  6
                360 CALL                     6
-               370 STORE_NAME              15 (Fantom)
+               370 STORE_NAME              15 (Avalanche)
    
-   199         372 PUSH_NULL
+   198         372 PUSH_NULL
                374 LOAD_NAME                8 (Chain)
    
-   200         376 LOAD_CONST              46 ('opBNB')
+   199         376 LOAD_CONST              45 ('Fantom')
    
-   201         378 LOAD_CONST              47 ('https://opbnb.publicnode.com')
+   200         378 LOAD_CONST              46 ('https://rpc.ankr.com/fantom/')
    
-   202         380 LOAD_CONST              48 (204)
+   201         380 LOAD_CONST              47 (250)
    
-   203         382 LOAD_CONST              13 (True)
+   202         382 LOAD_CONST              13 (True)
    
-   204         384 LOAD_CONST              49 ('BNB')
+   203         384 LOAD_CONST              48 ('FTM')
    
-   205         386 LOAD_CONST              50 ('https://bscscan.com/')
+   204         386 LOAD_CONST              49 ('https://ftmscan.com/')
    
-   199         388 KW_NAMES                22
+   198         388 KW_NAMES                22
                390 PRECALL                  6
                394 CALL                     6
-               404 STORE_NAME              16 (opBNB)
+               404 STORE_NAME              16 (Fantom)
    
-   208         406 PUSH_NULL
+   207         406 PUSH_NULL
                408 LOAD_NAME                8 (Chain)
    
-   209         410 LOAD_CONST              49 ('BNB')
+   208         410 LOAD_CONST              50 ('opBNB')
    
-   210         412 LOAD_CONST              51 ('https://bsc.meowrpc.com')
+   209         412 LOAD_CONST              51 ('https://opbnb.publicnode.com')
    
-   211         414 LOAD_CONST              52 (56)
+   210         414 LOAD_CONST              52 (204)
    
-   212         416 LOAD_CONST              13 (True)
+   211         416 LOAD_CONST              13 (True)
    
-   213         418 LOAD_CONST              49 ('BNB')
+   212         418 LOAD_CONST              53 ('BNB')
    
-   214         420 LOAD_CONST              50 ('https://bscscan.com/')
+   213         420 LOAD_CONST              54 ('https://bscscan.com/')
    
-   208         422 KW_NAMES                22
+   207         422 KW_NAMES                22
                424 PRECALL                  6
                428 CALL                     6
-               438 STORE_NAME              17 (BNB)
+               438 STORE_NAME              17 (opBNB)
    
-   217         440 PUSH_NULL
+   216         440 PUSH_NULL
                442 LOAD_NAME                8 (Chain)
    
-   218         444 LOAD_CONST              53 ('Linea')
+   217         444 LOAD_CONST              53 ('BNB')
    
-   219         446 LOAD_CONST              54 ('https://rpc.linea.build')
+   218         446 LOAD_CONST              55 ('https://bsc.meowrpc.com')
    
-   220         448 LOAD_CONST              55 (59144)
+   219         448 LOAD_CONST              56 (56)
    
-   221         450 LOAD_CONST              13 (True)
+   220         450 LOAD_CONST              13 (True)
    
-   222         452 LOAD_CONST              14 ('ETH')
+   221         452 LOAD_CONST              53 ('BNB')
    
-   223         454 LOAD_CONST              56 ('https://lineascan.build/')
+   222         454 LOAD_CONST              54 ('https://bscscan.com/')
    
-   217         456 KW_NAMES                22
+   216         456 KW_NAMES                22
                458 PRECALL                  6
                462 CALL                     6
-               472 STORE_NAME              18 (Linea)
+               472 STORE_NAME              18 (BNB)
    
-   226         474 PUSH_NULL
+   225         474 PUSH_NULL
                476 LOAD_NAME                8 (Chain)
    
-   227         478 LOAD_CONST              57 ('zkSync')
+   226         478 LOAD_CONST              57 ('Linea')
    
-   228         480 LOAD_CONST              58 ('https://mainnet.era.zksync.io')
+   227         480 LOAD_CONST              58 ('https://rpc.linea.build')
    
-   229         482 LOAD_CONST              59 (324)
+   228         482 LOAD_CONST              59 (59144)
    
-   230         484 LOAD_CONST              13 (True)
+   229         484 LOAD_CONST              13 (True)
    
-   231         486 LOAD_CONST              14 ('ETH')
+   230         486 LOAD_CONST              14 ('ETH')
    
-   232         488 LOAD_CONST              60 ('https://explorer.zksync.io/')
+   231         488 LOAD_CONST              60 ('https://lineascan.build/')
    
-   226         490 KW_NAMES                22
+   225         490 KW_NAMES                22
                492 PRECALL                  6
                496 CALL                     6
-               506 STORE_NAME              19 (zkSync)
+               506 STORE_NAME              19 (Linea)
    
-   235         508 PUSH_NULL
+   234         508 PUSH_NULL
                510 LOAD_NAME                8 (Chain)
    
-   236         512 LOAD_CONST              61 ('Zetachain')
+   235         512 LOAD_CONST              61 ('zkSync')
    
-   237         514 LOAD_CONST              62 ('https://zetachain-evm.blockpi.network/v1/rpc/public')
+   236         514 LOAD_CONST              62 ('https://mainnet.era.zksync.io')
    
-   238         516 LOAD_CONST              63 (7000)
+   237         516 LOAD_CONST              63 (324)
    
-   239         518 LOAD_CONST              13 (True)
+   238         518 LOAD_CONST              13 (True)
    
-   240         520 LOAD_CONST              64 ('ZETA')
+   239         520 LOAD_CONST              14 ('ETH')
    
-   241         522 LOAD_CONST              65 ('https://explorer.zetachain.com/')
+   240         522 LOAD_CONST              64 ('https://explorer.zksync.io/')
    
-   235         524 KW_NAMES                22
+   234         524 KW_NAMES                22
                526 PRECALL                  6
                530 CALL                     6
-               540 STORE_NAME              20 (ZetaChain)
+               540 STORE_NAME              20 (zkSync)
    
-   244         542 PUSH_NULL
+   243         542 PUSH_NULL
                544 LOAD_NAME                8 (Chain)
    
-   245         546 LOAD_CONST              66 ('Scroll')
+   244         546 LOAD_CONST              65 ('Zetachain')
    
-   246         548 LOAD_CONST              67 ('https://scroll.drpc.org')
+   245         548 LOAD_CONST              66 ('https://zetachain-evm.blockpi.network/v1/rpc/public')
    
-   247         550 LOAD_CONST              68 (534352)
+   246         550 LOAD_CONST              67 (7000)
    
-   248         552 LOAD_CONST              13 (True)
+   247         552 LOAD_CONST              13 (True)
    
-   249         554 LOAD_CONST              14 ('ETH')
+   248         554 LOAD_CONST              68 ('ZETA')
    
-   250         556 LOAD_CONST              69 ('https://scrollscan.com/')
+   249         556 LOAD_CONST              69 ('https://explorer.zetachain.com/')
    
-   244         558 KW_NAMES                22
+   243         558 KW_NAMES                22
                560 PRECALL                  6
                564 CALL                     6
-               574 STORE_NAME              21 (Scroll)
+               574 STORE_NAME              21 (ZetaChain)
    
-   253         576 PUSH_NULL
+   252         576 PUSH_NULL
                578 LOAD_NAME                8 (Chain)
    
-   254         580 LOAD_CONST              70 ('Zora')
+   253         580 LOAD_CONST              70 ('Scroll')
    
-   255         582 LOAD_CONST              71 ('https://rpc.zora.energy')
+   254         582 LOAD_CONST              71 ('https://scroll.drpc.org')
    
-   256         584 LOAD_CONST              72 (7777777)
+   255         584 LOAD_CONST              72 (534352)
    
-   257         586 LOAD_CONST              13 (True)
+   256         586 LOAD_CONST              13 (True)
    
-   258         588 LOAD_CONST              14 ('ETH')
+   257         588 LOAD_CONST              14 ('ETH')
    
-   259         590 LOAD_CONST              73 ('https://zora.superscan.network/')
+   258         590 LOAD_CONST              73 ('https://scrollscan.com/')
    
-   253         592 KW_NAMES                22
+   252         592 KW_NAMES                22
                594 PRECALL                  6
                598 CALL                     6
-               608 STORE_NAME              22 (Zora)
+               608 STORE_NAME              22 (Scroll)
    
-   262         610 PUSH_NULL
+   261         610 PUSH_NULL
                612 LOAD_NAME                8 (Chain)
    
-   263         614 LOAD_CONST              74 ('Base')
+   262         614 LOAD_CONST              74 ('Zora')
    
-   264         616 LOAD_CONST              75 ('https://base.llamarpc.com')
+   263         616 LOAD_CONST              75 ('https://rpc.zora.energy')
    
-   265         618 LOAD_CONST              76 (8453)
+   264         618 LOAD_CONST              76 (7777777)
    
-   266         620 LOAD_CONST              13 (True)
+   265         620 LOAD_CONST              13 (True)
    
-   267         622 LOAD_CONST              14 ('ETH')
+   266         622 LOAD_CONST              14 ('ETH')
    
-   268         624 LOAD_CONST              77 ('https://basescan.com/')
+   267         624 LOAD_CONST              77 ('https://zora.superscan.network/')
    
-   262         626 KW_NAMES                22
+   261         626 KW_NAMES                22
                628 PRECALL                  6
                632 CALL                     6
-               642 STORE_NAME              23 (Base)
-               644 LOAD_CONST              78 (None)
-               646 RETURN_VALUE
+               642 STORE_NAME              23 (Zora)
+   
+   270         644 PUSH_NULL
+               646 LOAD_NAME                8 (Chain)
+   
+   271         648 LOAD_CONST              78 ('Base')
+   
+   272         650 LOAD_CONST              79 ('https://base.llamarpc.com')
+   
+   273         652 LOAD_CONST              80 (8453)
+   
+   274         654 LOAD_CONST              13 (True)
+   
+   275         656 LOAD_CONST              14 ('ETH')
+   
+   276         658 LOAD_CONST              81 ('https://basescan.com/')
+   
+   270         660 KW_NAMES                22
+               662 PRECALL                  6
+               666 CALL                     6
+               676 STORE_NAME              24 (Base)
+               678 LOAD_CONST              82 (None)
+               680 RETURN_VALUE
    consts
       0
       ('dataclass',)
       ('Decimal',)
       ('Union',)
       code
          argcount  : 0
@@ -638,15 +659,15 @@
             '_to'
             'transfer'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'Token')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\timer\\Code\\crypto_multitool\\evm\\models.py'
+         filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\models.py'
          name       'DefaultABIs'
          firstlineno 6
          lnotab
             0x0a0204050201020102010a010201020102f9040a0201020102010a0102
             01020102f9040a0201020102010a010201020102f9040a0201020102010a
             010201020102f9040a02010a0102010a010201020102f9040a0201120102
             010a010201020102f9040a02011201020102010201020102f9040a020112
@@ -696,30 +717,30 @@
                       68 LOAD_CONST               3 ('decimals')
                       70 LOAD_NAME                3 (int)
                       72 LOAD_CONST               7 ('wei')
                       74 LOAD_NAME                9 (bool)
                       76 LOAD_CONST               8 ('return')
                       78 LOAD_CONST               9 (None)
                       80 BUILD_TUPLE              8
-                      82 LOAD_CONST              10 (<code object __init__, file "C:\Users\timer\Code\crypto_multitool\evm\models.py", line 90>)
+                      82 LOAD_CONST              10 (<code object __init__, file "C:\Users\timer\Code\web3mt\web3mt\evm\models.py", line 90>)
                       84 MAKE_FUNCTION            5 (defaults, annotations)
                       86 STORE_NAME              10 (__init__)
          
          101          88 LOAD_CONST               8 ('return')
                       90 LOAD_NAME                8 (str)
                       92 BUILD_TUPLE              2
-                      94 LOAD_CONST              11 (<code object __str__, file "C:\Users\timer\Code\crypto_multitool\evm\models.py", line 101>)
+                      94 LOAD_CONST              11 (<code object __str__, file "C:\Users\timer\Code\web3mt\web3mt\evm\models.py", line 101>)
                       96 MAKE_FUNCTION            4 (annotations)
                       98 STORE_NAME              11 (__str__)
          
-         104         100 LOAD_CONST              12 (<code object __eq__, file "C:\Users\timer\Code\crypto_multitool\evm\models.py", line 104>)
+         104         100 LOAD_CONST              12 (<code object __eq__, file "C:\Users\timer\Code\web3mt\web3mt\evm\models.py", line 104>)
                      102 MAKE_FUNCTION            0
                      104 STORE_NAME              12 (__eq__)
          
-         107         106 LOAD_CONST              13 (<code object __bool__, file "C:\Users\timer\Code\crypto_multitool\evm\models.py", line 107>)
+         107         106 LOAD_CONST              13 (<code object __bool__, file "C:\Users\timer\Code\web3mt\web3mt\evm\models.py", line 107>)
                      108 MAKE_FUNCTION            0
                      110 STORE_NAME              13 (__bool__)
                      112 LOAD_CONST               9 (None)
                      114 RETURN_VALUE
          consts
             'TokenAmount'
             'Wei'
@@ -806,15 +827,15 @@
                consts
                   None
                   10
                names      ('Wei', 'Decimal', 'str', 'Ether', 'int', 'decimals')
                varnames   ('self', 'amount', 'decimals', 'wei')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\timer\\Code\\crypto_multitool\\evm\\models.py'
+               filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\models.py'
                name       '__init__'
                firstlineno 90
                lnotab 0x020104010e01500368014202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
@@ -832,15 +853,15 @@
                             40 RETURN_VALUE
                consts
                   None
                names      ('str', 'Ether')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\timer\\Code\\crypto_multitool\\evm\\models.py'
+               filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\models.py'
                name       '__str__'
                firstlineno 101
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
@@ -858,15 +879,15 @@
                             32 RETURN_VALUE
                consts
                   None
                names      ('Wei',)
                varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\timer\\Code\\crypto_multitool\\evm\\models.py'
+               filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\models.py'
                name       '__eq__'
                firstlineno 104
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
@@ -884,24 +905,24 @@
                             40 RETURN_VALUE
                consts
                   None
                names      ('bool', 'Wei')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\timer\\Code\\crypto_multitool\\evm\\models.py'
+               filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\models.py'
                name       '__bool__'
                firstlineno 107
                lnotab 0x0201
             (18, False)
          names      ('__name__', '__module__', '__qualname__', 'int', '__annotations__', 'Decimal', 'Union', 'float', 'str', 'bool', '__init__', '__str__', '__eq__', '__bool__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\timer\\Code\\crypto_multitool\\evm\\models.py'
+         filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\models.py'
          name       'TokenAmount'
          firstlineno 85
          lnotab 0x0c010a010a010a022e0b0c030603
       'TokenAmount'
       code
          argcount  : 0
          nlocals   : 0
@@ -951,19 +972,19 @@
          120          42 LOAD_NAME                4 (int)
          
          112          44 LOAD_CONST              10 ('max_gwei')
          
          121          46 LOAD_NAME                4 (int)
          
          112          48 BUILD_TUPLE             16
-                      50 LOAD_CONST              11 (<code object __init__, file "C:\Users\timer\Code\crypto_multitool\evm\models.py", line 112>)
+                      50 LOAD_CONST              11 (<code object __init__, file "C:\Users\timer\Code\web3mt\web3mt\evm\models.py", line 112>)
                       52 MAKE_FUNCTION            5 (defaults, annotations)
                       54 STORE_NAME               6 (__init__)
          
-         132          56 LOAD_CONST              12 (<code object __str__, file "C:\Users\timer\Code\crypto_multitool\evm\models.py", line 132>)
+         132          56 LOAD_CONST              12 (<code object __str__, file "C:\Users\timer\Code\web3mt\web3mt\evm\models.py", line 132>)
                       58 MAKE_FUNCTION            0
                       60 STORE_NAME               7 (__str__)
                       62 LOAD_CONST              13 (None)
                       64 RETURN_VALUE
          consts
             'Chain'
             18
@@ -1023,15 +1044,15 @@
                            116 RETURN_VALUE
                consts
                   None
                names      ('name', 'rpc', 'chain_id', 'eip1559_tx', 'coin_symbol', 'decimals', 'explorer', 'max_gwei')
                varnames   ('self', 'name', 'rpc', 'chain_id', 'eip1559_tx', 'coin_symbol', 'explorer', 'decimals', 'max_gwei')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\timer\\Code\\crypto_multitool\\evm\\models.py'
+               filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\models.py'
                name       '__init__'
                firstlineno 112
                lnotab 0x020b0e010e010e010e010e010e010e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -1045,25 +1066,25 @@
                             16 RETURN_VALUE
                consts
                   None
                names      ('name',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\timer\\Code\\crypto_multitool\\evm\\models.py'
+               filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\models.py'
                name       '__str__'
                firstlineno 132
                lnotab 0x0201
             None
             (18, 15)
          names      ('__name__', '__module__', '__qualname__', 'str', 'int', 'bool', '__init__', '__str__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\timer\\Code\\crypto_multitool\\evm\\models.py'
+         filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\models.py'
          name       'Chain'
          firstlineno 111
          lnotab
             0x0a09020102f7040202fe020302fd020402fc020502fb020602fa020702
             f9020802f8020902f70814
       'Chain'
       'Ethereum'
@@ -1079,14 +1100,18 @@
       42161
       'https://arbiscan.io/'
       ('name', 'rpc', 'chain_id', 'eip1559_tx', 'coin_symbol', 'explorer')
       'Optimism'
       'https://rpc.ankr.com/optimism/'
       10
       'https://optimistic.etherscan.io/'
+      'Optimism Sepolia'
+      'https://sepolia.optimism.io'
+      11155420
+      'https://optimism-sepolia.blockscout.com/'
       'Polygon'
       'https://polygon-rpc.com/'
       137
       'MATIC'
       'https://polygonscan.com/'
       'Mumbai'
       'https://polygon-mumbai-bor-rpc.publicnode.com'
@@ -1131,24 +1156,25 @@
       7777777
       'https://zora.superscan.network/'
       'Base'
       'https://base.llamarpc.com'
       8453
       'https://basescan.com/'
       None
-   names      ('dataclasses', 'dataclass', 'decimal', 'Decimal', 'typing', 'Union', 'DefaultABIs', 'TokenAmount', 'Chain', 'Ethereum', 'Arbitrum', 'Optimism', 'Polygon', 'Mumbai', 'Avalanche', 'Fantom', 'opBNB', 'BNB', 'Linea', 'zkSync', 'ZetaChain', 'Scroll', 'Zora', 'Base')
+   names      ('dataclasses', 'dataclass', 'decimal', 'Decimal', 'typing', 'Union', 'DefaultABIs', 'TokenAmount', 'Chain', 'Ethereum', 'Arbitrum', 'Optimism', 'OP_Sepolia', 'Polygon', 'Mumbai', 'Avalanche', 'Fantom', 'opBNB', 'BNB', 'Linea', 'zkSync', 'ZetaChain', 'Scroll', 'Zora', 'Base')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\timer\\Code\\crypto_multitool\\evm\\models.py'
+   filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\evm\\models.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c010c010c03020118ff0e01024e1a1a1a1904010201020102
       0102010201020102f9120a04010201020102010201020102fa1209040102
-      01020102010201020102fa120904010201020102010201020102fa120804
-      010201020102010201020102fa120904010201020102010201020102fa12
+      01020102010201020102fa120804010201020102010201020102fa120904
+      010201020102010201020102fa120804010201020102010201020102fa12
       0904010201020102010201020102fa120904010201020102010201020102
       fa120904010201020102010201020102fa12090401020102010201020102
       0102fa120904010201020102010201020102fa1209040102010201020102
       01020102fa120904010201020102010201020102fa120904010201020102
-      010201020102fa120904010201020102010201020102fa
+      010201020102fa120904010201020102010201020102fa12090401020102
+      0102010201020102fa
```

### Comparing `web3mt-0.0.1/web3mt/evm/client.py` & `web3mt-0.0.2/web3mt/evm/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,19 +46,18 @@
             modules={'eth': (AsyncEth,), 'net': (AsyncNet,)},
             middlewares=[async_geth_poa_middleware]
         )
         self.delay_between_requests = delay_between_requests
         self.sleep_echo = sleep_echo
         self.do_no_matter_what = do_no_matter_what
         self.log_info = ''
-        if self.profile:
-            self.log_info += f"{self.profile.id}"
         if self.account:
-            self.log_info += f' | {self.account.address} ({self.network.name})'
-
+            self.log_info += f'{self.account.address} ({self.network.name})'
+        if self.profile:
+            self.log_info = f"{self.profile.id} | {self.log_info}"
         self.okx_api_key = okx_api_key
         self.okx_api_secret = okx_api_secret
         self.okx_passphrase = okx_passphrase
 
     async def __aenter__(self):
         return self
 
@@ -180,15 +179,15 @@
         if self.network.max_gwei:
             while True:
                 gas_price = self.w3.from_wei(await self.w3.eth.gas_price, 'gwei')
                 if gas_price > self.network.max_gwei:
                     logger.debug(
                         f'{self.log_info} | Current GWEI: {gas_price} > {self.network.max_gwei}. Waiting for gwei...'
                     )
-                    await sleep(15)
+                    await sleep(15, profile_id=self.profile.id if self.profile else None, echo=self.sleep_echo)
                 else:
                     break
 
         if self.network.eip1559_tx:
             last_block = await self.w3.eth.get_block('latest')
             await sleep(
                 self.delay_between_requests,
@@ -394,14 +393,15 @@
             echo: bool = False,
             get_usd_price: bool = False
     ) -> TokenAmount:
         balance = TokenAmount(
             amount=await self.w3.eth.get_balance(address or self.account.address),
             wei=True
         )
-        Client.NATIVE_PRICE = Client.NATIVE_PRICE or await self.get_token_price(token=self.network.coin_symbol)
+        if get_usd_price:
+            Client.NATIVE_PRICE = Client.NATIVE_PRICE or await self.get_token_price(token=self.network.coin_symbol)
         if echo:
             logger.info(
                 f'{self.log_info} | Balance - {float(balance.Ether)} {self.network.coin_symbol}'
                 f'{f" {(Client.NATIVE_PRICE * float(balance.Ether)):2f}$" if get_usd_price else ""}',
             )
         return balance
```

### Comparing `web3mt-0.0.1/web3mt/evm/models.py` & `web3mt-0.0.2/web3mt/evm/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,22 @@
     name='Optimism',
     rpc='https://rpc.ankr.com/optimism/',
     chain_id=10,
     eip1559_tx=True,
     coin_symbol='ETH',
     explorer='https://optimistic.etherscan.io/',
 )
+OP_Sepolia = Chain(
+    name='Optimism Sepolia',
+    rpc='https://sepolia.optimism.io',
+    chain_id=11155420,
+    eip1559_tx=True,
+    coin_symbol='ETH',
+    explorer='https://optimism-sepolia.blockscout.com/',
+)
 
 Polygon = Chain(
     name='Polygon',
     rpc='https://polygon-rpc.com/',
     chain_id=137,
     eip1559_tx=True,
     coin_symbol='MATIC',
```

### Comparing `web3mt-0.0.1/web3mt/utils/__pycache__/__init__.cpython-311.pyc` & `web3mt-0.0.2/web3mt/utils/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `web3mt-0.0.1/web3mt/utils/__pycache__/logger.cpython-311.pyc` & `web3mt-0.0.2/web3mt/utils/__pycache__/logger.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `web3mt-0.0.1/web3mt/utils/__pycache__/profile_session.cpython-311.pyc` & `web3mt-0.0.2/web3mt/utils/__pycache__/profile_session.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x37b81a66 (Sat Apr 13 16:52:07 2024 UTC)
-files sz: 4766
+moddate:  0x32cf2766 (Tue Apr 23 15:09:38 2024 UTC)
+files sz: 4864
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
@@ -197,150 +197,150 @@
                       56 BUILD_TUPLE              8
                       58 LOAD_CLOSURE             0 (__class__)
                       60 BUILD_TUPLE              1
                       62 LOAD_CONST              17 (<code object __init__, file "C:\Users\timer\Code\web3mt\web3mt\utils\profile_session.py", line 35>)
                       64 MAKE_FUNCTION           13 (defaults, annotations, closure)
                       66 STORE_NAME               7 (__init__)
          
-          48          68 LOAD_CONST              18 (<code object __aenter__, file "C:\Users\timer\Code\web3mt\web3mt\utils\profile_session.py", line 48>)
+          49          68 LOAD_CONST              18 (<code object __aenter__, file "C:\Users\timer\Code\web3mt\web3mt\utils\profile_session.py", line 49>)
                       70 MAKE_FUNCTION            0
                       72 STORE_NAME               8 (__aenter__)
          
-          51          74 LOAD_CONST              19 (<code object __aexit__, file "C:\Users\timer\Code\web3mt\web3mt\utils\profile_session.py", line 51>)
+          52          74 LOAD_CONST              19 (<code object __aexit__, file "C:\Users\timer\Code\web3mt\web3mt\utils\profile_session.py", line 52>)
                       76 MAKE_FUNCTION            0
                       78 STORE_NAME               9 (__aexit__)
          
-          54          80 LOAD_CONST              20 ('func')
+          55          80 LOAD_CONST              20 ('func')
                       82 LOAD_NAME               10 (Callable)
                       84 LOAD_CONST              15 ('return')
                       86 LOAD_NAME               10 (Callable)
                       88 BUILD_TUPLE              4
-                      90 LOAD_CONST              21 (<code object retry, file "C:\Users\timer\Code\web3mt\web3mt\utils\profile_session.py", line 54>)
+                      90 LOAD_CONST              21 (<code object retry, file "C:\Users\timer\Code\web3mt\web3mt\utils\profile_session.py", line 55>)
                       92 MAKE_FUNCTION            4 (annotations)
                       94 STORE_NAME              11 (retry)
          
-          90          96 LOAD_NAME               11 (retry)
+          91          96 LOAD_NAME               11 (retry)
          
-          95          98 LOAD_CONST              16 (None)
+          96          98 LOAD_CONST              16 (None)
          
-          96         100 LOAD_CONST              16 (None)
+          97         100 LOAD_CONST              16 (None)
          
-          97         102 LOAD_CONST              16 (None)
+          98         102 LOAD_CONST              16 (None)
          
-          98         104 LOAD_CONST              16 (None)
+          99         104 LOAD_CONST              16 (None)
          
-          99         106 LOAD_CONST              22 (False)
+         100         106 LOAD_CONST              22 (False)
          
-         100         108 LOAD_CONST              22 (False)
+         101         108 LOAD_CONST              22 (False)
          
-         101         110 LOAD_NAME               12 (RETRY_COUNT)
+         102         110 LOAD_NAME               12 (RETRY_COUNT)
          
-         102         112 LOAD_CONST              23 (30)
+         103         112 LOAD_CONST              23 (30)
          
-          91         114 BUILD_TUPLE              8
+          92         114 BUILD_TUPLE              8
                      116 LOAD_CONST              24 ('method')
          
-          93         118 LOAD_NAME               13 (str)
+          94         118 LOAD_NAME               13 (str)
          
-          91         120 LOAD_CONST              25 ('url')
+          92         120 LOAD_CONST              25 ('url')
          
-          94         122 LOAD_NAME               13 (str)
+          95         122 LOAD_NAME               13 (str)
          
-          91         124 LOAD_CONST              26 ('params')
+          92         124 LOAD_CONST              26 ('params')
          
-          95         126 LOAD_NAME               14 (dict)
+          96         126 LOAD_NAME               14 (dict)
          
-          91         128 LOAD_CONST              27 ('headers')
+          92         128 LOAD_CONST              27 ('headers')
          
-          96         130 LOAD_NAME               14 (dict)
+          97         130 LOAD_NAME               14 (dict)
          
-          91         132 LOAD_CONST              28 ('data')
+          92         132 LOAD_CONST              28 ('data')
          
-          97         134 LOAD_NAME               14 (dict)
+          98         134 LOAD_NAME               14 (dict)
          
-          91         136 LOAD_CONST              29 ('json')
+          92         136 LOAD_CONST              29 ('json')
          
-          98         138 LOAD_NAME               14 (dict)
+          99         138 LOAD_NAME               14 (dict)
          
-          91         140 LOAD_CONST              30 ('follow_redirects')
+          92         140 LOAD_CONST              30 ('follow_redirects')
          
-          99         142 LOAD_NAME                6 (bool)
+         100         142 LOAD_NAME                6 (bool)
          
-          91         144 LOAD_CONST              31 ('verify')
+          92         144 LOAD_CONST              31 ('verify')
          
-         100         146 LOAD_NAME                6 (bool)
+         101         146 LOAD_NAME                6 (bool)
          
-          91         148 LOAD_CONST              32 ('retry_count')
+          92         148 LOAD_CONST              32 ('retry_count')
          
-         101         150 LOAD_NAME               15 (int)
+         102         150 LOAD_NAME               15 (int)
          
-          91         152 LOAD_CONST              33 ('timeout')
+          92         152 LOAD_CONST              33 ('timeout')
          
-         102         154 LOAD_NAME               15 (int)
+         103         154 LOAD_NAME               15 (int)
          
-          91         156 BUILD_TUPLE             20
+          92         156 BUILD_TUPLE             20
                      158 LOAD_CLOSURE             0 (__class__)
                      160 BUILD_TUPLE              1
-                     162 LOAD_CONST              34 (<code object request, file "C:\Users\timer\Code\web3mt\web3mt\utils\profile_session.py", line 90>)
+                     162 LOAD_CONST              34 (<code object request, file "C:\Users\timer\Code\web3mt\web3mt\utils\profile_session.py", line 91>)
                      164 MAKE_FUNCTION           13 (defaults, annotations, closure)
          
-          90         166 PRECALL                  0
+          91         166 PRECALL                  0
                      170 CALL                     0
          
-          91         180 STORE_NAME              16 (request)
+          92         180 STORE_NAME              16 (request)
          
-         121         182 PUSH_NULL
+         122         182 PUSH_NULL
                      184 LOAD_NAME               17 (partialmethod)
                      186 LOAD_NAME               16 (request)
                      188 LOAD_CONST              35 ('HEAD')
                      190 PRECALL                  2
                      194 CALL                     2
                      204 STORE_NAME              18 (head)
          
-         122         206 PUSH_NULL
+         123         206 PUSH_NULL
                      208 LOAD_NAME               17 (partialmethod)
                      210 LOAD_NAME               16 (request)
                      212 LOAD_CONST              36 ('GET')
                      214 PRECALL                  2
                      218 CALL                     2
                      228 STORE_NAME              19 (get)
          
-         123         230 PUSH_NULL
+         124         230 PUSH_NULL
                      232 LOAD_NAME               17 (partialmethod)
                      234 LOAD_NAME               16 (request)
                      236 LOAD_CONST              37 ('POST')
                      238 PRECALL                  2
                      242 CALL                     2
                      252 STORE_NAME              20 (post)
          
-         124         254 PUSH_NULL
+         125         254 PUSH_NULL
                      256 LOAD_NAME               17 (partialmethod)
                      258 LOAD_NAME               16 (request)
                      260 LOAD_CONST              38 ('PUT')
                      262 PRECALL                  2
                      266 CALL                     2
                      276 STORE_NAME              21 (put)
          
-         125         278 PUSH_NULL
+         126         278 PUSH_NULL
                      280 LOAD_NAME               17 (partialmethod)
                      282 LOAD_NAME               16 (request)
                      284 LOAD_CONST              39 ('PATCH')
                      286 PRECALL                  2
                      290 CALL                     2
                      300 STORE_NAME              22 (patch)
          
-         126         302 PUSH_NULL
+         127         302 PUSH_NULL
                      304 LOAD_NAME               17 (partialmethod)
                      306 LOAD_NAME               16 (request)
                      308 LOAD_CONST              40 ('DELETE')
                      310 PRECALL                  2
                      314 CALL                     2
                      324 STORE_NAME              23 (delete)
          
-         127         326 PUSH_NULL
+         128         326 PUSH_NULL
                      328 LOAD_NAME               17 (partialmethod)
                      330 LOAD_NAME               16 (request)
                      332 LOAD_CONST              41 ('OPTIONS')
                      334 PRECALL                  2
                      338 CALL                     2
                      348 STORE_NAME              24 (options)
                      350 LOAD_CLOSURE             0 (__class__)
@@ -373,19 +373,20 @@
                code
                   0x950197007c017c005f0000000000000000007c027c005f010000000000
                   0000007c037c005f0200000000000000007c04a003000000000000000000
                   000000000000000000000064017c006a040000000000000000a6020000ab
                   0200000000000000007d057c04a003000000000000000000000000000000
                   00000000006402740a000000000000000000006a0600000000000000006a
                   0700000000000000006a080000000000000000a6020000ab020000000000
-                  0000007d060200741300000000000000000000a6000000ab000000000000
-                  0000006a0a000000000000000064057417000000000000000000006a0c00
-                  000000000000007c016a0d00000000000000006a0e0000000000000000ac
-                  03a6010000ab0100000000000000006a0f00000000000000007c057c0664
-                  049c037c04a4018e01010064005300
+                  0000007d067c006a0000000000000000006a0900000000000000009b007c
+                  005f0a00000000000000000200741700000000000000000000a6000000ab
+                  0000000000000000006a0c00000000000000006405741b00000000000000
+                  0000006a0e00000000000000007c016a0f00000000000000006a10000000
+                  0000000000ac03a6010000ab0100000000000000006a1100000000000000
+                  007c057c0664049c037c04a4018e01010064005300
                              0 COPY_FREE_VARS           1
                
                 35           2 RESUME                   0
                
                 36           4 LOAD_FAST                1 (profile)
                              6 LOAD_FAST                0 (self)
                              8 STORE_ATTR               0 (profile)
@@ -414,96 +415,103 @@
                            138 LOAD_ATTR                6 (requests)
                            148 LOAD_ATTR                7 (BrowserType)
                            158 LOAD_ATTR                8 (chrome120)
                            168 PRECALL                  2
                            172 CALL                     2
                            182 STORE_FAST               6 (impersonate)
                
-                41         184 PUSH_NULL
-                           186 LOAD_GLOBAL             19 (NULL + super)
-                           198 PRECALL                  0
-                           202 CALL                     0
-                           212 LOAD_ATTR               10 (__init__)
-                           222 LOAD_CONST               5 (())
-               
-                42         224 LOAD_GLOBAL             23 (NULL + Proxy)
-                           236 LOAD_ATTR               12 (from_str)
-                           246 LOAD_FAST                1 (profile)
-                           248 LOAD_ATTR               13 (proxy)
-                           258 LOAD_ATTR               14 (proxy_string)
-                           268 KW_NAMES                 3
-                           270 PRECALL                  1
-                           274 CALL                     1
-                           284 LOAD_ATTR               15 (as_url)
-               
-                43         294 LOAD_FAST                5 (headers)
-               
-                44         296 LOAD_FAST                6 (impersonate)
-               
-                41         298 LOAD_CONST               4 (('proxy', 'headers', 'impersonate'))
-                           300 BUILD_CONST_KEY_MAP      3
-               
-                45         302 LOAD_FAST                4 (kwargs)
-               
-                41         304 DICT_MERGE               1
-                           306 CALL_FUNCTION_EX         1
-                           308 POP_TOP
-                           310 LOAD_CONST               0 (None)
-                           312 RETURN_VALUE
+                41         184 LOAD_FAST                0 (self)
+                           186 LOAD_ATTR                0 (profile)
+                           196 LOAD_ATTR                9 (id)
+                           206 FORMAT_VALUE             0
+                           208 LOAD_FAST                0 (self)
+                           210 STORE_ATTR              10 (log_info)
+               
+                42         220 PUSH_NULL
+                           222 LOAD_GLOBAL             23 (NULL + super)
+                           234 PRECALL                  0
+                           238 CALL                     0
+                           248 LOAD_ATTR               12 (__init__)
+                           258 LOAD_CONST               5 (())
+               
+                43         260 LOAD_GLOBAL             27 (NULL + Proxy)
+                           272 LOAD_ATTR               14 (from_str)
+                           282 LOAD_FAST                1 (profile)
+                           284 LOAD_ATTR               15 (proxy)
+                           294 LOAD_ATTR               16 (proxy_string)
+                           304 KW_NAMES                 3
+                           306 PRECALL                  1
+                           310 CALL                     1
+                           320 LOAD_ATTR               17 (as_url)
+               
+                44         330 LOAD_FAST                5 (headers)
+               
+                45         332 LOAD_FAST                6 (impersonate)
+               
+                42         334 LOAD_CONST               4 (('proxy', 'headers', 'impersonate'))
+                           336 BUILD_CONST_KEY_MAP      3
+               
+                46         338 LOAD_FAST                4 (kwargs)
+               
+                42         340 DICT_MERGE               1
+                           342 CALL_FUNCTION_EX         1
+                           344 POP_TOP
+                           346 LOAD_CONST               0 (None)
+                           348 RETURN_VALUE
                consts
                   None
                   'headers'
                   'impersonate'
                   ('proxy',)
                   ('proxy', 'headers', 'impersonate')
                   ()
-               names      ('profile', 'sleep_echo', 'request_echo', 'pop', 'DEFAULT_HEADERS', 'curl_cffi', 'requests', 'BrowserType', 'chrome120', 'super', '__init__', 'Proxy', 'from_str', 'proxy', 'proxy_string', 'as_url')
+               names      ('profile', 'sleep_echo', 'request_echo', 'pop', 'DEFAULT_HEADERS', 'curl_cffi', 'requests', 'BrowserType', 'chrome120', 'id', 'log_info', 'super', '__init__', 'Proxy', 'from_str', 'proxy', 'proxy_string', 'as_url')
                varnames   ('self', 'profile', 'sleep_echo', 'requests_echo', 'kwargs', 'headers', 'impersonate')
                freevars   ('__class__',)
                cellvars   ()
                filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\utils\\profile_session.py'
                name       '__init__'
                firstlineno 35
-               lnotab 0x04010e010e010e013601540128014601020102fd040402fc
+               lnotab 0x04010e010e010e0136015401240128014601020102fd040402fc
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 131
                code 0x4b00010097007c005300
-                48           0 RETURN_GENERATOR
+                49           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                49           6 LOAD_FAST                0 (self)
+                50           6 LOAD_FAST                0 (self)
                              8 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\utils\\profile_session.py'
                name       '__aenter__'
-               firstlineno 48
+               firstlineno 49
                lnotab 0x0601
             code
                argcount  : 4
                nlocals   : 4
                stacksize : 2
                flags     : 131
                code
                   0x4b00010097007c00a00000000000000000000000000000000000000000
                   00a6000000ab000000000000000000830064007b03560097038604010064
                   005300
-                51           0 RETURN_GENERATOR
+                52           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                52           6 LOAD_FAST                0 (self)
+                53           6 LOAD_FAST                0 (self)
                              8 LOAD_METHOD              0 (close)
                             30 PRECALL                  0
                             34 CALL                     0
                             44 GET_AWAITABLE            0
                             46 LOAD_CONST               0 (None)
                        >>   48 SEND                     3 (to 56)
                             50 YIELD_VALUE
@@ -516,39 +524,39 @@
                   None
                names      ('close',)
                varnames   ('self', 'exc_type', 'exc_val', 'exc_tb')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\utils\\profile_session.py'
                name       '__aexit__'
-               firstlineno 51
+               firstlineno 52
                lnotab 0x0601
             'func'
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x8700970064017400000000000000000000006602880066016402840c7d
                   017c015300
                              0 MAKE_CELL                0 (func)
                
-                54           2 RESUME                   0
+                55           2 RESUME                   0
                
-                55           4 LOAD_CONST               1 ('return')
+                56           4 LOAD_CONST               1 ('return')
                              6 LOAD_GLOBAL              0 (Any)
                             18 BUILD_TUPLE              2
                             20 LOAD_CLOSURE             0 (func)
                             22 BUILD_TUPLE              1
-                            24 LOAD_CONST               2 (<code object wrapper, file "C:\Users\timer\Code\web3mt\web3mt\utils\profile_session.py", line 55>)
+                            24 LOAD_CONST               2 (<code object wrapper, file "C:\Users\timer\Code\web3mt\web3mt\utils\profile_session.py", line 56>)
                             26 MAKE_FUNCTION           12 (annotations, closure)
                             28 STORE_FAST               1 (wrapper)
                
-                88          30 LOAD_FAST                1 (wrapper)
+                89          30 LOAD_FAST                1 (wrapper)
                             32 RETURN_VALUE
                consts
                   None
                   'return'
                   code
                      argcount  : 1
                      nlocals   : 12
@@ -563,94 +571,95 @@
                         006a03000000000000000064066407a6020000ab020000000000000000a6
                         020000ab0200000000000000007d057c02a0010000000000000000000000
                         0000000000000000006408740800000000000000000000a6020000ab0200
                         000000000000007d067c006a0500000000000000007226740d0000000000
                         00000000006a0700000000000000007c006a0800000000000000006a0900
                         000000000000009b0064097c039b00640a7c049b009d05a6010000ab0100
                         00000000000000010064007d077415000000000000000000007c06a60100
-                        00ab010000000000000000440090015d5b7d0809000200890c7c0067017c
+                        00ab010000000000000000440090015d6e7d0809000200890c7c0067017c
                         01a201520069007c02a4018e01830064007b035600970386045c0200007d
                         097d077c02a0000000000000000000000000000000000000000000640ba6
                         010000ab01000000000000000073147c09a00b0000000000000000000000
                         000000000000000000a6000000ab00000000000000000001007419000000
-                        000000000000007c057c006a0800000000000000006a0900000000000000
-                        007c006a0d0000000000000000ac0ca6030000ab03000000000000000083
-                        0064007b0356009703860401007c097c0766026302010053002300741c00
-                        000000000000000000240072e17d0a7c006a0800000000000000006a0900
-                        000000000000009b0064097c049b00640a7c0a9b00640a7c0781027c076e
-                        01640d9b009d077d0b7c0a6a0f0000000000000000640e7600724c740d00
-                        0000000000000000006a1000000000000000007c0b9b00640f7c0864107a
-                        0000009b0064117c059b0064129d06a6010000ab01000000000000000001
-                        007419000000000000000000007c057c006a0800000000000000006a0900
-                        000000000000007c006a0d0000000000000000ac0ca6030000ab03000000
-                        0000000000830064007b035600970386040100590064007d0a7e0a8ce97c
-                        096a110000000000000000641376007216740d000000000000000000006a
-                        1000000000000000007c0ba6010000ab01000000000000000001007c0a82
-                        01740d000000000000000000006a1000000000000000007c0b9b00640f7c
-                        0864107a0000009b0064117c059b0064129d06a6010000ab010000000000
-                        00000001007419000000000000000000007c057c006a0800000000000000
-                        006a0900000000000000007c006a0d0000000000000000ac0ca6030000ab
-                        030000000000000000830064007b035600970386040100590064007d0a7e
-                        0a90018c5564007d0a7e0a770177007803590077017c006a050000000000
-                        0000007229740d000000000000000000006a0700000000000000007c006a
-                        0800000000000000006a0900000000000000009b00641474080000000000
-                        00000000009b0064159d04a6010000ab0100000000000000000100640053
-                        00
+                        000000000000007405000000000000000000006a03000000000000000064
+                        066407a6020000ab0200000000000000007c006a0800000000000000006a
+                        0900000000000000007c006a0d0000000000000000ac0ca6030000ab0300
+                        00000000000000830064007b0356009703860401007c097c076602630201
+                        0053002300741c00000000000000000000240072e17d0a7c006a08000000
+                        00000000006a0900000000000000009b0064097c049b00640a7c0a9b0064
+                        0a7c0781027c076e01640d9b009d077d0b7c0a6a0f000000000000000064
+                        0e7600724c740d000000000000000000006a1000000000000000007c0b9b
+                        00640f7c0864107a0000009b0064117c059b0064129d06a6010000ab0100
+                        0000000000000001007419000000000000000000007c057c006a08000000
+                        00000000006a0900000000000000007c006a0d0000000000000000ac0ca6
+                        030000ab030000000000000000830064007b035600970386040100590064
+                        007d0a7e0a8cfc7c096a110000000000000000641376007216740d000000
+                        000000000000006a1000000000000000007c0ba6010000ab010000000000
+                        00000001007c0a8201740d000000000000000000006a1000000000000000
+                        007c0b9b00640f7c0864107a0000009b0064117c059b0064129d06a60100
+                        00ab01000000000000000001007419000000000000000000007c057c006a
+                        0800000000000000006a0900000000000000007c006a0d00000000000000
+                        00ac0ca6030000ab030000000000000000830064007b0356009703860401
+                        00590064007d0a7e0a90018c6864007d0a7e0a770177007803590077017c
+                        006a0500000000000000007229740d000000000000000000006a07000000
+                        00000000007c006a0800000000000000006a0900000000000000009b0064
+                        147408000000000000000000009b0064159d04a6010000ab010000000000
+                        000000010064005300
                                    0 COPY_FREE_VARS           1
                      
-                      55           2 RETURN_GENERATOR
+                      56           2 RETURN_GENERATOR
                                    4 POP_TOP
                                    6 RESUME                   0
                      
-                      56           8 LOAD_FAST                2 (kwargs)
+                      57           8 LOAD_FAST                2 (kwargs)
                                   10 LOAD_METHOD              0 (get)
                                   32 LOAD_CONST               1 ('method')
                                   34 LOAD_CONST               0 (None)
                                   36 PRECALL                  2
                                   40 CALL                     2
                                   50 JUMP_IF_TRUE_OR_POP      7 (to 66)
                                   52 LOAD_FAST                1 (args)
                                   54 LOAD_CONST               2 (0)
                                   56 BINARY_SUBSCR
                              >>   66 STORE_FAST               3 (method)
                      
-                      57          68 LOAD_FAST                2 (kwargs)
+                      58          68 LOAD_FAST                2 (kwargs)
                                   70 LOAD_METHOD              0 (get)
                                   92 LOAD_CONST               3 ('url')
                                   94 LOAD_CONST               4 ('unknown url')
                                   96 PRECALL                  2
                                  100 CALL                     2
                                  110 STORE_FAST               4 (url)
                      
-                      58         112 LOAD_FAST                2 (kwargs)
+                      59         112 LOAD_FAST                2 (kwargs)
                                  114 LOAD_METHOD              1 (pop)
-                                 136 LOAD_CONST               5 ('delay')
+                                 136 LOAD_CONST               5 ('retry_delay')
                                  138 LOAD_GLOBAL              5 (NULL + random)
                                  150 LOAD_ATTR                3 (uniform)
                                  160 LOAD_CONST               6 (5)
                                  162 LOAD_CONST               7 (10)
                                  164 PRECALL                  2
                                  168 CALL                     2
                                  178 PRECALL                  2
                                  182 CALL                     2
-                                 192 STORE_FAST               5 (delay)
+                                 192 STORE_FAST               5 (retry_delay)
                      
-                      59         194 LOAD_FAST                2 (kwargs)
+                      60         194 LOAD_FAST                2 (kwargs)
                                  196 LOAD_METHOD              1 (pop)
                                  218 LOAD_CONST               8 ('retry_count')
                                  220 LOAD_GLOBAL              8 (RETRY_COUNT)
                                  232 PRECALL                  2
                                  236 CALL                     2
                                  246 STORE_FAST               6 (retry_count)
                      
-                      60         248 LOAD_FAST                0 (self)
+                      61         248 LOAD_FAST                0 (self)
                                  250 LOAD_ATTR                5 (request_echo)
                                  260 POP_JUMP_FORWARD_IF_FALSE    38 (to 338)
                      
-                      61         262 LOAD_GLOBAL             13 (NULL + logger)
+                      62         262 LOAD_GLOBAL             13 (NULL + logger)
                                  274 LOAD_ATTR                7 (info)
                                  284 LOAD_FAST                0 (self)
                                  286 LOAD_ATTR                8 (profile)
                                  296 LOAD_ATTR                9 (id)
                                  306 FORMAT_VALUE             0
                                  308 LOAD_CONST               9 (' | ')
                                  310 LOAD_FAST                3 (method)
@@ -659,29 +668,29 @@
                                  316 LOAD_FAST                4 (url)
                                  318 FORMAT_VALUE             0
                                  320 BUILD_STRING             5
                                  322 PRECALL                  1
                                  326 CALL                     1
                                  336 POP_TOP
                      
-                      62     >>  338 LOAD_CONST               0 (None)
+                      63     >>  338 LOAD_CONST               0 (None)
                                  340 STORE_FAST               7 (data)
                      
-                      63         342 LOAD_GLOBAL             21 (NULL + range)
+                      64         342 LOAD_GLOBAL             21 (NULL + range)
                                  354 LOAD_FAST                6 (retry_count)
                                  356 PRECALL                  1
                                  360 CALL                     1
                                  370 GET_ITER
                              >>  372 EXTENDED_ARG             1
-                                 374 FOR_ITER               347 (to 1070)
+                                 374 FOR_ITER               366 (to 1108)
                                  376 STORE_FAST               8 (i)
                      
-                      64         378 NOP
+                      65         378 NOP
                      
-                      65         380 PUSH_NULL
+                      66         380 PUSH_NULL
                                  382 LOAD_DEREF              12 (func)
                                  384 LOAD_FAST                0 (self)
                                  386 BUILD_LIST               1
                                  388 LOAD_FAST                1 (args)
                                  390 LIST_EXTEND              1
                                  392 LIST_TO_TUPLE
                                  394 BUILD_MAP                0
@@ -694,228 +703,233 @@
                                  408 YIELD_VALUE
                                  410 RESUME                   3
                                  412 JUMP_BACKWARD_NO_INTERRUPT     4 (to 406)
                              >>  414 UNPACK_SEQUENCE          2
                                  418 STORE_FAST               9 (response)
                                  420 STORE_FAST               7 (data)
                      
-                      66         422 LOAD_FAST                2 (kwargs)
+                      67         422 LOAD_FAST                2 (kwargs)
                                  424 LOAD_METHOD              0 (get)
                                  446 LOAD_CONST              11 ('follow_redirects')
                                  448 PRECALL                  1
                                  452 CALL                     1
                                  462 POP_JUMP_FORWARD_IF_TRUE    20 (to 504)
                      
-                      67         464 LOAD_FAST                9 (response)
+                      68         464 LOAD_FAST                9 (response)
                                  466 LOAD_METHOD             11 (raise_for_status)
                                  488 PRECALL                  0
                                  492 CALL                     0
                                  502 POP_TOP
                      
-                      68     >>  504 LOAD_GLOBAL             25 (NULL + sleep)
-                                 516 LOAD_FAST                5 (delay)
-                                 518 LOAD_FAST                0 (self)
-                                 520 LOAD_ATTR                8 (profile)
-                                 530 LOAD_ATTR                9 (id)
-                                 540 LOAD_FAST                0 (self)
-                                 542 LOAD_ATTR               13 (sleep_echo)
-                                 552 KW_NAMES                12
-                                 554 PRECALL                  3
-                                 558 CALL                     3
-                                 568 GET_AWAITABLE            0
-                                 570 LOAD_CONST               0 (None)
-                             >>  572 SEND                     3 (to 580)
-                                 574 YIELD_VALUE
-                                 576 RESUME                   3
-                                 578 JUMP_BACKWARD_NO_INTERRUPT     4 (to 572)
-                             >>  580 POP_TOP
-                     
-                      69         582 LOAD_FAST                9 (response)
-                                 584 LOAD_FAST                7 (data)
-                                 586 BUILD_TUPLE              2
-                                 588 SWAP                     2
-                                 590 POP_TOP
-                                 592 RETURN_VALUE
-                             >>  594 PUSH_EXC_INFO
-                     
-                      70         596 LOAD_GLOBAL             28 (RequestsError)
-                                 608 CHECK_EXC_MATCH
-                                 610 POP_JUMP_FORWARD_IF_FALSE   225 (to 1062)
-                                 612 STORE_FAST              10 (e)
-                     
-                      71         614 LOAD_FAST                0 (self)
-                                 616 LOAD_ATTR                8 (profile)
-                                 626 LOAD_ATTR                9 (id)
-                                 636 FORMAT_VALUE             0
-                                 638 LOAD_CONST               9 (' | ')
-                                 640 LOAD_FAST                4 (url)
-                                 642 FORMAT_VALUE             0
-                                 644 LOAD_CONST              10 (' ')
-                                 646 LOAD_FAST               10 (e)
-                                 648 FORMAT_VALUE             0
-                                 650 LOAD_CONST              10 (' ')
-                                 652 LOAD_FAST                7 (data)
-                                 654 POP_JUMP_FORWARD_IF_NONE     2 (to 660)
-                                 656 LOAD_FAST                7 (data)
-                                 658 JUMP_FORWARD             1 (to 662)
-                             >>  660 LOAD_CONST              13 ('')
-                             >>  662 FORMAT_VALUE             0
-                                 664 BUILD_STRING             7
-                                 666 STORE_FAST              11 (s)
-                     
-                      72         668 LOAD_FAST               10 (e)
-                                 670 LOAD_ATTR               15 (code)
-                                 680 LOAD_CONST              14 ((28, 35, 52, 56))
-                                 682 CONTAINS_OP              0
-                                 684 POP_JUMP_FORWARD_IF_FALSE    76 (to 838)
-                     
-                      73         686 LOAD_GLOBAL             13 (NULL + logger)
-                                 698 LOAD_ATTR               16 (warning)
-                                 708 LOAD_FAST               11 (s)
-                                 710 FORMAT_VALUE             0
-                                 712 LOAD_CONST              15 (' Retrying ')
-                                 714 LOAD_FAST                8 (i)
-                                 716 LOAD_CONST              16 (1)
-                                 718 BINARY_OP                0 (+)
-                                 722 FORMAT_VALUE             0
-                                 724 LOAD_CONST              17 (' after ')
-                                 726 LOAD_FAST                5 (delay)
-                                 728 FORMAT_VALUE             0
-                                 730 LOAD_CONST              18 (' seconds')
-                                 732 BUILD_STRING             6
-                                 734 PRECALL                  1
-                                 738 CALL                     1
-                                 748 POP_TOP
-                     
-                      74         750 LOAD_GLOBAL             25 (NULL + sleep)
-                                 762 LOAD_FAST                5 (delay)
-                                 764 LOAD_FAST                0 (self)
-                                 766 LOAD_ATTR                8 (profile)
-                                 776 LOAD_ATTR                9 (id)
-                                 786 LOAD_FAST                0 (self)
-                                 788 LOAD_ATTR               13 (sleep_echo)
-                                 798 KW_NAMES                12
-                                 800 PRECALL                  3
-                                 804 CALL                     3
-                                 814 GET_AWAITABLE            0
-                                 816 LOAD_CONST               0 (None)
-                             >>  818 SEND                     3 (to 826)
-                                 820 YIELD_VALUE
-                                 822 RESUME                   3
-                                 824 JUMP_BACKWARD_NO_INTERRUPT     4 (to 818)
-                             >>  826 POP_TOP
-                     
-                      75         828 POP_EXCEPT
-                                 830 LOAD_CONST               0 (None)
-                                 832 STORE_FAST              10 (e)
-                                 834 DELETE_FAST             10 (e)
-                                 836 JUMP_BACKWARD          233 (to 372)
-                     
-                      76     >>  838 LOAD_FAST                9 (response)
-                                 840 LOAD_ATTR               17 (status_code)
-                                 850 LOAD_CONST              19 ((400, 401, 403, 404, 500))
-                                 852 CONTAINS_OP              0
-                                 854 POP_JUMP_FORWARD_IF_FALSE    22 (to 900)
-                     
-                      77         856 LOAD_GLOBAL             13 (NULL + logger)
-                                 868 LOAD_ATTR               16 (warning)
-                                 878 LOAD_FAST               11 (s)
-                                 880 PRECALL                  1
-                                 884 CALL                     1
-                                 894 POP_TOP
-                     
-                      78         896 LOAD_FAST               10 (e)
-                                 898 RAISE_VARARGS            1
-                     
-                      80     >>  900 LOAD_GLOBAL             13 (NULL + logger)
-                                 912 LOAD_ATTR               16 (warning)
-                                 922 LOAD_FAST               11 (s)
-                                 924 FORMAT_VALUE             0
-                                 926 LOAD_CONST              15 (' Retrying ')
-                                 928 LOAD_FAST                8 (i)
-                                 930 LOAD_CONST              16 (1)
-                                 932 BINARY_OP                0 (+)
-                                 936 FORMAT_VALUE             0
-                                 938 LOAD_CONST              17 (' after ')
-                                 940 LOAD_FAST                5 (delay)
-                                 942 FORMAT_VALUE             0
-                                 944 LOAD_CONST              18 (' seconds')
-                                 946 BUILD_STRING             6
-                                 948 PRECALL                  1
-                                 952 CALL                     1
-                                 962 POP_TOP
-                     
-                      81         964 LOAD_GLOBAL             25 (NULL + sleep)
-                                 976 LOAD_FAST                5 (delay)
-                                 978 LOAD_FAST                0 (self)
-                                 980 LOAD_ATTR                8 (profile)
-                                 990 LOAD_ATTR                9 (id)
-                                1000 LOAD_FAST                0 (self)
-                                1002 LOAD_ATTR               13 (sleep_echo)
-                                1012 KW_NAMES                12
-                                1014 PRECALL                  3
-                                1018 CALL                     3
-                                1028 GET_AWAITABLE            0
-                                1030 LOAD_CONST               0 (None)
-                             >> 1032 SEND                     3 (to 1040)
-                                1034 YIELD_VALUE
-                                1036 RESUME                   3
-                                1038 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1032)
-                             >> 1040 POP_TOP
-                     
-                      82        1042 POP_EXCEPT
-                                1044 LOAD_CONST               0 (None)
-                                1046 STORE_FAST              10 (e)
-                                1048 DELETE_FAST             10 (e)
-                                1050 EXTENDED_ARG             1
-                                1052 JUMP_BACKWARD          341 (to 372)
-                             >> 1054 LOAD_CONST               0 (None)
-                                1056 STORE_FAST              10 (e)
-                                1058 DELETE_FAST             10 (e)
-                                1060 RERAISE                  1
-                     
-                      70     >> 1062 RERAISE                  0
-                             >> 1064 COPY                     3
-                                1066 POP_EXCEPT
-                                1068 RERAISE                  1
-                     
-                      84     >> 1070 LOAD_FAST                0 (self)
-                                1072 LOAD_ATTR                5 (request_echo)
-                                1082 POP_JUMP_FORWARD_IF_FALSE    41 (to 1166)
-                     
-                      85        1084 LOAD_GLOBAL             13 (NULL + logger)
-                                1096 LOAD_ATTR                7 (info)
-                                1106 LOAD_FAST                0 (self)
-                                1108 LOAD_ATTR                8 (profile)
-                                1118 LOAD_ATTR                9 (id)
-                                1128 FORMAT_VALUE             0
-                                1130 LOAD_CONST              20 (' | Tried to retry ')
-                                1132 LOAD_GLOBAL              8 (RETRY_COUNT)
-                                1144 FORMAT_VALUE             0
-                                1146 LOAD_CONST              21 (' times. Nothing can do anymore :(')
-                                1148 BUILD_STRING             4
-                                1150 PRECALL                  1
-                                1154 CALL                     1
-                                1164 POP_TOP
+                      69     >>  504 LOAD_GLOBAL             25 (NULL + sleep)
+                                 516 LOAD_GLOBAL              5 (NULL + random)
+                                 528 LOAD_ATTR                3 (uniform)
+                                 538 LOAD_CONST               6 (5)
+                                 540 LOAD_CONST               7 (10)
+                                 542 PRECALL                  2
+                                 546 CALL                     2
+                                 556 LOAD_FAST                0 (self)
+                                 558 LOAD_ATTR                8 (profile)
+                                 568 LOAD_ATTR                9 (id)
+                                 578 LOAD_FAST                0 (self)
+                                 580 LOAD_ATTR               13 (sleep_echo)
+                                 590 KW_NAMES                12
+                                 592 PRECALL                  3
+                                 596 CALL                     3
+                                 606 GET_AWAITABLE            0
+                                 608 LOAD_CONST               0 (None)
+                             >>  610 SEND                     3 (to 618)
+                                 612 YIELD_VALUE
+                                 614 RESUME                   3
+                                 616 JUMP_BACKWARD_NO_INTERRUPT     4 (to 610)
+                             >>  618 POP_TOP
+                     
+                      70         620 LOAD_FAST                9 (response)
+                                 622 LOAD_FAST                7 (data)
+                                 624 BUILD_TUPLE              2
+                                 626 SWAP                     2
+                                 628 POP_TOP
+                                 630 RETURN_VALUE
+                             >>  632 PUSH_EXC_INFO
+                     
+                      71         634 LOAD_GLOBAL             28 (RequestsError)
+                                 646 CHECK_EXC_MATCH
+                                 648 POP_JUMP_FORWARD_IF_FALSE   225 (to 1100)
+                                 650 STORE_FAST              10 (e)
+                     
+                      72         652 LOAD_FAST                0 (self)
+                                 654 LOAD_ATTR                8 (profile)
+                                 664 LOAD_ATTR                9 (id)
+                                 674 FORMAT_VALUE             0
+                                 676 LOAD_CONST               9 (' | ')
+                                 678 LOAD_FAST                4 (url)
+                                 680 FORMAT_VALUE             0
+                                 682 LOAD_CONST              10 (' ')
+                                 684 LOAD_FAST               10 (e)
+                                 686 FORMAT_VALUE             0
+                                 688 LOAD_CONST              10 (' ')
+                                 690 LOAD_FAST                7 (data)
+                                 692 POP_JUMP_FORWARD_IF_NONE     2 (to 698)
+                                 694 LOAD_FAST                7 (data)
+                                 696 JUMP_FORWARD             1 (to 700)
+                             >>  698 LOAD_CONST              13 ('')
+                             >>  700 FORMAT_VALUE             0
+                                 702 BUILD_STRING             7
+                                 704 STORE_FAST              11 (s)
+                     
+                      73         706 LOAD_FAST               10 (e)
+                                 708 LOAD_ATTR               15 (code)
+                                 718 LOAD_CONST              14 ((28, 35, 52, 56))
+                                 720 CONTAINS_OP              0
+                                 722 POP_JUMP_FORWARD_IF_FALSE    76 (to 876)
+                     
+                      74         724 LOAD_GLOBAL             13 (NULL + logger)
+                                 736 LOAD_ATTR               16 (warning)
+                                 746 LOAD_FAST               11 (s)
+                                 748 FORMAT_VALUE             0
+                                 750 LOAD_CONST              15 (' Retrying ')
+                                 752 LOAD_FAST                8 (i)
+                                 754 LOAD_CONST              16 (1)
+                                 756 BINARY_OP                0 (+)
+                                 760 FORMAT_VALUE             0
+                                 762 LOAD_CONST              17 (' after ')
+                                 764 LOAD_FAST                5 (retry_delay)
+                                 766 FORMAT_VALUE             0
+                                 768 LOAD_CONST              18 (' seconds')
+                                 770 BUILD_STRING             6
+                                 772 PRECALL                  1
+                                 776 CALL                     1
+                                 786 POP_TOP
+                     
+                      75         788 LOAD_GLOBAL             25 (NULL + sleep)
+                                 800 LOAD_FAST                5 (retry_delay)
+                                 802 LOAD_FAST                0 (self)
+                                 804 LOAD_ATTR                8 (profile)
+                                 814 LOAD_ATTR                9 (id)
+                                 824 LOAD_FAST                0 (self)
+                                 826 LOAD_ATTR               13 (sleep_echo)
+                                 836 KW_NAMES                12
+                                 838 PRECALL                  3
+                                 842 CALL                     3
+                                 852 GET_AWAITABLE            0
+                                 854 LOAD_CONST               0 (None)
+                             >>  856 SEND                     3 (to 864)
+                                 858 YIELD_VALUE
+                                 860 RESUME                   3
+                                 862 JUMP_BACKWARD_NO_INTERRUPT     4 (to 856)
+                             >>  864 POP_TOP
+                     
+                      76         866 POP_EXCEPT
+                                 868 LOAD_CONST               0 (None)
+                                 870 STORE_FAST              10 (e)
+                                 872 DELETE_FAST             10 (e)
+                                 874 JUMP_BACKWARD          252 (to 372)
+                     
+                      77     >>  876 LOAD_FAST                9 (response)
+                                 878 LOAD_ATTR               17 (status_code)
+                                 888 LOAD_CONST              19 ((400, 401, 403, 404, 500))
+                                 890 CONTAINS_OP              0
+                                 892 POP_JUMP_FORWARD_IF_FALSE    22 (to 938)
+                     
+                      78         894 LOAD_GLOBAL             13 (NULL + logger)
+                                 906 LOAD_ATTR               16 (warning)
+                                 916 LOAD_FAST               11 (s)
+                                 918 PRECALL                  1
+                                 922 CALL                     1
+                                 932 POP_TOP
+                     
+                      79         934 LOAD_FAST               10 (e)
+                                 936 RAISE_VARARGS            1
+                     
+                      81     >>  938 LOAD_GLOBAL             13 (NULL + logger)
+                                 950 LOAD_ATTR               16 (warning)
+                                 960 LOAD_FAST               11 (s)
+                                 962 FORMAT_VALUE             0
+                                 964 LOAD_CONST              15 (' Retrying ')
+                                 966 LOAD_FAST                8 (i)
+                                 968 LOAD_CONST              16 (1)
+                                 970 BINARY_OP                0 (+)
+                                 974 FORMAT_VALUE             0
+                                 976 LOAD_CONST              17 (' after ')
+                                 978 LOAD_FAST                5 (retry_delay)
+                                 980 FORMAT_VALUE             0
+                                 982 LOAD_CONST              18 (' seconds')
+                                 984 BUILD_STRING             6
+                                 986 PRECALL                  1
+                                 990 CALL                     1
+                                1000 POP_TOP
+                     
+                      82        1002 LOAD_GLOBAL             25 (NULL + sleep)
+                                1014 LOAD_FAST                5 (retry_delay)
+                                1016 LOAD_FAST                0 (self)
+                                1018 LOAD_ATTR                8 (profile)
+                                1028 LOAD_ATTR                9 (id)
+                                1038 LOAD_FAST                0 (self)
+                                1040 LOAD_ATTR               13 (sleep_echo)
+                                1050 KW_NAMES                12
+                                1052 PRECALL                  3
+                                1056 CALL                     3
+                                1066 GET_AWAITABLE            0
+                                1068 LOAD_CONST               0 (None)
+                             >> 1070 SEND                     3 (to 1078)
+                                1072 YIELD_VALUE
+                                1074 RESUME                   3
+                                1076 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1070)
+                             >> 1078 POP_TOP
+                     
+                      83        1080 POP_EXCEPT
+                                1082 LOAD_CONST               0 (None)
+                                1084 STORE_FAST              10 (e)
+                                1086 DELETE_FAST             10 (e)
+                                1088 EXTENDED_ARG             1
+                                1090 JUMP_BACKWARD          360 (to 372)
+                             >> 1092 LOAD_CONST               0 (None)
+                                1094 STORE_FAST              10 (e)
+                                1096 DELETE_FAST             10 (e)
+                                1098 RERAISE                  1
+                     
+                      71     >> 1100 RERAISE                  0
+                             >> 1102 COPY                     3
+                                1104 POP_EXCEPT
+                                1106 RERAISE                  1
+                     
+                      85     >> 1108 LOAD_FAST                0 (self)
+                                1110 LOAD_ATTR                5 (request_echo)
+                                1120 POP_JUMP_FORWARD_IF_FALSE    41 (to 1204)
+                     
+                      86        1122 LOAD_GLOBAL             13 (NULL + logger)
+                                1134 LOAD_ATTR                7 (info)
+                                1144 LOAD_FAST                0 (self)
+                                1146 LOAD_ATTR                8 (profile)
+                                1156 LOAD_ATTR                9 (id)
+                                1166 FORMAT_VALUE             0
+                                1168 LOAD_CONST              20 (' | Tried to retry ')
+                                1170 LOAD_GLOBAL              8 (RETRY_COUNT)
+                                1182 FORMAT_VALUE             0
+                                1184 LOAD_CONST              21 (' times. Nothing can do anymore :(')
+                                1186 BUILD_STRING             4
+                                1188 PRECALL                  1
+                                1192 CALL                     1
+                                1202 POP_TOP
                      
-                      86     >> 1166 LOAD_CONST               0 (None)
-                                1168 RETURN_VALUE
+                      87     >> 1204 LOAD_CONST               0 (None)
+                                1206 RETURN_VALUE
                      ExceptionTable:
-                       380 to 586 -> 594 [1]
-                       594 to 612 -> 1064 [2] lasti
-                       614 to 826 -> 1054 [2] lasti
-                       838 to 1040 -> 1054 [2] lasti
-                       1054 to 1062 -> 1064 [2] lasti
+                       380 to 624 -> 632 [1]
+                       632 to 650 -> 1102 [2] lasti
+                       652 to 864 -> 1092 [2] lasti
+                       876 to 1078 -> 1092 [2] lasti
+                       1092 to 1100 -> 1102 [2] lasti
                      consts
                         None
                         'method'
                         0
                         'url'
                         'unknown url'
-                        'delay'
+                        'retry_delay'
                         5
                         10
                         'retry_count'
                         ' | '
                         ' '
                         'follow_redirects'
                         ('profile_id', 'echo')
@@ -925,31 +939,31 @@
                         1
                         ' after '
                         ' seconds'
                         (400, 401, 403, 404, 500)
                         ' | Tried to retry '
                         ' times. Nothing can do anymore :('
                      names      ('get', 'pop', 'random', 'uniform', 'RETRY_COUNT', 'request_echo', 'logger', 'info', 'profile', 'id', 'range', 'raise_for_status', 'sleep', 'sleep_echo', 'RequestsError', 'code', 'warning', 'status_code')
-                     varnames   ('self', 'args', 'kwargs', 'method', 'url', 'delay', 'retry_count', 'data', 'i', 'response', 'e', 's')
+                     varnames   ('self', 'args', 'kwargs', 'method', 'url', 'retry_delay', 'retry_count', 'data', 'i', 'response', 'e', 's')
                      freevars   ('func',)
                      cellvars   ()
                      filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\utils\\profile_session.py'
                      name       'wrapper'
-                     firstlineno 55
+                     firstlineno 56
                      lnotab
-                        0x08013c012c01520136010e014c010401240102012a012a0128014e010e
+                        0x08013c012c01520136010e014c010401240102012a012a01280174010e
                         0112013601120140014e010a0112012801040240014e0114f4080e0e0152
                         01
                names      ('Any',)
                varnames   ('func', 'wrapper')
                freevars   ()
                cellvars   ('func',)
                filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\utils\\profile_session.py'
                name       'retry'
-               firstlineno 54
+               firstlineno 55
                lnotab 0x04011a21
             False
             30
             'method'
             'url'
             'params'
             'headers'
@@ -970,79 +984,79 @@
                   027c037c047c057c067c077c087c0aac01a6090000ab0900000000000000
                   00830064007b035600970386047d0b09007c0ba002000000000000000000
                   0000000000000000000000a6000000ab0000000000000000007d056e1723
                   007406000000000000000000002400720a01007c0b6a0400000000000000
                   007d0559006e0477007803590077017c0b7c0566025300
                              0 COPY_FREE_VARS           1
                
-                90           2 RETURN_GENERATOR
+                91           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                
-               104           8 LOAD_GLOBAL              1 (NULL + super)
+               105           8 LOAD_GLOBAL              1 (NULL + super)
                             20 PRECALL                  0
                             24 CALL                     0
                             34 LOAD_METHOD              1 (request)
                
-               105          56 LOAD_FAST                1 (method)
+               106          56 LOAD_FAST                1 (method)
                
-               106          58 LOAD_FAST                2 (url)
+               107          58 LOAD_FAST                2 (url)
                
-               107          60 LOAD_FAST                3 (params)
+               108          60 LOAD_FAST                3 (params)
                
-               108          62 LOAD_FAST                4 (headers)
+               109          62 LOAD_FAST                4 (headers)
                
-               109          64 LOAD_FAST                5 (data)
+               110          64 LOAD_FAST                5 (data)
                
-               110          66 LOAD_FAST                6 (json)
+               111          66 LOAD_FAST                6 (json)
                
-               111          68 LOAD_FAST                7 (follow_redirects)
+               112          68 LOAD_FAST                7 (follow_redirects)
                
-               112          70 LOAD_FAST                8 (verify)
+               113          70 LOAD_FAST                8 (verify)
                
-               113          72 LOAD_FAST               10 (timeout)
+               114          72 LOAD_FAST               10 (timeout)
                
-               104          74 KW_NAMES                 1
+               105          74 KW_NAMES                 1
                             76 PRECALL                  9
                             80 CALL                     9
                             90 GET_AWAITABLE            0
                             92 LOAD_CONST               0 (None)
                        >>   94 SEND                     3 (to 102)
                             96 YIELD_VALUE
                             98 RESUME                   3
                            100 JUMP_BACKWARD_NO_INTERRUPT     4 (to 94)
                        >>  102 STORE_FAST              11 (response)
                
-               115         104 NOP
+               116         104 NOP
                
-               116         106 LOAD_FAST               11 (response)
+               117         106 LOAD_FAST               11 (response)
                            108 LOAD_METHOD              2 (json)
                            130 PRECALL                  0
                            134 CALL                     0
                            144 STORE_FAST               5 (data)
                            146 JUMP_FORWARD            23 (to 194)
                        >>  148 PUSH_EXC_INFO
                
-               117         150 LOAD_GLOBAL              6 (JSONDecodeError)
+               118         150 LOAD_GLOBAL              6 (JSONDecodeError)
                            162 CHECK_EXC_MATCH
                            164 POP_JUMP_FORWARD_IF_FALSE    10 (to 186)
                            166 POP_TOP
                
-               118         168 LOAD_FAST               11 (response)
+               119         168 LOAD_FAST               11 (response)
                            170 LOAD_ATTR                4 (text)
                            180 STORE_FAST               5 (data)
                            182 POP_EXCEPT
                            184 JUMP_FORWARD             4 (to 194)
                
-               117     >>  186 RERAISE                  0
+               118     >>  186 RERAISE                  0
                        >>  188 COPY                     3
                            190 POP_EXCEPT
                            192 RERAISE                  1
                
-               119     >>  194 LOAD_FAST               11 (response)
+               120     >>  194 LOAD_FAST               11 (response)
                            196 LOAD_FAST                5 (data)
                            198 BUILD_TUPLE              2
                            200 RETURN_VALUE
                ExceptionTable:
                  106 to 144 -> 148 [0]
                  148 to 180 -> 188 [1] lasti
                  186 to 186 -> 188 [1] lasti
@@ -1051,15 +1065,15 @@
                   ('method', 'url', 'params', 'headers', 'data', 'json', 'allow_redirects', 'verify', 'timeout')
                names      ('super', 'request', 'json', 'JSONDecodeError', 'text')
                varnames   ('self', 'method', 'url', 'params', 'headers', 'data', 'json', 'follow_redirects', 'verify', 'retry_count', 'timeout', 'response')
                freevars   ('__class__',)
                cellvars   ()
                filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\utils\\profile_session.py'
                name       'request'
-               firstlineno 90
+               firstlineno 91
                lnotab
                   0x080e30010201020102010201020102010201020102f71e0b02012c0112
                   0112ff0802
             'HEAD'
             'GET'
             'POST'
             'PUT'
@@ -1071,15 +1085,15 @@
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'C:\\Users\\timer\\Code\\web3mt\\web3mt\\utils\\profile_session.py'
          name       'ProfileSession'
          firstlineno 21
          lnotab
-            0x0c0202010201020102010201020102010201020102f6060d1e0d060306
+            0x0c0202010201020102010201020102010201020102f6060d1e0e060306
             0310240205020102010201020102010201020102f5040202fe020302fd02
             0402fc020502fb020602fa020702f9020802f8020902f7020a02f6020b02
             f50aff0e01021e180118011801180118011801
       'ProfileSession'
    names      ('random', 'functools', 'partialmethod', 'json', 'JSONDecodeError', 'typing', 'Callable', 'Any', 'curl_cffi.requests', 'curl_cffi', 'AsyncSession', 'RequestsError', 'better_proxy', 'Proxy', 'web3db.models', 'Profile', 'web3db.utils', 'DEFAULT_UA', 'logger', 'sleeping', 'sleep', 'windows', 'set_windows_event_loop_policy', 'RETRY_COUNT', 'ProfileSession')
    varnames   ()
    freevars   ()
```

### Comparing `web3mt-0.0.1/web3mt/utils/__pycache__/reader.cpython-311.pyc` & `web3mt-0.0.2/web3mt/utils/__pycache__/reader.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `web3mt-0.0.1/web3mt/utils/__pycache__/sleeping.cpython-311.pyc` & `web3mt-0.0.2/web3mt/utils/__pycache__/sleeping.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `web3mt-0.0.1/web3mt/utils/__pycache__/windows.cpython-311.pyc` & `web3mt-0.0.2/web3mt/utils/__pycache__/windows.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `web3mt-0.0.1/web3mt/utils/logger.py` & `web3mt-0.0.2/web3mt/utils/logger.py`

 * *Files identical despite different names*

### Comparing `web3mt-0.0.1/web3mt/utils/profile_session.py` & `web3mt-0.0.2/web3mt/utils/profile_session.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,30 +3,29 @@
 from json import JSONDecodeError
 from typing import Callable, Any
 
 import curl_cffi.requests
 from curl_cffi.requests import AsyncSession, RequestsError
 from better_proxy import Proxy
 from web3db.models import Profile
-from web3db.utils import DEFAULT_UA
 
 from .logger import logger
 from .sleeping import sleep
 from .windows import set_windows_event_loop_policy
 
 set_windows_event_loop_policy()
 
 RETRY_COUNT = 5
 
 
 class ProfileSession(AsyncSession):
     DEFAULT_HEADERS = {
         "accept": "*/*",
         "accept-language": "en-US,en",
-        "user-agent": DEFAULT_UA,
+        "user-agent": 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36',
         "sec-ch-ua": '"Not_A Brand";v="8", "Chromium";v="120", "Google Chrome";v="120"',
         "sec-ch-ua-platform": '"Windows"',
         "sec-ch-ua-mobile": "?0",
         "sec-fetch-dest": "empty",
         "sec-fetch-mode": "cors",
         "sec-fetch-site": "same-origin",
         "connection": "keep-alive",
@@ -34,14 +33,15 @@
 
     def __init__(self, profile: Profile, sleep_echo: bool = True, requests_echo: bool = True, **kwargs) -> None:
         self.profile = profile
         self.sleep_echo = sleep_echo
         self.request_echo = requests_echo
         headers = kwargs.pop('headers', self.DEFAULT_HEADERS)
         impersonate = kwargs.pop('impersonate', curl_cffi.requests.BrowserType.chrome120)
+        self.log_info = f'{self.profile.id}'
         super().__init__(
             proxy=Proxy.from_str(proxy=profile.proxy.proxy_string).as_url,
             headers=headers,
             impersonate=impersonate,
             **kwargs
         )
 
@@ -51,38 +51,38 @@
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self.close()
 
     def retry(func: Callable) -> Callable:
         async def wrapper(self, *args, **kwargs) -> Any:
             method = kwargs.get('method', None) or args[0]
             url = kwargs.get('url', 'unknown url')
-            delay = kwargs.pop('delay', random.uniform(5, 10))
+            retry_delay = kwargs.pop('retry_delay', random.uniform(5, 10))
             retry_count = kwargs.pop('retry_count', RETRY_COUNT)
             if self.request_echo:
                 logger.info(f'{self.profile.id} | {method} {url}')
             data = None
             for i in range(retry_count):
                 try:
                     response, data = await func(self, *args, **kwargs)
                     if not kwargs.get('follow_redirects'):
                         response.raise_for_status()
-                    await sleep(delay, profile_id=self.profile.id, echo=self.sleep_echo)
+                    await sleep(random.uniform(5, 10), profile_id=self.profile.id, echo=self.sleep_echo)
                     return response, data
                 except RequestsError as e:
                     s = f'{self.profile.id} | {url} {e} {data if data is not None else ""}'
                     if e.code in (28, 35, 52, 56):
-                        logger.warning(f'{s} Retrying {i + 1} after {delay} seconds')
-                        await sleep(delay, profile_id=self.profile.id, echo=self.sleep_echo)
+                        logger.warning(f'{s} Retrying {i + 1} after {retry_delay} seconds')
+                        await sleep(retry_delay, profile_id=self.profile.id, echo=self.sleep_echo)
                         continue
                     elif response.status_code in [400, 401, 403, 404, 500]:
                         logger.warning(s)
                         raise e
                     else:
-                        logger.warning(f'{s} Retrying {i + 1} after {delay} seconds')
-                        await sleep(delay, profile_id=self.profile.id, echo=self.sleep_echo)
+                        logger.warning(f'{s} Retrying {i + 1} after {retry_delay} seconds')
+                        await sleep(retry_delay, profile_id=self.profile.id, echo=self.sleep_echo)
                         continue
             else:
                 if self.request_echo:
                     logger.info(f'{self.profile.id} | Tried to retry {RETRY_COUNT} times. Nothing can do anymore :(')
                 return None
 
         return wrapper
```

### Comparing `web3mt-0.0.1/PKG-INFO` & `web3mt-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: web3mt
-Version: 0.0.1
+Version: 0.0.2
 Summary: Web3 multitool
 Home-page: https://github.com/timertimertimer/web3mt
 Author: timertimertimer
 Author-email: timerkhan2002@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aptos-sdk (==0.7.1)
 Requires-Dist: better-proxy (>=1.1.5,<2.0.0)
 Requires-Dist: curl-cffi (>=0.6.2,<0.7.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: python-okx (>=0.2.8,<0.3.0)
-Requires-Dist: web3 (>=6.17.0,<7.0.0)
-Requires-Dist: web3db (>=1.0.0,<2.0.0)
+Requires-Dist: web3 (>=6.17.2,<7.0.0)
+Requires-Dist: web3db (>=1.0.2,<2.0.0)
 Project-URL: Repository, https://github.com/timertimertimer/web3mt
 Project-URL: Source, https://github.com/timertimertimer/web3mt
```

