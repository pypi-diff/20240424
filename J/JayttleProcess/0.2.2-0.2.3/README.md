# Comparing `tmp/JayttleProcess-0.2.2-py3-none-any.whl.zip` & `tmp/JayttleProcess-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 51932 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat     2602 b- defN 24-Apr-22 05:39 JayttleProcess/CommonDecorator.py
--rw-rw-rw-  2.0 fat     4727 b- defN 24-Apr-23 07:39 JayttleProcess/ComputerControl.py
+Zip file size: 53835 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat     2978 b- defN 24-Apr-24 02:33 JayttleProcess/CommonDecorator.py
+-rw-rw-rw-  2.0 fat    10691 b- defN 24-Apr-24 02:33 JayttleProcess/ComputerControl.py
 -rw-rw-rw-  2.0 fat      613 b- defN 24-Apr-08 05:57 JayttleProcess/EntertainmentCode.py
--rw-rw-rw-  2.0 fat     6586 b- defN 24-Apr-23 07:39 JayttleProcess/FTPCommonUse.py
--rw-rw-rw-  2.0 fat     5650 b- defN 24-Apr-22 05:39 JayttleProcess/JsonCommonManage.py
+-rw-rw-rw-  2.0 fat     6780 b- defN 24-Apr-23 15:04 JayttleProcess/FTPCommonUse.py
+-rw-rw-rw-  2.0 fat     5650 b- defN 24-Apr-24 02:33 JayttleProcess/JsonCommonManage.py
 -rw-rw-rw-  2.0 fat    36633 b- defN 24-Apr-23 07:39 JayttleProcess/RinexCommonManage.py
--rw-rw-rw-  2.0 fat    32413 b- defN 24-Apr-23 07:09 JayttleProcess/SQLCommonUse.py
--rw-rw-rw-  2.0 fat   117788 b- defN 24-Apr-22 05:38 JayttleProcess/TimeSeriesDataMethod.py
+-rw-rw-rw-  2.0 fat    32805 b- defN 24-Apr-24 02:33 JayttleProcess/SQLCommonUse.py
+-rw-rw-rw-  2.0 fat   117788 b- defN 24-Apr-24 02:34 JayttleProcess/TimeSeriesDataMethod.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-14 14:39 JayttleProcess/__init__.py
--rw-rw-rw-  2.0 fat      554 b- defN 24-Apr-23 07:40 JayttleProcess-0.2.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-23 07:40 JayttleProcess-0.2.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-23 07:40 JayttleProcess-0.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1132 b- defN 24-Apr-23 07:40 JayttleProcess-0.2.2.dist-info/RECORD
-13 files, 208805 bytes uncompressed, 50022 bytes compressed:  76.0%
+-rw-rw-rw-  2.0 fat      554 b- defN 24-Apr-24 02:34 JayttleProcess-0.2.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-24 02:34 JayttleProcess-0.2.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-24 02:34 JayttleProcess-0.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1133 b- defN 24-Apr-24 02:34 JayttleProcess-0.2.3.dist-info/RECORD
+13 files, 215732 bytes uncompressed, 51925 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: JayttleProcess/TimeSeriesDataMethod.py
 Comment: 
 
 Filename: JayttleProcess/__init__.py
 Comment: 
 
-Filename: JayttleProcess-0.2.2.dist-info/METADATA
+Filename: JayttleProcess-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: JayttleProcess-0.2.2.dist-info/WHEEL
+Filename: JayttleProcess-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: JayttleProcess-0.2.2.dist-info/top_level.txt
+Filename: JayttleProcess-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: JayttleProcess-0.2.2.dist-info/RECORD
+Filename: JayttleProcess-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## JayttleProcess/CommonDecorator.py

```diff
@@ -8,19 +8,25 @@
     def wrapper(*args, **kwargs):
         # 记录函数调用时间
         call_time = datetime.now()
         start_time = time.time()  # 记录函数开始执行的时间
 
         print(f"Function '{func.__name__}' called at {call_time}")
 
-        # 记录传入的参数类型
-        args_type_str = ', '.join(map(lambda arg: f"{type(arg).__name__}", args))
-        kwargs_type_str = ', '.join(f"{key}={type(value).__name__}" for key, value in kwargs.items())
-        all_args_type = ', '.join(filter(None, [args_type_str, kwargs_type_str]))
-        print(f"Arguments type: {all_args_type}")
+        # 记录传入的参数
+        if len(args) + len(kwargs) > 3:
+            # 如果传入的参数很多，则只打印参数类型
+            args_type_str = ', '.join(map(lambda arg: f"{type(arg).__name__}", args))
+            kwargs_type_str = ', '.join(f"{key}={type(value).__name__}" for key, value in kwargs.items())
+            all_args_type = ', '.join(filter(None, [args_type_str, kwargs_type_str]))
+            print(f"Arguments type: {all_args_type}")
+        else:
+            # 如果不多于3个参数，则返回参数的值
+            all_args = ', '.join(filter(None, [str(arg) for arg in args] + [f"{key}={value}" for key, value in kwargs.items()]))
+            print(f"Arguments: {all_args}")
 
         # 调用函数并记录返回值
         result = func(*args, **kwargs)
         print(f"Returned data type: {type(result).__name__}")  # 打印返回值的数据类型
         end_time = time.time()  # 记录函数执行完毕的时间
         print(f"executed in {(end_time - start_time):.4f}s")  # 打印执行时间
         print()
```

