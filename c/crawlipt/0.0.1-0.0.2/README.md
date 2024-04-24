# Comparing `tmp/crawlipt-0.0.1.tar.gz` & `tmp/crawlipt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlipt-0.0.1.tar", last modified: Fri Apr 19 08:51:07 2024, max compression
+gzip compressed data, was "crawlipt-0.0.2.tar", last modified: Wed Apr 24 04:13:45 2024, max compression
```

## Comparing `crawlipt-0.0.1.tar` & `crawlipt-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:51:07.649433 crawlipt-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-19 08:51:03.000000 crawlipt-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 08:51:03.000000 crawlipt-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-19 08:51:07.649433 crawlipt-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-19 08:51:03.000000 crawlipt-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:51:07.645433 crawlipt-0.0.1/crawlipt/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-19 08:51:03.000000 crawlipt-0.0.1/crawlipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-19 08:51:03.000000 crawlipt-0.0.1/crawlipt/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-19 08:51:03.000000 crawlipt-0.0.1/crawlipt/action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:51:07.649433 crawlipt-0.0.1/crawlipt/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-19 08:51:03.000000 crawlipt-0.0.1/crawlipt/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-19 08:51:03.000000 crawlipt-0.0.1/crawlipt/actions/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-19 08:51:03.000000 crawlipt-0.0.1/crawlipt/actions/input.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-19 08:51:03.000000 crawlipt-0.0.1/crawlipt/actions/redirect.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-19 08:51:03.000000 crawlipt-0.0.1/crawlipt/actions/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-19 08:51:03.000000 crawlipt-0.0.1/crawlipt/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-19 08:51:03.000000 crawlipt-0.0.1/crawlipt/script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:51:07.649433 crawlipt-0.0.1/crawlipt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-19 08:51:07.000000 crawlipt-0.0.1/crawlipt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-19 08:51:07.000000 crawlipt-0.0.1/crawlipt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:51:07.000000 crawlipt-0.0.1/crawlipt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 08:51:07.000000 crawlipt-0.0.1/crawlipt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 08:51:07.000000 crawlipt-0.0.1/crawlipt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 08:51:07.649433 crawlipt-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-19 08:51:03.000000 crawlipt-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:13:45.725271 crawlipt-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-24 04:13:39.000000 crawlipt-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 04:13:39.000000 crawlipt-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-24 04:13:45.725271 crawlipt-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-24 04:13:39.000000 crawlipt-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:13:45.721271 crawlipt-0.0.2/crawlipt/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:13:45.725271 crawlipt-0.0.2/crawlipt/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/actions/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/actions/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/actions/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/actions/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/actions/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/actions/slide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/actions/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:13:45.725271 crawlipt-0.0.2/crawlipt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-24 04:13:45.000000 crawlipt-0.0.2/crawlipt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-24 04:13:45.000000 crawlipt-0.0.2/crawlipt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 04:13:45.000000 crawlipt-0.0.2/crawlipt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-24 04:13:45.000000 crawlipt-0.0.2/crawlipt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 04:13:45.000000 crawlipt-0.0.2/crawlipt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 04:13:45.725271 crawlipt-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-24 04:13:39.000000 crawlipt-0.0.2/setup.py
```

### Comparing `crawlipt-0.0.1/LICENSE` & `crawlipt-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.1/PKG-INFO` & `crawlipt-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: crawlipt
-Version: 0.0.1
+Version: 0.0.2
 Summary: The script for selenium in python
 Home-page: https://github.com/WwwwwyDev/crawlipt
 Author: WwwwwyDev
-Author-email: me@example.com
+Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: selenium>=4.0.0
 Requires-Dist: ddddocr
+Requires-Dist: webdriver-manager
 
 
 <!-- markdownlint-disable MD033 MD041 -->
 <p align="center">
   <a href="https://github.com/WwwwwyDev/crawlipt"><img src="https://s2.loli.net/2024/04/19/1T7sZdrjbEfci8W.png" alt="crawlist" style="width:254px; height:208px" ></a>
 </p>
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: crawlipt Version: 0.0.1 Summary: The script for
+Metadata-Version: 2.1 Name: crawlipt Version: 0.0.2 Summary: The script for
 selenium in python Home-page: https://github.com/WwwwwyDev/crawlipt Author:
