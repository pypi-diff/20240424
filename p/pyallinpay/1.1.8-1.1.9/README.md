# Comparing `tmp/pyallinpay-1.1.8.tar.gz` & `tmp/pyallinpay-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyallinpay-1.1.8.tar", last modified: Tue Jun 23 10:04:21 2020, max compression
+gzip compressed data, was "dist\pyallinpay-1.1.9.tar", last modified: Wed Jun 30 04:32:32 2021, max compression
```

## Comparing `pyallinpay-1.1.8.tar` & `pyallinpay-1.1.9.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-23 10:04:21.000000 pyallinpay-1.1.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)       44 2020-06-23 10:04:03.000000 pyallinpay-1.1.8/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-23 10:04:21.000000 pyallinpay-1.1.8/pyallinpay.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1901 2020-06-23 10:04:21.000000 pyallinpay-1.1.8/pyallinpay.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-23 10:04:21.000000 pyallinpay-1.1.8/pyallinpay.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2020-06-23 10:04:21.000000 pyallinpay-1.1.8/pyallinpay.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-23 10:04:17.000000 pyallinpay-1.1.8/pyallinpay.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      715 2020-06-23 10:04:21.000000 pyallinpay-1.1.8/pyallinpay.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       47 2020-06-23 10:04:21.000000 pyallinpay-1.1.8/pyallinpay.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       46 2020-06-23 10:04:03.000000 pyallinpay-1.1.8/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1901 2020-06-23 10:04:21.000000 pyallinpay-1.1.8/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-23 10:04:21.000000 pyallinpay-1.1.8/allinpay/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-23 10:04:21.000000 pyallinpay-1.1.8/allinpay/client/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-23 10:04:21.000000 pyallinpay-1.1.8/allinpay/client/api/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2207 2020-06-23 10:04:03.000000 pyallinpay-1.1.8/allinpay/client/api/verify.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3276 2020-06-23 10:04:03.000000 pyallinpay-1.1.8/allinpay/client/api/gateway.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11104 2020-06-23 10:04:03.000000 pyallinpay-1.1.8/allinpay/client/api/unitorder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1370 2020-06-23 10:04:03.000000 pyallinpay-1.1.8/allinpay/client/api/trxfile.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3375 2020-06-23 10:04:03.000000 pyallinpay-1.1.8/allinpay/client/api/posol.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10453 2020-06-23 10:04:03.000000 pyallinpay-1.1.8/allinpay/client/api/qpay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3257 2020-06-23 10:04:03.000000 pyallinpay-1.1.8/allinpay/client/api/tranx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1124 2020-06-23 10:04:03.000000 pyallinpay-1.1.8/allinpay/client/api/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      377 2020-06-23 10:04:03.000000 pyallinpay-1.1.8/allinpay/client/api/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4669 2020-06-23 10:04:03.000000 pyallinpay-1.1.8/allinpay/client/api/prescanpay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6681 2020-06-23 10:04:03.000000 pyallinpay-1.1.8/allinpay/client/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2611 2020-06-23 10:04:03.000000 pyallinpay-1.1.8/allinpay/client/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-23 10:04:21.000000 pyallinpay-1.1.8/allinpay/core/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1775 2020-06-23 10:04:03.000000 pyallinpay-1.1.8/allinpay/core/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2302 2020-06-23 10:04:03.000000 pyallinpay-1.1.8/allinpay/core/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       83 2020-06-23 10:04:03.000000 pyallinpay-1.1.8/allinpay/core/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      176 2020-06-23 10:04:03.000000 pyallinpay-1.1.8/allinpay/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      126 2020-06-23 10:04:21.000000 pyallinpay-1.1.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      810 2020-06-23 10:04:03.000000 pyallinpay-1.1.8/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2333 2020-06-23 10:04:03.000000 pyallinpay-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-06-30 04:32:32.000000 pyallinpay-1.1.9/
+-rw-rw-rw-   0        0        0    35147 2019-12-17 08:05:24.000000 pyallinpay-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0       44 2019-11-06 10:17:03.000000 pyallinpay-1.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1954 2021-06-30 04:32:32.000000 pyallinpay-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      810 2019-11-06 09:48:03.000000 pyallinpay-1.1.9/README.rst
+drwxrwxrwx   0        0        0        0 2021-06-30 04:32:32.000000 pyallinpay-1.1.9/allinpay/
+-rw-rw-rw-   0        0        0      176 2021-06-30 04:29:44.000000 pyallinpay-1.1.9/allinpay/__init__.py
+drwxrwxrwx   0        0        0        0 2021-06-30 04:32:32.000000 pyallinpay-1.1.9/allinpay/client/
+-rw-rw-rw-   0        0        0     4824 2021-06-30 04:29:26.000000 pyallinpay-1.1.9/allinpay/client/__init__.py
+drwxrwxrwx   0        0        0        0 2021-06-30 04:32:32.000000 pyallinpay-1.1.9/allinpay/client/api/
+-rw-rw-rw-   0        0        0      377 2019-11-06 09:17:56.000000 pyallinpay-1.1.9/allinpay/client/api/__init__.py
+-rw-rw-rw-   0        0        0     1124 2019-12-17 06:40:34.000000 pyallinpay-1.1.9/allinpay/client/api/base.py
+-rw-rw-rw-   0        0        0     3276 2019-11-06 06:59:18.000000 pyallinpay-1.1.9/allinpay/client/api/gateway.py
+-rw-rw-rw-   0        0        0     3375 2019-12-17 06:40:18.000000 pyallinpay-1.1.9/allinpay/client/api/posol.py
+-rw-rw-rw-   0        0        0     4669 2019-11-06 07:13:23.000000 pyallinpay-1.1.9/allinpay/client/api/prescanpay.py
+-rw-rw-rw-   0        0        0    10453 2019-11-06 07:39:30.000000 pyallinpay-1.1.9/allinpay/client/api/qpay.py
+-rw-rw-rw-   0        0        0     3257 2019-11-20 10:57:13.000000 pyallinpay-1.1.9/allinpay/client/api/tranx.py
+-rw-rw-rw-   0        0        0     1370 2019-12-17 06:48:38.000000 pyallinpay-1.1.9/allinpay/client/api/trxfile.py
+-rw-rw-rw-   0        0        0    11104 2019-11-27 03:38:15.000000 pyallinpay-1.1.9/allinpay/client/api/unitorder.py
+-rw-rw-rw-   0        0        0     2207 2019-12-17 06:39:41.000000 pyallinpay-1.1.9/allinpay/client/api/verify.py
+-rw-rw-rw-   0        0        0     6681 2019-12-17 07:40:15.000000 pyallinpay-1.1.9/allinpay/client/base.py
+drwxrwxrwx   0        0        0        0 2021-06-30 04:32:32.000000 pyallinpay-1.1.9/allinpay/core/
+-rw-rw-rw-   0        0        0       83 2019-11-04 03:40:50.000000 pyallinpay-1.1.9/allinpay/core/__init__.py
+-rw-rw-rw-   0        0        0     1775 2019-11-04 03:43:10.000000 pyallinpay-1.1.9/allinpay/core/exceptions.py
+-rw-rw-rw-   0        0        0     4279 2021-06-30 04:29:26.000000 pyallinpay-1.1.9/allinpay/core/utils.py
+drwxrwxrwx   0        0        0        0 2021-06-30 04:32:32.000000 pyallinpay-1.1.9/pyallinpay.egg-info/
+-rw-rw-rw-   0        0        0     1954 2021-06-30 04:32:32.000000 pyallinpay-1.1.9/pyallinpay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      723 2021-06-30 04:32:32.000000 pyallinpay-1.1.9/pyallinpay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-06-30 04:32:32.000000 pyallinpay-1.1.9/pyallinpay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2019-11-06 08:05:12.000000 pyallinpay-1.1.9/pyallinpay.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       63 2021-06-30 04:32:32.000000 pyallinpay-1.1.9/pyallinpay.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2021-06-30 04:32:32.000000 pyallinpay-1.1.9/pyallinpay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       65 2021-06-30 04:29:26.000000 pyallinpay-1.1.9/requirements.txt
+-rw-rw-rw-   0        0        0      134 2021-06-30 04:32:32.000000 pyallinpay-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     2333 2021-06-30 04:29:44.000000 pyallinpay-1.1.9/setup.py
```

### Comparing `pyallinpay-1.1.8/pyallinpay.egg-info/PKG-INFO` & `pyallinpay-1.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-Metadata-Version: 1.1
-Name: pyallinpay
-Version: 1.1.8
-Summary: AllInPay SDK for Python
-Home-page: https://github.com/007gzs/pyallinpay
-Author: 007gzs
-Author-email: 007gzs@sina.com
-License: LGPL v3
-Description: #######################
-        AllInPay Sdk for Python
-        #######################
-        .. image:: https://travis-ci.org/007gzs/pyallinpay.svg?branch=master
-               :target: https://travis-ci.org/007gzs/pyallinpay
-        .. image:: https://img.shields.io/pypi/v/pyallinpay.svg
-               :target: https://pypi.org/project/pyallinpay
-        
-        通联支付 Python SDK。
-        `【阅读文档】 <http://pyallinpay.readthedocs.io/zh_CN/latest/>`_。
-        
-        ********
-        安装
-        ********
-        
-        目前 PyAllInPay 支持的 Python 环境有 2.7, 3.4, 3.5, 3.6, 3.7 和 pypy。
-        
-        为了简化安装过程，推荐使用 pip 进行安装
-        
-        .. code-block:: bash
-        
-            pip install pyallinpay
-        
-        升级 pyallinpay 到新版本::
-        
-            pip install -U pyallinpay
-        
-        如果需要安装 GitHub 上的最新代码::
-        
-            pip install https://github.com/007gzs/pyallinpay/archive/master.zip
-        
-        
-Keywords: pyallinpay,SDK,通联支付
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Metadata-Version: 1.1
+Name: pyallinpay
+Version: 1.1.9
+Summary: AllInPay SDK for Python
+Home-page: https://github.com/007gzs/pyallinpay
+Author: 007gzs
+Author-email: 007gzs@sina.com
+License: LGPL v3
+Description: #######################
+        AllInPay Sdk for Python
+        #######################
+        .. image:: https://travis-ci.org/007gzs/pyallinpay.svg?branch=master
+               :target: https://travis-ci.org/007gzs/pyallinpay
+        .. image:: https://img.shields.io/pypi/v/pyallinpay.svg
+               :target: https://pypi.org/project/pyallinpay
+        
+        通联支付 Python SDK。
+        `【阅读文档】 <http://pyallinpay.readthedocs.io/zh_CN/latest/>`_。
+        
+        ********
+        安装
+        ********
+        
+        目前 PyAllInPay 支持的 Python 环境有 2.7, 3.4, 3.5, 3.6, 3.7 和 pypy。
+        
+        为了简化安装过程，推荐使用 pip 进行安装
+        
+        .. code-block:: bash
+        
+            pip install pyallinpay
+        
+        升级 pyallinpay 到新版本::
+        
+            pip install -U pyallinpay
+        
+        如果需要安装 GitHub 上的最新代码::
+        
+            pip install https://github.com/007gzs/pyallinpay/archive/master.zip
+        
+        
+Keywords: pyallinpay,SDK,通联支付
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyallinpay-1.1.8/pyallinpay.egg-info/SOURCES.txt` & `pyallinpay-1.1.9/pyallinpay.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.rst
 requirements.txt
 setup.cfg
 setup.py
 allinpay/__init__.py
 allinpay/client/__init__.py