## JayttleProcess/ComputerControl.py

```diff
@@ -1,14 +1,21 @@
 import pyautogui
 import os
+from PIL import Image 
+import time
+import pytesseract
+
+pytesseract.pytesseract.tesseract_cmd = r'D:\Program Files\Tesseract-OCR\tesseract.exe'
+
 
 def move_and_click( x, y):
     """移动鼠标到指定坐标并单击"""
     pyautogui.moveTo(x, y)
     pyautogui.click()
+    time.sleep(0.5)
 
 def move_and_Twoclick( x, y):
     """移动鼠标到指定坐标并双击"""
     pyautogui.moveTo(x, y)
     pyautogui.click()
     pyautogui.click()
 
@@ -120,8 +127,149 @@
 def list_files_in_folders(folder_names):
     """获取目标文件夹下的所有文件file名字"""
     file_paths = []
     for folder in folder_names:
         for root, dirs, files in os.walk(folder):
             for file in files:
                 file_paths.append(os.path.join(root, file))
-    return file_paths
+    return file_paths
+
+
+def read_text_from_window(window_region):
+    """
+    从指定的窗口区域中读取文本
+    Args:
+        window_region: 窗口区域的坐标 (x, y, width, height)
+    Returns:
+        识别到的文本
+    """
+    # 截取窗口区域的截图
+    screenshot = pyautogui.screenshot(region=window_region)
+    # 示例：灰度化和二值化
+    screenshot = screenshot.convert('L')  # 转为灰度图
+    threshold = 200  # 阈值，根据需要调整
+    screenshot = screenshot.point(lambda p: p > threshold and 255)
+    # 将截图保存为临时文件
+    temp_image_path = "temp_screenshot.png"
+    screenshot.save(temp_image_path)
+    # 使用 pytesseract 识别文本
+    text = pytesseract.image_to_string(Image.open(temp_image_path), lang='chi_sim')
+    # # 删除临时文件
+    # os.remove(temp_image_path)
+    return text
+
+
+def ensure_no_input_data():
+    # 确保tbc输入的文件为空
+    window_region_输入= (170, 284, 35, 16)
+    while True:
+        # 识别窗口中的文本
+        recognized_text = read_text_from_window(window_region_输入)
+        if recognized_text:
+            move_and_click(190, 289) #单击第一个文件
+            right_click_and_press_D() #删除文件
+        else:
+            break
+    # 请替换为您希望识别的窗口区域的坐标
+    window_region_输入= (170, 270, 35, 16)
+    # 识别窗口中的文本
+    recognized_text = read_text_from_window(window_region_输入)
+
+    if recognized_text:
+        move_and_click(205, 275) #单击第一个文件
+        right_click_and_press_D() #删除文件
+
+
+def auto_turn_off():
+    move_and_click(27, 1572)#菜单
+    move_and_click(582, 1500)#菜单
+    time.sleep(1)
+    move_and_click(592, 1433)#关机
+    move_and_click(592, 1433)#关机
+
+
+def TBC_auto_Process():
+    window_region_保存 = (1625, 567, 37, 20)
+    window_region_输入= (1590, 950, 35, 16)
+    # 目标文件夹路径
+    folder_path = r"D:\Ropeway\FTPMerge"
+    # 获取目标文件夹中所有文件夹的名字
+    subdirectories = get_subdirectories_with_no_csv_without03(folder_path)
+
+
+    for directory in subdirectories:
+        exit_for_loop = False  # 标志，用于指示是否退出外部循环
+        ensure_no_input_data()
+        move_and_click(87, 31)#本地
+        time.sleep(1) #等待
+        move_and_click(39, 74)     #tbc-输入
+        time.sleep(1) #等待
+        move_and_click(2453, 233)     #导入文件夹
+        time.sleep(1) #等待
+        move_and_Twoclick(2424, 233)     #双击
+        type_string(f"\\{directory}") # 输入文件夹名字
+        move_and_click(2422, 323) #单击第一个文件
+        move_and_click_with_shift(2422, 423) #拖动并点击最后一个文件
+        move_and_click(2431, 1510) #输入
+        start_time_input = time.time()  # 开始第一个循环的时间
+         # 内部while循环
+        while True:
+            # 识别窗口中的文本
+            recognized_text = read_text_from_window(window_region_输入)
+            # 如果识别到的文本是"确定"
+            if "确定" in recognized_text:
+                move_and_click(1607, 961)  # 保存
+                break  # 结束内部循环
+            # 检查是否超过一分钟
+            if time.time() - start_time_input > 60:
+                print("第一个循环执行时间超过1分钟，终止程序。")
+                exit_for_loop = True  # 设置标志，指示需要退出外部循环
+                break  # 结束内部循环
+            time.sleep(1)  # 等待
+
+        # 检查是否需要退出外部循环
+        if exit_for_loop:
+            print("外部循环执行时间超过1分钟，终止程序。")
+            break  # 退出外部循环
+
+        time.sleep(1) #等待
+        move_and_click(136, 40) #测量
+        time.sleep(0.5) #等待
+        move_and_click(675, 77) #基线解算
+        start_time_save = time.time()  # 开始第二个循环的时间
+        while True:
+            # 识别窗口中的文本
+            recognized_text = read_text_from_window(window_region_保存)
+            # 如果识别到的文本是"保存"
+            if "保存" in recognized_text:
+                time.sleep(1)  # 等待
+                move_and_click(1643, 575)  # 点击保存按钮
+                break  # 结束循环
+            # 检查是否超过一分钟
+            if time.time() - start_time_save > 90:
+                print("第二个循环执行时间超过1分钟，终止程序。")
+                exit_for_loop = True  # 设置标志，指示需要退出外部循环
+                break
+        # 检查是否需要退出外部循环
+        if exit_for_loop:
+            print("外部循环执行时间超过1分钟，终止程序。")
+            break  # 退出外部循环
+        time.sleep(1.5) #等待
+        move_and_click(84, 40)#本地
+        time.sleep(0.5) #等待
+        move_and_click(96, 73)#输出菜单
+        time.sleep(1) #等待
+        move_and_click(54, 244) #单击R031点
+        move_and_click(2179, 449) #单击到文件名的初始
+        time.sleep(1) #等待
+        move_and_click_with_shift(2474, 447) #拖动并全选文件名
+        time.sleep(1) #等待
+        type_string(f"D:\\Ropeway\\FTPcsv2\\{directory}.csv") # 输入文件夹名字
+        time.sleep(1) #等待D
+        move_and_click(2436, 1511)#输出栏里的保存
+        time.sleep(1) #等待
+        move_and_click(168, 290) #单击第一个文件
+        time.sleep(0.5) #等待
+        move_and_click_with_shift(147, 376) #拖动并点击最后一个文件
+        time.sleep(0.5) #等待
+        right_click_and_press_D() #删除文件
+
```