-WwwwwyDev Author-email: me@example.com License: MIT Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
-Python: >=3.10.0 Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: selenium>=4.0.0 Requires-Dist: ddddocr
+WwwwwyDev Author-email: wwy20001014@foxmail.com License: MIT Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python ::
+Implementation :: CPython Classifier: Programming Language :: Python ::
+Implementation :: PyPy Requires-Python: >=3.10.0 Description-Content-Type:
+text/markdown License-File: LICENSE Requires-Dist: selenium>=4.0.0 Requires-
+Dist: ddddocr Requires-Dist: webdriver-manager
                                   _[_c_r_a_w_l_i_s_t_]
                  # crawlipt The script for selenium in python
                          _[_p_y_p_i_][python]_[_G_i_t_H_u_b_ _s_t_a_r_s_]
 ## introduction You can use Crawlipt to driver the selenium by script in
 python.The script adopts JSON format for better cross language operations and
 physical storage. ## installing You can use pip or pip3 to install the
 crawlist\ `pip install crawlipt` or `pip3 install crawlipt` ## quickly start
```

### Comparing `crawlipt-0.0.1/README.md` & `crawlipt-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.1/crawlipt/actions/click.py` & `crawlipt-0.0.2/crawlipt/actions/slide.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.remote.webdriver import WebDriver
-from selenium.webdriver.support.wait import WebDriverWait
-
+from selenium.webdriver.common.action_chains import ActionChains
 from crawlipt.annotation import check
 
 
-class Click:
+class Slide:
     @staticmethod
     @check(exclude="driver")
-    def click(driver: WebDriver, xpath: str,) -> None:
+    def slide(driver: WebDriver, xpath: str, position: list) -> None:
         """
         Handling click events
         :param driver: selenium webdriver
-        :param xpath: click on the xpath path of the button
+        :param xpath: The element to be slid
+        :param position: The x, y position
         """
-        WebDriverWait(driver, 2).until(EC.presence_of_element_located((By.XPATH, xpath)))
-        element = driver.find_element(By.XPATH, xpath)
-        driver.execute_script("arguments[0].click();", element)
+        assert len(position) == 2
+        slider = driver.find_element(By.XPATH, xpath)
+        x, y = position
+        start_x = slider.location["x"]
+        end_x = start_x + x
+        distance_x = end_x - start_x
+        start_y = slider.location["y"]
+        end_y = start_y + y
+        distance_y = end_y - start_y
+        action_chains = ActionChains(driver)
+        action_chains.click_and_hold(slider).move_by_offset(distance_x, distance_y).release().perform()
```

### Comparing `crawlipt-0.0.1/crawlipt/actions/input.py` & `crawlipt-0.0.2/crawlipt/actions/switch.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,48 @@
-from selenium.webdriver import Keys
 from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.remote.webdriver import WebDriver
-from selenium.webdriver.support.wait import WebDriverWait
-
 from crawlipt.annotation import check
 
 
-class Input:
+class Switch:
+    @staticmethod
+    @check(exclude="driver")
+    def switchLastTab(driver: WebDriver) -> None:
+        """
+        Switch to the last handle
+        :param driver: selenium webdriver
+        """
+        window_handles = driver.window_handles
+        driver.switch_to.window(window_handles[-1])
+
+    @staticmethod
+    @check(exclude="driver")
+    def switchTab(driver: WebDriver, index: int | str) -> None:
+        """
+        Switch to the index handle
+        :param driver: selenium webdriver
+        :param index: The index handle
+        """
+        if isinstance(index, str):
+            index = int(index)
+        window_handles = driver.window_handles
+        driver.switch_to.window(window_handles[index])
+
     @staticmethod
     @check(exclude="driver")
-    def input(driver: WebDriver, xpath: str, keyword: str) -> None:
+    def switchToframe(driver: WebDriver, xpath: str) -> None:
         """
-        Handling keyboard input events
+        Switch to the inner frame
         :param driver: selenium webdriver
-        :param xpath: The xpath path of the input box
-        :param keyword: keyword needs to be passed in
+        :param xpath: The xpath of frame
         """
-        WebDriverWait(driver, 2).until(EC.presence_of_element_located((By.XPATH, xpath)))
-        element = driver.find_element(By.XPATH, xpath)
-        element.send_keys(keyword)
+        frame = driver.find_element(By.XPATH, xpath)
+        driver.switch_to.frame(frame)
 
     @staticmethod
     @check(exclude="driver")
