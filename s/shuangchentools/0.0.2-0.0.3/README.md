# Comparing `tmp/shuangchentools-0.0.2.tar.gz` & `tmp/shuangchentools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shuangchentools-0.0.2.tar", last modified: Mon Mar 25 02:59:41 2024, max compression
+gzip compressed data, was "shuangchentools-0.0.3.tar", last modified: Wed Apr 24 06:28:17 2024, max compression
```

## Comparing `shuangchentools-0.0.2.tar` & `shuangchentools-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 02:59:41.805841 shuangchentools-0.0.2/
--rw-rw-rw-   0        0        0      834 2024-03-25 02:59:41.804842 shuangchentools-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      573 2024-03-25 02:02:16.000000 shuangchentools-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-03-25 02:59:41.805841 shuangchentools-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      582 2024-03-25 02:49:03.000000 shuangchentools-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-25 02:59:41.786318 shuangchentools-0.0.2/shuangchentools/
--rw-rw-rw-   0        0        0       64 2024-03-13 10:53:27.000000 shuangchentools-0.0.2/shuangchentools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 02:59:41.796318 shuangchentools-0.0.2/shuangchentools/doc_segment/
--rw-rw-rw-   0        0        0       51 2024-03-12 12:56:11.000000 shuangchentools-0.0.2/shuangchentools/doc_segment/__init__.py
--rw-rw-rw-   0        0        0     7037 2024-03-23 10:25:14.000000 shuangchentools-0.0.2/shuangchentools/doc_segment/doc_segment_by_rule.py
-drwxrwxrwx   0        0        0        0 2024-03-25 02:59:41.799319 shuangchentools-0.0.2/shuangchentools/spider/
--rw-rw-rw-   0        0        0       38 2024-03-12 11:09:07.000000 shuangchentools-0.0.2/shuangchentools/spider/__init__.py
--rw-rw-rw-   0        0        0     3012 2024-03-13 03:21:23.000000 shuangchentools-0.0.2/shuangchentools/spider/selenium.py
-drwxrwxrwx   0        0        0        0 2024-03-25 02:59:41.803825 shuangchentools-0.0.2/shuangchentools/utils/
--rw-rw-rw-   0        0        0       47 2024-03-25 02:48:24.000000 shuangchentools-0.0.2/shuangchentools/utils/__init__.py
--rw-rw-rw-   0        0        0     1570 2024-03-25 02:48:42.000000 shuangchentools-0.0.2/shuangchentools/utils/decorators.py
--rw-rw-rw-   0        0        0     3437 2024-03-13 08:53:59.000000 shuangchentools-0.0.2/shuangchentools/utils/transform.py
-drwxrwxrwx   0        0        0        0 2024-03-25 02:59:41.794319 shuangchentools-0.0.2/shuangchentools.egg-info/
--rw-rw-rw-   0        0        0      834 2024-03-25 02:59:41.000000 shuangchentools-0.0.2/shuangchentools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      506 2024-03-25 02:59:41.000000 shuangchentools-0.0.2/shuangchentools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 02:59:41.000000 shuangchentools-0.0.2/shuangchentools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-03-25 02:59:41.000000 shuangchentools-0.0.2/shuangchentools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-03-25 02:59:41.000000 shuangchentools-0.0.2/shuangchentools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 06:28:17.936745 shuangchentools-0.0.3/
+-rw-rw-rw-   0        0        0      842 2024-04-24 06:28:17.935733 shuangchentools-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      573 2024-03-25 02:02:16.000000 shuangchentools-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 06:28:17.936745 shuangchentools-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      590 2024-04-24 05:31:40.000000 shuangchentools-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 06:28:17.922572 shuangchentools-0.0.3/shuangchentools/
+-rw-rw-rw-   0        0        0       64 2024-03-13 10:53:27.000000 shuangchentools-0.0.3/shuangchentools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 06:28:17.929601 shuangchentools-0.0.3/shuangchentools/doc_segment/
+-rw-rw-rw-   0        0        0       51 2024-03-12 12:56:11.000000 shuangchentools-0.0.3/shuangchentools/doc_segment/__init__.py
+-rw-rw-rw-   0        0        0     7036 2024-04-19 11:18:34.000000 shuangchentools-0.0.3/shuangchentools/doc_segment/doc_segment_by_rule.py
+drwxrwxrwx   0        0        0        0 2024-04-24 06:28:17.932119 shuangchentools-0.0.3/shuangchentools/spider/
+-rw-rw-rw-   0        0        0       38 2024-03-12 11:09:07.000000 shuangchentools-0.0.3/shuangchentools/spider/__init__.py
+-rw-rw-rw-   0        0        0     3119 2024-04-24 06:26:59.000000 shuangchentools-0.0.3/shuangchentools/spider/selenium.py
+drwxrwxrwx   0        0        0        0 2024-04-24 06:28:17.935733 shuangchentools-0.0.3/shuangchentools/utils/
+-rw-rw-rw-   0        0        0       47 2024-03-25 02:48:24.000000 shuangchentools-0.0.3/shuangchentools/utils/__init__.py
+-rw-rw-rw-   0        0        0     1569 2024-04-19 11:18:23.000000 shuangchentools-0.0.3/shuangchentools/utils/decorators.py
+-rw-rw-rw-   0        0        0     3405 2024-04-19 11:24:59.000000 shuangchentools-0.0.3/shuangchentools/utils/transform.py
+drwxrwxrwx   0        0        0        0 2024-04-24 06:28:17.927496 shuangchentools-0.0.3/shuangchentools.egg-info/
+-rw-rw-rw-   0        0        0      842 2024-04-24 06:28:17.000000 shuangchentools-0.0.3/shuangchentools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2024-04-24 06:28:17.000000 shuangchentools-0.0.3/shuangchentools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 06:28:17.000000 shuangchentools-0.0.3/shuangchentools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-24 06:28:17.000000 shuangchentools-0.0.3/shuangchentools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-24 06:28:17.000000 shuangchentools-0.0.3/shuangchentools.egg-info/top_level.txt
```

### Comparing `shuangchentools-0.0.2/PKG-INFO` & `shuangchentools-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: shuangchentools
-Version: 0.0.2
+Version: 0.0.3
 Summary: encapsulated some commonly used tools