## JayttleProcess/FTPCommonUse.py

```diff
@@ -118,15 +118,16 @@
         # 确保本地保存路径存在
         os.makedirs(local_save_path, exist_ok=True)
 
         # 下载指定的文件
         for file_name in files_to_download:
             local_file_path = os.path.join(local_save_path, file_name)
             # 检查文件是否已经存在于本地路径中
-            if not os.path.exists(local_file_path):
+            # 检查文件是否已经存在于本地路径中，且替换后的文件也不存在
+            if not os.path.exists(local_file_path) and not os.path.exists(local_file_path.replace(".crx.Z", ".rnx").replace(".rnx.Z", ".rnx")):
                 with open(local_file_path, 'wb') as local_file:
                     ftp.retrbinary(f'RETR {file_name}', local_file.write)
 
                 print(f"已下载文件: {file_name} 到本地路径: {local_file_path}")
             else:
                 print(f"文件 {file_name} 已存在于本地路径: {local_file_path}, 跳过下载")
 
@@ -137,14 +138,15 @@
         return False
 
     finally:
         # 关闭FTP连接
         ftp.quit()
 
 
+
 def process_string(s: str) -> str:
     if len(s) == 4:
         if s.startswith('B'):
             return 'towerbase' + s[2]
         elif s.startswith('R'):
             return 'tower' + s[2]
     return None
```

## JayttleProcess/SQLCommonUse.py

