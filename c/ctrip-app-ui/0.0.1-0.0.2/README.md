# Comparing `tmp/ctrip-app-ui-0.0.1.tar.gz` & `tmp/ctrip-app-ui-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.0.1.tar", last modified: Wed Apr 24 09:41:38 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.0.2.tar", last modified: Wed Apr 24 10:24:49 2024, max compression
```

## Comparing `ctrip-app-ui-0.0.1.tar` & `ctrip-app-ui-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 09:41:38.146736 ctrip-app-ui-0.0.1/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      474 2024-04-24 09:41:38.145740 ctrip-app-ui-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 09:41:38.130806 ctrip-app-ui-0.0.1/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.0.1/capp_ui/__init__.py
--rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.0.1/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.0.1/capp_ui/device.py
--rw-rw-rw-   0        0        0     1263 2024-04-24 09:31:47.000000 ctrip-app-ui-0.0.1/capp_ui/dir.py
--rw-rw-rw-   0        0        0    47748 2024-04-24 09:35:47.000000 ctrip-app-ui-0.0.1/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.0.1/capp_ui/libs.py
--rw-rw-rw-   0        0        0    23814 2024-04-24 09:32:32.000000 ctrip-app-ui-0.0.1/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.0.1/capp_ui/platforms.py
--rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.0.1/capp_ui/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:41:38.143744 ctrip-app-ui-0.0.1/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-04-24 09:41:37.000000 ctrip-app-ui-0.0.1/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2024-04-24 09:41:38.000000 ctrip-app-ui-0.0.1/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 09:41:37.000000 ctrip-app-ui-0.0.1/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-24 09:41:37.000000 ctrip-app-ui-0.0.1/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-24 09:41:37.000000 ctrip-app-ui-0.0.1/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 09:41:38.147744 ctrip-app-ui-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-04-24 09:39:16.000000 ctrip-app-ui-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:24:49.410220 ctrip-app-ui-0.0.2/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-04-24 10:24:49.409222 ctrip-app-ui-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 10:24:49.394264 ctrip-app-ui-0.0.2/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.0.2/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.0.2/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.0.2/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1263 2024-04-24 09:31:47.000000 ctrip-app-ui-0.0.2/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    49360 2024-04-24 10:21:33.000000 ctrip-app-ui-0.0.2/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.0.2/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    23814 2024-04-24 09:32:32.000000 ctrip-app-ui-0.0.2/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.0.2/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.0.2/capp_ui/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:24:49.407228 ctrip-app-ui-0.0.2/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-24 10:24:49.000000 ctrip-app-ui-0.0.2/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2024-04-24 10:24:49.000000 ctrip-app-ui-0.0.2/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 10:24:49.000000 ctrip-app-ui-0.0.2/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-24 10:24:49.000000 ctrip-app-ui-0.0.2/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-24 10:24:49.000000 ctrip-app-ui-0.0.2/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 10:24:49.411217 ctrip-app-ui-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-04-24 10:24:37.000000 ctrip-app-ui-0.0.2/setup.py
```

### Comparing `ctrip-app-ui-0.0.1/LICENSE` & `ctrip-app-ui-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.1/capp_ui/date_extend.py` & `ctrip-app-ui-0.0.2/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.1/capp_ui/device.py` & `ctrip-app-ui-0.0.2/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.1/capp_ui/dir.py` & `ctrip-app-ui-0.0.2/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.1/capp_ui/domain_service.py` & `ctrip-app-ui-0.0.2/capp_ui/domain_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,14 +62,47 @@
         if is_exists(file_name):
             temp = self.device.get_cv_template(file_name=file_name)
         else:
             temp = (154, 2878)  # LG g7手机上对应的坐标位置，其他型号手机可能不是这个值
         self.device.touch(v=temp)
 
     @SleepWait(wait_time=1)
+    def touch_my(self) -> None:
+        """进入app后，点击【我的】"""
+        my_button = self.device.poco(type="android.view.ViewGroup", name="ctrip.android.view:id/a", desc="我的")
+        my_button.click()
+
+    @SleepWait(wait_time=2)
+    def touch_unpaid(self) -> None:
+        """进入my主页后，点击【待付款】"""
+        unpaid_button = self.device.poco(type="android.widget.TextView", name="ctrip.android.view:id/a", text="待付款")
+        unpaid_button.click()
+
+    @SleepWait(wait_time=2)
+    def select_search_box(self, ctrip_order_id: str) -> None:
+        """进入待付款列表页，点击【搜索框】"""
+        search_box = self.device.poco(type="android.widget.TextView", name="ctrip.android.view:id/a", text="搜索订单")
+        search_box.click()
+        search_box.set_text(ctrip_order_id)
+        # 模拟键盘按下回车键（keyCode为66表示回车键）
+        self.device.poco.device.input(keyevent="66")
+
+    @SleepWait(wait_time=1)
+    def touch_to_payment_at_list_page(self) -> None:
+        """进入待付款列表页，点击【去支付】"""
+        search_box = self.device.poco(type="android.widget.TextView", name="android.widget.TextView", text="去支付")
+        search_box.click()
+
+    @SleepWait(wait_time=2)
+    def touch_to_payment_at_order_detail(self) -> None:
+        """在订单详情页，点击【去支付】"""
+        search_box = self.device.poco(type="android.widget.TextView", name="pcardLimit_Text_去支付", text="去支付")
+        search_box.click()
+
+    @SleepWait(wait_time=1)
     def touch_flight_ticket(self) -> None:
         """进入app后，点击【首页】，点击【机票】"""
         file_name = join_path([get_images_dir(), "机票.png"])
         if is_exists(file_name):
             temp = self.device.get_cv_template(file_name=file_name)
         else:
             temp = (445, 560)  # LG g7手机上对应的坐标位置，其他型号手机可能不是这个值
```

### Comparing `ctrip-app-ui-0.0.1/capp_ui/libs.py` & `ctrip-app-ui-0.0.2/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.1/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.0.2/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.1/capp_ui/platforms.py` & `ctrip-app-ui-0.0.2/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.1/capp_ui/utils.py` & `ctrip-app-ui-0.0.2/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.1/setup.py` & `ctrip-app-ui-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.0.1',
+    version='0.0.2',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