-Home-page: https://github.com/wangtao2001/sctools
+Home-page: https://github.com/wangtao2001/shuangchentools
 Author: shuangchen
 Author-email: wangtao.cpu@gmail.com
 Description-Content-Type: text/markdown
 
 <p align="center">
 <img src="assets/icon.png" width="200"  alt="">
 </p>
```

### Comparing `shuangchentools-0.0.2/README.md` & `shuangchentools-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `shuangchentools-0.0.2/setup.py` & `shuangchentools-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='shuangchentools',
-    version='0.0.2',
+    version='0.0.3',
     author='shuangchen',
     author_email='wangtao.cpu@gmail.com',
     description='encapsulated some commonly used tools',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/wangtao2001/sctools',
+    url='https://github.com/wangtao2001/shuangchentools',
     packages=setuptools.find_packages(),
     install_requires=[
         'selenium>=4.15.2',
         'requests>=2.31.0'
     ]
 )
```

### Comparing `shuangchentools-0.0.2/shuangchentools/doc_segment/doc_segment_by_rule.py` & `shuangchentools-0.0.3/shuangchentools/doc_segment/doc_segment_by_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 @Author: shuangchen
-@Time：2024/3/12
+@Time: 2024/3/12
 @File: doc_segment_by_rule.py
 @Description: 通过规则分割文档
 """
 
 import re
```

### Comparing `shuangchentools-0.0.2/shuangchentools/spider/selenium.py` & `shuangchentools-0.0.3/shuangchentools/spider/selenium.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,36 +12,39 @@
 
 
 class PageNotFound(Exception):
     pass
 
 
 class SeleniumSpider:
-    def __init__(self, url: str, cookies: str = '') -> None:
+    def __init__(self, url: str, cookies: str = '', headless: bool = True) -> None:
         """
         :param url: 网页链接
         :param cookies: 全局的cookies值