```

### Comparing `pyallinpay-1.1.8/PKG-INFO` & `pyallinpay-1.1.9/pyallinpay.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-Metadata-Version: 1.1
-Name: pyallinpay
-Version: 1.1.8
-Summary: AllInPay SDK for Python
-Home-page: https://github.com/007gzs/pyallinpay
-Author: 007gzs
-Author-email: 007gzs@sina.com
-License: LGPL v3
-Description: #######################
-        AllInPay Sdk for Python
-        #######################
-        .. image:: https://travis-ci.org/007gzs/pyallinpay.svg?branch=master
-               :target: https://travis-ci.org/007gzs/pyallinpay
-        .. image:: https://img.shields.io/pypi/v/pyallinpay.svg
-               :target: https://pypi.org/project/pyallinpay
-        
-        通联支付 Python SDK。
-        `【阅读文档】 <http://pyallinpay.readthedocs.io/zh_CN/latest/>`_。
-        
-        ********
-        安装
-        ********
-        
-        目前 PyAllInPay 支持的 Python 环境有 2.7, 3.4, 3.5, 3.6, 3.7 和 pypy。
-        
-        为了简化安装过程，推荐使用 pip 进行安装
-        
-        .. code-block:: bash
-        
-            pip install pyallinpay
-        
-        升级 pyallinpay 到新版本::
-        
-            pip install -U pyallinpay
-        
-        如果需要安装 GitHub 上的最新代码::
-        
-            pip install https://github.com/007gzs/pyallinpay/archive/master.zip
-        
-        
-Keywords: pyallinpay,SDK,通联支付
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Metadata-Version: 1.1
+Name: pyallinpay
+Version: 1.1.9
+Summary: AllInPay SDK for Python
+Home-page: https://github.com/007gzs/pyallinpay
+Author: 007gzs
+Author-email: 007gzs@sina.com
+License: LGPL v3
+Description: #######################
+        AllInPay Sdk for Python
+        #######################
+        .. image:: https://travis-ci.org/007gzs/pyallinpay.svg?branch=master
+               :target: https://travis-ci.org/007gzs/pyallinpay
+        .. image:: https://img.shields.io/pypi/v/pyallinpay.svg
+               :target: https://pypi.org/project/pyallinpay
+        
+        通联支付 Python SDK。
+        `【阅读文档】 <http://pyallinpay.readthedocs.io/zh_CN/latest/>`_。
+        
+        ********
+        安装
+        ********
+        
+        目前 PyAllInPay 支持的 Python 环境有 2.7, 3.4, 3.5, 3.6, 3.7 和 pypy。
+        
+        为了简化安装过程，推荐使用 pip 进行安装
+        
+        .. code-block:: bash
+        
+            pip install pyallinpay
+        
+        升级 pyallinpay 到新版本::
+        
+            pip install -U pyallinpay
+        
+        如果需要安装 GitHub 上的最新代码::
+        
+            pip install https://github.com/007gzs/pyallinpay/archive/master.zip
+        
+        
+Keywords: pyallinpay,SDK,通联支付
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyallinpay-1.1.8/allinpay/client/api/verify.py` & `pyallinpay-1.1.9/allinpay/client/api/verify.py`

 * *Files identical despite different names*

### Comparing `pyallinpay-1.1.8/allinpay/client/api/gateway.py` & `pyallinpay-1.1.9/allinpay/client/api/gateway.py`

 * *Files identical despite different names*

### Comparing `pyallinpay-1.1.8/allinpay/client/api/unitorder.py` & `pyallinpay-1.1.9/allinpay/client/api/unitorder.py`

 * *Files identical despite different names*

### Comparing `pyallinpay-1.1.8/allinpay/client/api/trxfile.py` & `pyallinpay-1.1.9/allinpay/client/api/trxfile.py`

 * *Files identical despite different names*

### Comparing `pyallinpay-1.1.8/allinpay/client/api/posol.py` & `pyallinpay-1.1.9/allinpay/client/api/posol.py`

 * *Files identical despite different names*

### Comparing `pyallinpay-1.1.8/allinpay/client/api/qpay.py` & `pyallinpay-1.1.9/allinpay/client/api/qpay.py`

 * *Files identical despite different names*

### Comparing `pyallinpay-1.1.8/allinpay/client/api/tranx.py` & `pyallinpay-1.1.9/allinpay/client/api/tranx.py`

 * *Files identical despite different names*

### Comparing `pyallinpay-1.1.8/allinpay/client/api/base.py` & `pyallinpay-1.1.9/allinpay/client/api/base.py`

 * *Files identical despite different names*

### Comparing `pyallinpay-1.1.8/allinpay/client/api/prescanpay.py` & `pyallinpay-1.1.9/allinpay/client/api/prescanpay.py`

 * *Files identical despite different names*

### Comparing `pyallinpay-1.1.8/allinpay/client/base.py` & `pyallinpay-1.1.9/allinpay/client/base.py`

 * *Files identical despite different names*

### Comparing `pyallinpay-1.1.8/allinpay/core/exceptions.py` & `pyallinpay-1.1.9/allinpay/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyallinpay-1.1.8/README.rst` & `pyallinpay-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyallinpay-1.1.8/setup.py` & `pyallinpay-1.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     long_description = f.read()
 
 with open('requirements.txt') as f:
     requirements = [line for line in f.read().splitlines() if line]
 
 setup(
     name='pyallinpay',
-    version='1.1.8',
+    version='1.1.9',
     keywords='pyallinpay, SDK, 通联支付',
     description='AllInPay SDK for Python',
     long_description=long_description,
     url='https://github.com/007gzs/pyallinpay',
     author='007gzs',
     author_email='007gzs@sina.com',
     license='LGPL v3',
```

