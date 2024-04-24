# Comparing `tmp/atomcache-0.7.5.tar.gz` & `tmp/atomcache-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomcache-0.7.5.tar", max compression
+gzip compressed data, was "atomcache-0.7.6.tar", max compression
```

## Comparing `atomcache-0.7.5.tar` & `atomcache-0.7.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2021-10-31 14:30:27.194665 atomcache-0.7.5/LICENSE
--rw-r--r--   0        0        0     4164 2022-12-02 13:52:44.271882 atomcache-0.7.5/README.md
--rw-r--r--   0        0        0      160 2023-07-11 07:39:04.603650 atomcache-0.7.5/atomcache/__init__.py
--rw-r--r--   0        0        0     1421 2023-06-30 10:06:30.127745 atomcache-0.7.5/atomcache/backend.py
--rw-r--r--   0        0        0    10144 2023-07-11 07:38:24.711125 atomcache-0.7.5/atomcache/base.py
--rw-r--r--   0        0        0        0 2022-03-11 07:33:27.689230 atomcache-0.7.5/atomcache/py.typed
--rw-r--r--   0        0        0     4962 2023-06-30 10:06:30.130746 atomcache-0.7.5/atomcache/redis.py
--rw-r--r--   0        0        0      951 2023-07-11 07:39:10.887890 atomcache-0.7.5/pyproject.toml
--rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 atomcache-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2021-10-31 14:30:27.194665 atomcache-0.7.6/LICENSE
+-rw-r--r--   0        0        0     4164 2022-12-02 13:52:44.271882 atomcache-0.7.6/README.md
+-rw-r--r--   0        0        0      160 2024-04-24 10:33:59.783011 atomcache-0.7.6/atomcache/__init__.py
+-rw-r--r--   0        0        0     1421 2023-06-30 10:06:30.127745 atomcache-0.7.6/atomcache/backend.py
+-rw-r--r--   0        0        0    10144 2023-07-11 07:38:24.711125 atomcache-0.7.6/atomcache/base.py
+-rw-r--r--   0        0        0        0 2022-03-11 07:33:27.689230 atomcache-0.7.6/atomcache/py.typed
+-rw-r--r--   0        0        0     5050 2024-04-24 10:32:26.240170 atomcache-0.7.6/atomcache/redis.py
+-rw-r--r--   0        0        0      951 2024-04-24 10:33:55.290880 atomcache-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0     4978 1970-01-01 00:00:00.000000 atomcache-0.7.6/PKG-INFO
```

### Comparing `atomcache-0.7.5/LICENSE` & `atomcache-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `atomcache-0.7.5/README.md` & `atomcache-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `atomcache-0.7.5/atomcache/backend.py` & `atomcache-0.7.6/atomcache/backend.py`

 * *Files identical despite different names*

### Comparing `atomcache-0.7.5/atomcache/base.py` & `atomcache-0.7.6/atomcache/base.py`

 * *Files identical despite different names*

### Comparing `atomcache-0.7.5/atomcache/redis.py` & `atomcache-0.7.6/atomcache/redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,28 +30,30 @@
             Redis: Client from connection pool
         """
         return self._redis
 
     def lock_key(self, key: str) -> str:
         return f"{key}{self.lock_name}"
 
-    async def get(
+    async def get(  # noqa: WPS212
         self,
         key: KeyT,
         default: VT = None,
         timeout: int = DEFAULT_LOCK_TIMEOUT,
         with_lock: bool = True,
         lockspace: Optional[str] = None,
     ) -> Tuple[VT, TTL]:
         async with self._redis.pipeline() as pipe:
             pipe.get(key)
             pipe.ttl(key)
             if not with_lock:
                 cached_value, ttl = await pipe.execute()
-                return cached_value.decode() or default, ttl
+                if cached_value is None:
+                    return default, ttl
+                return cached_value.decode(), ttl
             lock_name = self.lock_key(lockspace) if lockspace else self.lock_key(key)
             pipe.get(lock_name)
             cached_value, ttl, lock = await pipe.execute()
 
             if cached_value:
                 return cached_value.decode(), ttl
```

### Comparing `atomcache-0.7.5/pyproject.toml` & `atomcache-0.7.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atomcache"
-version = "0.7.5"
+version = "0.7.6"
 description = "Asynchronous cache manager designed for horizontally scaled web applications."
 authors = ["Serghei Ungurean <srg@intelbit.io>", "Nichita Morcotilo <nmorkotilo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pysergio/atomcache"
 repository = "https://github.com/pysergio/atomcache"
```

### Comparing `atomcache-0.7.5/PKG-INFO` & `atomcache-0.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: atomcache
-Version: 0.7.5
+Version: 0.7.6
 Summary: Asynchronous cache manager designed for horizontally scaled web applications.
 Home-page: https://github.com/pysergio/atomcache
 License: MIT
 Author: Serghei Ungurean
 Author-email: srg@intelbit.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fastapi (>=0.61.2)
 Requires-Dist: redis (>=4.5.4,<5.0.0)
 Project-URL: Repository, https://github.com/pysergio/atomcache
 Description-Content-Type: text/markdown
 
 <p align="center">
 <a href="https://codecov.io/gh/pysergio/atomcache">
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1 Name: atomcache Version: 0.7.5 Summary: Asynchronous
+Metadata-Version: 2.1 Name: atomcache Version: 0.7.6 Summary: Asynchronous
 cache manager designed for horizontally scaled web applications. Home-page:
 https://github.com/pysergio/atomcache License: MIT Author: Serghei Ungurean
 Author-email: srg@intelbit.io Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: fastapi
-(>=0.61.2) Requires-Dist: redis (>=4.5.4,<5.0.0) Project-URL: Repository,
-https://github.com/pysergio/atomcache Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Requires-Dist: fastapi (>=0.61.2) Requires-Dist:
+redis (>=4.5.4,<5.0.0) Project-URL: Repository, https://github.com/pysergio/
+atomcache Description-Content-Type: text/markdown
         _[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_p_y_s_e_r_g_i_o_/_a_t_o_m_c_a_c_h_e_/_b_r_a_n_c_h_/_m_a_s_t_e_r_/_g_r_a_p_h_/
     _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_O_V_Z_A_B_B_E_1_U_J_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
 ## Introduction Asynchronous cache manager designed for horizontally scaled web
 applications. **NOTE:** _Currently has implementation only for FastAPI using
 Redis._ ## Requirements Python 3.7+ * _r_e_d_i_s for cache implementation. * _F_a_s_t_A_P_I
 for the web parts. ## Installation
 ```console $ pip install atomcache ---> 100% ``` ## Explanation schema ![Class
```