+        :param headless: 无头模式
         """
         self.base_url = url
         self.headers = {
             'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/119.0.0.0 Safari/537.36',
             'Cookie': cookies
         }
+        self.headless = headless
         self.chrome_path = r'C:\ChromeAutomationProfile'
         if not os.path.exists(self.chrome_path):
             os.mkdir(self.chrome_path)
 
     def _get_client_cookies(self) -> None:
         """
         获取客户端的cookies
         :return: None
         """
         os.system(f'start chrome --remote-debugging-port=9527 --user-data-dir="{self.chrome_path}"')
         options = Options()
-        options.add_argument('--headless')
+        if self.headless:
+            options.add_argument('--headless')
         options.add_experimental_option("debuggerAddress", "127.0.0.1:9527")
         chrome = webdriver.Chrome(options=options)
         chrome.get(self.base_url)
         chrome.refresh()
         cookies = ''
         for c in chrome.get_cookies():
             cookies += f'{c["name"]}={c["value"]};'
@@ -58,15 +61,15 @@
         try:
             r = requests.get(url, headers=self.headers)
         except requests.exceptions.ConnectTimeout:
             raise PageNotFound('网页不存在: ' + url)
         else:
             if r.status_code == 412 or r.status_code == 202:
                 self._get_client_cookies()
-                return self.get_html(url)
+                raise
             elif r.status_code == 404 or r.status_code == 500:
                 raise PageNotFound('网页不存在: ' + url)
             r.encoding = 'utf-8'
             return r.text
 
     def get_content(self, url=None) -> bytes:
         """
```

### Comparing `shuangchentools-0.0.2/shuangchentools/utils/decorators.py` & `shuangchentools-0.0.3/shuangchentools/utils/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 @Author: shuangchen
-@Time：2024/3/25
+@Time: 2024/3/25
 @File: decorators.py
 @Description: 常用装饰器
 """
 
 import time
 import functools
 from typing import Callable, Any
```

### Comparing `shuangchentools-0.0.2/shuangchentools/utils/transform.py` & `shuangchentools-0.0.3/shuangchentools/utils/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
 @Author: shuangchen
-@Time：2024/3/12
+@Time: 2024/3/12
 @File: transform.py
 @Description: 各类转换工具函数
 """
 
-NUMBER_TOO_LONG_ERR_MSG = '数字最大99999'
-
 
 def numeral2chinese(number: int) -> str:
     """
     阿拉伯数字转中文表达
     :param number: 待转换的数字
     """
-    assert number <= 99999, NUMBER_TOO_LONG_ERR_MSG
+    if number > 99999:
+        raise ValueError('数字最大99999')
     num_dict = {1: '一', 2: '二', 3: '三', 4: '四', 5: '五', 6: '六', 7: '七', 8: '八', 9: '九', 0: '零'}
     digit_dict = {1: '十', 2: '百', 3: '千', 4: '万'}
 
     def max_digit(number, count):
         num = number // 10  # 整除
         if num != 0:
             return max_digit(num, count + 1)
```

### Comparing `shuangchentools-0.0.2/shuangchentools.egg-info/PKG-INFO` & `shuangchentools-0.0.3/shuangchentools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: shuangchentools
-Version: 0.0.2
+Version: 0.0.3
 Summary: encapsulated some commonly used tools
-Home-page: https://github.com/wangtao2001/sctools
+Home-page: https://github.com/wangtao2001/shuangchentools
 Author: shuangchen
 Author-email: wangtao.cpu@gmail.com
 Description-Content-Type: text/markdown
 
 <p align="center">
 <img src="assets/icon.png" width="200"  alt="">
 </p>
```