```diff
@@ -937,13 +937,22 @@
     except Exception as e:
         print("Error executing SQL statement:", e)
         return None
     finally:
         cursor.close()
         conn.close()
 
-# # 使用示例（需要提供实际的数据库表名和时间范围）
-# listName = 'ggkx'
-# StartTime = datetime(2023, 3, 1)
-# EndTime = datetime(2024, 4, 2)
-# high_frequency_periods = query_high_frequency_periods(listName, StartTime, EndTime)
-# print(high_frequency_periods)
+# 使用示例（需要提供实际的数据库表名和时间范围）
+# 打开或创建一个文本文件以写入模式打开
+# with open('query_high_frequency_periods.txt', 'w') as file:
+#     # 使用示例（需要提供实际的数据库表名和时间范围）
+#     listName = 'ggkx'
+#     StartTime = datetime(2023, 3, 1)
+#     EndTime = datetime(2024, 4, 2)
+#     high_frequency_periods = query_high_frequency_periods(listName, StartTime, EndTime)
+
+#     # 将每个高频周期写入文件中
+#     for period in high_frequency_periods:
+#         file.write(str(period) + '\n')
+
+# # 输出完成提示
+# print("Output has been written to output.txt")
```

## Comparing `JayttleProcess-0.2.2.dist-info/METADATA` & `JayttleProcess-0.2.3.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: JayttleProcess
-Version: 0.2.2
-Summary: modifty time:2024-04-23 15:00
+Version: 0.2.3
+Summary: modifty time:2024-04-24 10:35
  en: Data Process;
  zh_CN:数据处理的方法
 Home-page: UNKNOWN
 Author: Jayttle
 Author-email: 294448068@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
```

## Comparing `JayttleProcess-0.2.2.dist-info/RECORD` & `JayttleProcess-0.2.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-JayttleProcess/CommonDecorator.py,sha256=JbmL5wFuJ1bxNh-ka2drELVX8Y4InzNJ-_sXKDyiMvU,2602
-JayttleProcess/ComputerControl.py,sha256=S-glg1n5thtd-GxeemZVKIJT2ibXkyw71qUTYDxmG6A,4727
+JayttleProcess/CommonDecorator.py,sha256=ES7hIDpAL3zhzpJYEXlgG4_LGvDsBoJqgIcruJiIr9A,2978
+JayttleProcess/ComputerControl.py,sha256=kUsJJmW2U_rY2SXiHGZ1_baRFfSL40F5PoWpmawofPE,10691
 JayttleProcess/EntertainmentCode.py,sha256=KR-nFHjwIjfl8E_IMuRl44p2Xwkw6UMZYuvkdL9NFck,613
-JayttleProcess/FTPCommonUse.py,sha256=m48OiTsxu4G4sP1_wJj7rpeK1m-R3BTfnkXdTukogNQ,6586
+JayttleProcess/FTPCommonUse.py,sha256=gpniZo2IAqyOWsuqh3NIsZ0ON6vfAHJBcIR3tVLX7zs,6780
 JayttleProcess/JsonCommonManage.py,sha256=KJtfAxPUGktFMocoFKFd8E_VtGW-vyhAMPPz--34mkA,5650
 JayttleProcess/RinexCommonManage.py,sha256=4LxiF_DKccS01OkQidPgDwRkgJukjU2VyIlekHvMifo,36633
-JayttleProcess/SQLCommonUse.py,sha256=PBIw5fBMCrg1R3PHPaNVZstXd625aIOVFJ1760vk-mE,32413
+JayttleProcess/SQLCommonUse.py,sha256=w7mOwUQ81MyXjg8NP_vYs7trLTF0_3H5B-CXL4AqPhw,32805
 JayttleProcess/TimeSeriesDataMethod.py,sha256=HUmf2RjkcNRAcjS4XkTwDqQNc-6mGhVcufjGo82D4rk,117788
 JayttleProcess/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-JayttleProcess-0.2.2.dist-info/METADATA,sha256=794sMy0WJ0j5sWheHXUyEbsKDKuPgG1q24Wdjl5olcs,554
-JayttleProcess-0.2.2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-JayttleProcess-0.2.2.dist-info/top_level.txt,sha256=0wohZ9zSz5j0d_abN3JTtoTUIvlCsfp-LHIP_NcoOlw,15
-JayttleProcess-0.2.2.dist-info/RECORD,,
+JayttleProcess-0.2.3.dist-info/METADATA,sha256=2l7g2m24U4dF--J2gKXSBFs3Lneqg1xmYIBDQbnt3Hc,554
+JayttleProcess-0.2.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+JayttleProcess-0.2.3.dist-info/top_level.txt,sha256=0wohZ9zSz5j0d_abN3JTtoTUIvlCsfp-LHIP_NcoOlw,15
+JayttleProcess-0.2.3.dist-info/RECORD,,
```