-    def enter(driver: WebDriver, xpath: str) -> None:
+    def switchOutFrame(driver: WebDriver) -> None:
         """
-        Press the enter key once
+        Switch to the outer frame
         :param driver: selenium webdriver
-        :param xpath: The xpath path of the input box
-        :return: Whether successful
         """
-        WebDriverWait(driver, 2).until(EC.presence_of_element_located((By.XPATH, xpath)))
-        element = driver.find_element(By.XPATH, xpath)
-        element.send_keys(Keys.RETURN)
+        driver.switch_to.parent_frame()
```

### Comparing `crawlipt-0.0.1/crawlipt/actions/redirect.py` & `crawlipt-0.0.2/crawlipt/actions/redirect.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.1/crawlipt/annotation.py` & `crawlipt-0.0.2/crawlipt/annotation.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,16 @@
                     continue
                 if type_.annotation == type_.empty:
                     raise ParamTypeError(f"Parameter {name} must be indicated the type.")
                 if name not in all_kwargs:
                     raise ParamTypeError(f"Parameter {name} is not in the defined parameter list.")
                 if all_kwargs[name] is None and type_.default is not type_.empty:
                     continue
+                if all_kwargs[name] == "__PRE_RETURN__":
+                    continue
                 if isinstance(all_kwargs[name], int) and type_.annotation is float:
                     all_kwargs[name] = float(all_kwargs.get(name))
                 if not isinstance(all_kwargs[name], type_.annotation):
                     raise ParamTypeError(f"Parameter {name} must be {type_.annotation}.")
             return func(*args, **kwargs)
 
         return inner_wrapper
```

### Comparing `crawlipt-0.0.1/crawlipt.egg-info/PKG-INFO` & `crawlipt-0.0.2/crawlipt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: crawlipt
-Version: 0.0.1
+Version: 0.0.2
 Summary: The script for selenium in python
 Home-page: https://github.com/WwwwwyDev/crawlipt
 Author: WwwwwyDev
-Author-email: me@example.com
+Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: selenium>=4.0.0
 Requires-Dist: ddddocr
+Requires-Dist: webdriver-manager
 
 
 <!-- markdownlint-disable MD033 MD041 -->
 <p align="center">
   <a href="https://github.com/WwwwwyDev/crawlipt"><img src="https://s2.loli.net/2024/04/19/1T7sZdrjbEfci8W.png" alt="crawlist" style="width:254px; height:208px" ></a>
 </p>
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: crawlipt Version: 0.0.1 Summary: The script for
+Metadata-Version: 2.1 Name: crawlipt Version: 0.0.2 Summary: The script for
 selenium in python Home-page: https://github.com/WwwwwyDev/crawlipt Author:
-WwwwwyDev Author-email: me@example.com License: MIT Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
-Python: >=3.10.0 Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: selenium>=4.0.0 Requires-Dist: ddddocr
+WwwwwyDev Author-email: wwy20001014@foxmail.com License: MIT Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python ::
+Implementation :: CPython Classifier: Programming Language :: Python ::
+Implementation :: PyPy Requires-Python: >=3.10.0 Description-Content-Type:
+text/markdown License-File: LICENSE Requires-Dist: selenium>=4.0.0 Requires-
+Dist: ddddocr Requires-Dist: webdriver-manager
                                   _[_c_r_a_w_l_i_s_t_]
                  # crawlipt The script for selenium in python
                          _[_p_y_p_i_][python]_[_G_i_t_H_u_b_ _s_t_a_r_s_]
 ## introduction You can use Crawlipt to driver the selenium by script in
 python.The script adopts JSON format for better cross language operations and
 physical storage. ## installing You can use pip or pip3 to install the
 crawlist\ `pip install crawlipt` or `pip3 install crawlipt` ## quickly start
```

### Comparing `crawlipt-0.0.1/setup.py` & `crawlipt-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 
 from setuptools import find_packages, setup, Command
 
 # Package meta-data.
 NAME = 'crawlipt'
 DESCRIPTION = 'The script for selenium in python'
 URL = 'https://github.com/WwwwwyDev/crawlipt'
-EMAIL = 'me@example.com'
+EMAIL = 'wwy20001014@foxmail.com'
 AUTHOR = 'WwwwwyDev'
 REQUIRES_PYTHON = '>=3.10.0'
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-    "selenium>=4.0.0", "ddddocr"
+    "selenium>=4.0.0", "ddddocr",  'webdriver-manager'
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

