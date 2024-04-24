# Comparing `tmp/unibot_hn-0.1.0.tar.gz` & `tmp/unibot_hn-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unibot_hn-0.1.0.tar", max compression
+gzip compressed data, was "unibot_hn-0.1.1.tar", max compression
```

## Comparing `unibot_hn-0.1.0.tar` & `unibot_hn-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1066 2024-03-22 14:48:34.861774 unibot_hn-0.1.0/LICENSE
--rw-r--r--   0        0        0       14 2024-03-23 15:51:40.067352 unibot_hn-0.1.0/README.md
--rw-r--r--   0        0        0      319 2024-04-19 10:11:24.553482 unibot_hn-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      426 2024-02-26 08:00:27.894916 unibot_hn-0.1.0/unibot_hn/Misc.py
--rw-r--r--   0        0        0     3696 2024-02-26 08:00:27.898217 unibot_hn-0.1.0/unibot_hn/PID.py
--rw-r--r--   0        0        0        0 2024-03-23 16:05:04.761382 unibot_hn-0.1.0/unibot_hn/__init__.py
--rw-r--r--   0        0        0    22001 2024-02-26 09:57:26.859814 unibot_hn-0.1.0/unibot_hn/board.py
--rw-r--r--   0        0        0    36032 2024-04-19 11:15:52.560156 unibot_hn-0.1.0/unibot_hn/camera.py
--rw-r--r--   0        0        0     7104 2024-02-26 09:58:19.954440 unibot_hn-0.1.0/unibot_hn/img_processing.py
--rw-r--r--   0        0        0     1680 2024-03-01 15:34:18.533544 unibot_hn-0.1.0/unibot_hn/robot_config.py
--rw-r--r--   0        0        0      676 2024-03-01 15:44:13.270021 unibot_hn-0.1.0/unibot_hn/robot_param_init.txt
--rw-r--r--   0        0        0     6301 2024-04-19 10:31:37.631075 unibot_hn-0.1.0/unibot_hn/setObjectColor.py
--rw-r--r--   0        0        0     6296 2024-04-19 10:31:37.632369 unibot_hn-0.1.0/unibot_hn/setScreenObjectColor.py
--rw-r--r--   0        0        0    23524 2024-04-19 11:15:19.100483 unibot_hn-0.1.0/unibot_hn/unibot.py
--rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 unibot_hn-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-22 14:48:34.861774 unibot_hn-0.1.1/LICENSE
+-rw-r--r--   0        0        0       14 2024-03-23 15:51:40.067352 unibot_hn-0.1.1/README.md
+-rw-r--r--   0        0        0      319 2024-04-24 13:52:53.271077 unibot_hn-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      426 2024-02-26 08:00:27.894916 unibot_hn-0.1.1/unibot_hn/Misc.py
+-rw-r--r--   0        0        0     3696 2024-02-26 08:00:27.898217 unibot_hn-0.1.1/unibot_hn/PID.py
+-rw-r--r--   0        0        0        0 2024-03-23 16:05:04.761382 unibot_hn-0.1.1/unibot_hn/__init__.py
+-rw-r--r--   0        0        0    22001 2024-02-26 09:57:26.859814 unibot_hn-0.1.1/unibot_hn/board.py
+-rw-r--r--   0        0        0    38374 2024-04-24 13:05:17.486416 unibot_hn-0.1.1/unibot_hn/camera.py
+-rw-r--r--   0        0        0     7104 2024-02-26 09:58:19.954440 unibot_hn-0.1.1/unibot_hn/img_processing.py
+-rw-r--r--   0        0        0     1680 2024-03-01 15:34:18.533544 unibot_hn-0.1.1/unibot_hn/robot_config.py
+-rw-r--r--   0        0        0      676 2024-03-01 15:44:13.270021 unibot_hn-0.1.1/unibot_hn/robot_param_init.txt
+-rw-r--r--   0        0        0     6301 2024-04-19 11:47:41.367257 unibot_hn-0.1.1/unibot_hn/setObjectColor.py
+-rw-r--r--   0        0        0     6296 2024-04-19 11:47:41.367539 unibot_hn-0.1.1/unibot_hn/setScreenObjectColor.py
+-rw-r--r--   0        0        0    24774 2024-04-24 13:52:28.657934 unibot_hn-0.1.1/unibot_hn/unibot.py
+-rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 unibot_hn-0.1.1/PKG-INFO
```

### Comparing `unibot_hn-0.1.0/LICENSE` & `unibot_hn-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.1.0/unibot_hn/PID.py` & `unibot_hn-0.1.1/unibot_hn/PID.py`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.1.0/unibot_hn/board.py` & `unibot_hn-0.1.1/unibot_hn/board.py`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.1.0/unibot_hn/camera.py` & `unibot_hn-0.1.1/unibot_hn/camera.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 '''
 摄像头设置相关的函数
 '''
 
 import cv2
 import numpy as np
 import math
-from .robot_config import Device_Config
+from robot_config import Device_Config
 
 target_object = {
     'target_shape': 0,
     'target_color': 0,
     'color': 0,
     'shape': 0,
     'x': 0,
     'y': 0,
-    'flag': 0
+    'flag': 0,
+    'objcet_num': 0
 }
 
-rs = []
 object_rs = {
     'rs_object1_line': 0,
     'rs_object2_line': 0,
     'rs_object1_num': 0,
     'rs_object2_num': 0,
 }
 
+rs = []
+
 
 class DetectResult:
     color = None
     shape = None
 
 
 screen_result_pic = {
@@ -268,14 +270,15 @@
             target_object['color'] = 0
         elif (color_flag == 1):
             str += "绿色"
             target_object['color'] = 1
         else:
             str += "黄色"
             target_object['color'] = 2
+        rs.append(color_flag)
         shape_flag = 3
         print("颜色识别结束，颜色为:", str)
 
         shape_flag = self.detect_object_shape(color_flag, round_square_threshold, big_small_round_threshold, times=10)
         if (shape_flag == 0):
             str += "圆柱"
             target_object['shape'] = 0
@@ -287,14 +290,15 @@
             target_object['shape'] = 2
         print("本次识别结果为：", str)
         if (target_object['shape'] == target_object['target_shape'] and target_object["target_color"] == target_object[
             "shape"]):
             target_object["flag"] = 1
         else:
             target_object["flag"] = 0
+        rs.append(shape_flag)
         print("形状识别结束,真假为:", target_object["flag"])
 
     # 识别物体颜色
     def detect_object_color(self, times: int, target: int):
         rs = []
         for l in range(0, times):
             frame = self.get_frame()
@@ -624,15 +628,15 @@
             return 2
         # 3重新识别
         else:
             return 3
 
             # 识别物体中心，用来矫正
 
-    def detect_object_center(self, color_flag: int,min_x,max_x,min_y,max_y, target_area: int = 5000):
+    def detect_object_center(self, color_flag: int, min_x, max_x, min_y, max_y, target_area: int = 5000):
         color_value = []
         if color_flag == 0:
             color_value = colors_value['red']
         if color_flag == 1:
             color_value = colors_value['green']
         if color_flag == 2:
             color_value = colors_value['yellow']
@@ -678,15 +682,15 @@
                     # for p in approx:
                     # print(p)
                     # cv2.circle(img,(p[0][0],p[0][1]),2,(255,0,0),3)
                     cv2.circle(img, (center_x, center_y), 2, (255, 0, 0), 3)
                     cv2.imshow('camera', img)
                     cv2.waitKey(1)
 
-            if (center_x>min_x and center_x<max_x and center_y>min_y and center_y<=max_y):
+            if (center_x > min_x and center_x < max_x and center_y > min_y and center_y <= max_y):
                 return center_x, center_y
             else:
                 return -1, -1
         except:
             return -1, -1
 
     def getAreaMaxContour(self, contours):
@@ -850,65 +854,121 @@
                 color = [0, 255, 0]
                 sstr += "绿色"
             if (color1_list[i] == 2):
                 color = [0, 255, 255]
                 sstr += "黄色"
 
             cv2.putText(canvas, str(i + 1), (1 + i * 53 + 16, 260), cv2.FONT_HERSHEY_TRIPLEX, 1, (255, 255, 255), 2)
-            if shape1_list[i] == 0:
+            if (shape1_list[i] == 0):
                 sstr += "圆柱"
                 cv2.circle(canvas, (1 + i * 53 + 26, 210), 20, color, -1)
-            if shape1_list[i] == 1:
+            if (shape1_list[i] == 1):
                 pts = np.array(
                     [[(1 + i * 53 + 16, 190), (1 + i * 53 + 36, 190), (1 + i * 53 + 46, 230), (1 + i * 53 + 6, 230)]],
                     dtype=np.int32)
                 cv2.fillPoly(canvas, pts, color)
                 sstr += "锥体"
-            if shape1_list[i] == 2:
+            if (shape1_list[i] == 2):
                 sstr += "方块"
                 cv2.rectangle(canvas, (1 + i * 53 + 6, 190), (1 + i * 53 + 46, 230), color, -1)
             print(sstr)
         cv2.imshow('camera', canvas)
         cv2.waitKey(1)
         target_color = self.object_result('target_color')
         target_shape = self.object_result('target_shape')
         flag = 0
         rs_object1_line = -1
         rs_object1_num = -1
         rs_object2_line = -1
         rs_object2_num = -1
         for i in range(9):
-            if color1_list[i] == target_color and shape1_list[i] == target_shape:
-                if flag == 0:
+            if (color1_list[i] == target_color and shape1_list[i] == target_shape):
+                if (flag == 0):
                     flag = 1
                     rs_object1_line = 1
                     rs_object1_num = i
                 else:
                     rs_object2_line = 1
                     rs_object2_num = i
-            if color2_list[i] == target_color and shape2_list[i] == target_shape:
-                if flag == 0:
+            if (color2_list[i] == target_color and shape2_list[i] == target_shape):
+                if (flag == 0):
                     flag = 1
                     rs_object1_line = 2
                     rs_object1_num = i
                 else:
                     rs_object2_line = 2
                     rs_object2_num = i
-        if rs_object1_num == rs_object2_num:
-            if rs_object1_line > rs_object2_line:
+        if (rs_object1_num == rs_object2_num):
+            if (rs_object1_line > rs_object2_line):
                 t = rs_object1_line
                 rs_object1_line = rs_object2_line
                 rs_object2_line = t
-        elif rs_object1_num > rs_object2_num:
+        elif (rs_object1_num > rs_object2_num):
             t = rs_object1_line
             rs_object1_line = rs_object2_line
             rs_object2_line = t
             t = rs_object1_num
             rs_object1_num = rs_object2_num
             rs_object2_num = t
         object_rs['rs_object1_line'] = rs_object1_line
         object_rs['rs_object2_line'] = rs_object2_line
         object_rs['rs_object1_num'] = rs_object1_num
         object_rs['rs_object2_num'] = rs_object2_num
 
     def settest(self, param, value):
         object_rs[param] = value
+
+    def detect_vertical_black_line_for_align(self, img):
+        lineColorSet = 0
+        frame = self.image_pre_processing(img)
+
+        # 处理图片变成点
+        linePos_1 = 5
+        linePos_2 = 320 - 5
+        colorPos_1 = frame[:, linePos_1]
+        colorPos_2 = frame[:, linePos_2]
+        center_Pos1 = 0
+        center_Pos2 = 0
+        error = 10
+        try:
+            lineColorCount_Pos1 = np.sum(colorPos_1 == lineColorSet)
+            lineColorCount_Pos2 = np.sum(colorPos_2 == lineColorSet)
+
+            lineIndex_Pos1 = np.where(colorPos_1 == lineColorSet)
+            lineIndex_Pos2 = np.where(colorPos_2 == lineColorSet)
+            if lineColorCount_Pos1 == 0:
+                lineColorCount_Pos1 = 1
+            if lineColorCount_Pos2 == 0:
+                lineColorCount_Pos2 = 1
+
+            down_Pos1 = lineIndex_Pos1[0][lineColorCount_Pos1 - 1]
+            up_Pos1 = lineIndex_Pos1[0][0]
+            center_Pos1 = int((down_Pos1 + up_Pos1) / 2)
+
+            down_Pos2 = lineIndex_Pos2[0][lineColorCount_Pos2 - 1]
+            up_Pos2 = lineIndex_Pos2[0][0]
+            center_Pos2 = int((down_Pos2 + up_Pos2) / 2)
+            cv2.line(img, (linePos_1, up_Pos1), (linePos_2, up_Pos2), (255, 128, 64), 2)
+            cv2.line(img, (linePos_1, down_Pos1), (linePos_2, down_Pos2), (255, 128, 64), 2)
+
+            cv2.line(img, (linePos_1, up_Pos1), (linePos_1, down_Pos1), (255, 128, 64), 2)
+            cv2.line(img, (linePos_2, up_Pos2), (linePos_2, down_Pos2), (255, 128, 64), 2)
+
+            cv2.line(img, (linePos_1, center_Pos1), (linePos_2, center_Pos2), (255, 128, 64), 2)
+
+            self.show_frame(img)
+        except:
+            print("error")
+            pass
+
+        return center_Pos1, center_Pos2, img
+
+    def first_detected_object_rs(self):
+        target_color = self.object_result('target_color')
+        target_shape = self.object_result('target_shape')
+        now_color = self.object_result('color')
+        now_shape = self.object_result('shape')
+        print("当前检测结果和目标:", target_color, target_shape, now_color, now_shape)
+        if (target_color == now_color and target_shape == now_shape):
+            return True
+        else:
+            return False
```

### Comparing `unibot_hn-0.1.0/unibot_hn/img_processing.py` & `unibot_hn-0.1.1/unibot_hn/img_processing.py`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.1.0/unibot_hn/robot_config.py` & `unibot_hn-0.1.1/unibot_hn/robot_config.py`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.1.0/unibot_hn/robot_param_init.txt` & `unibot_hn-0.1.1/unibot_hn/robot_param_init.txt`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.1.0/unibot_hn/setObjectColor.py` & `unibot_hn-0.1.1/unibot_hn/setObjectColor.py`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.1.0/unibot_hn/setScreenObjectColor.py` & `unibot_hn-0.1.1/unibot_hn/setScreenObjectColor.py`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.1.0/unibot_hn/unibot.py` & `unibot_hn-0.1.1/unibot_hn/unibot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .board import Board
 from .camera import Camera
 from .robot_config import Device_Config
 import math
-import unibot_hn.Misc as Misc
+import Misc as Misc
 import time
 from threading import Thread
 
 th = None
 slow_en = True
 
 last_velocity = 0
@@ -510,29 +510,29 @@
         """
         机械展执行动作的函数，指定持续时间、舵机角度和可选的舵机ID。
 
         参数:
             duration (int): 动作持续时间。
             servo_degree (int): 舵机角度。
             servo_id (int, optional): 舵机 ID。默认为 1。
-            
+
         返回:
             None
         """
         deg = Misc.setRange(servo_degree, 0, 180)  # 将输入限制在0-180度
         pulse = int(Misc.map(deg, 0, 180, 500, 2500))  # 将角度转换为脉冲
         self.board.pwm_servo_set_position(duration, [[servo_id, pulse]])
 
     def read_position(self, servo_id=1):
         """
         读取机械爪舵机角度和可选的舵机ID。
 
-        参数:  
+        参数:
             servo_id (int, optional): 舵机 ID。默认为 1。
-            
+
         返回:
             servo_degree (int): 舵机角度。
         """
         pulse = self.board.pwm_servo_read_position(servo_id)
         servo_degree = int(Misc.map(pulse, 500, 2500, 0, 180))
         return servo_degree
 
@@ -587,25 +587,29 @@
 
         self.chassis.stop()
 
     def translational_move_find_line(self, endpointnum=45, point=3):
         # endpointnum数值表示黑点构成的线宽，与摄像头的高低位置相关
         # point数值表示需要对齐的点点数量
         img = self.camera.get_frame()
-        ls, lsc, img = self.camera.detect_vertical_black_line(img)
-        self.camera.show_frame(img)
-        ans = 0
-        for i in range(5):
-            if ls[i][0] is not None:
-                if endpointnum < lsc[i] < 100:
-                    ans += 1
-            if ans >= point:
-                find_line = True
-            else:
-                find_line = False
+        find_line = False
+        try:
+            ls, lsc, img = self.camera.detect_vertical_black_line(img)
+            self.camera.show_frame(img)
+            ans = 0
+            for i in range(5):
+                if ls[i][0] is not None:
+                    if endpointnum < lsc[i] < 100:
+                        ans += 1
+                if ans >= point:
+                    find_line = True
+                else:
+                    find_line = False
+        except:
+            pass
         return find_line
 
     # 前后移动，寻找水平的黑线
     def move_find_line(self, endpointnum=200):
         img = self.camera.get_frame()
         ls, lsc, img = self.camera.detect_vertical_black_line(img)
         self.camera.show_frame(img)
@@ -623,66 +627,107 @@
 
         elif direction == 'right':
             self.board.bus_servo_set_position(1, [[1, self.right_holder_servo_position['angle1']],
                                                   [2, self.right_holder_servo_position['angle2']],
                                                   [3, self.right_holder_servo_position['angle3']],
                                                   [4, self.right_holder_servo_position['angle4']]])
 
-    def align_object(self, p_x, p_y,error,min_x = 30,max_x = 290,min_y = 20,max_y = 260,target_area: int = 5000,speed=0):
+    def align_object(self, p_x, p_y, error, min_x=30, max_x=290, min_y=20, max_y=260, target_area: int = 5000, speed=0):
         color_flag = 3
         cx = -1
         cy = -1
         for index in range(0, 3):
             frame = self.camera.get_frame()
         while color_flag == 3:
             color_flag = self.camera.detect_object_color(5, target_area)
             print(color_flag)
         ans = 0
         print("颜色：", color_flag)
         while True:
-            cx, cy = self.camera.detect_object_center(color_flag, min_x,max_x,min_y,max_y ,target_area)
+            cx, cy = self.camera.detect_object_center(color_flag, min_x, max_x, min_y, max_y, target_area)
             if cx != -1 and cy != -1:
-                #print(cx,cy)
+                # print(cx,cy)
                 error_x = cx - 160
                 error_y = cy - 120
                 px = error_x * p_x
                 py = error_y * p_y
 
-                if(abs(cx-160)<=error and abs(cy-120)<=error):
-                    ans+=1
+                if (abs(cx - 160) <= error and abs(cy - 120) <= error):
+                    ans += 1
                 else:
-                    if(abs(cx-160)<=8):
-                        px=0
-                    elif(px<0):
-                        px-=speed
-                    elif(px>0):
-                        px+=speed
-                    if(abs(cy-120)<=8):
-                        py=0
-                    elif(py<0):
-                        py-=speed
-                    elif(py>0):
-                        py+=speed
-                    ans=0
-                if(ans>=3):
+                    if (abs(cx - 160) <= 8):
+                        px = 0
+                    elif (px < 0):
+                        px -= speed
+                    elif (px > 0):
+                        px += speed
+                    if (abs(cy - 120) <= 8):
+                        py = 0
+                    elif (py < 0):
+                        py -= speed
+                    elif (py > 0):
+                        py += speed
+                    ans = 0
+                if (ans >= 3):
                     self.chassis.stop()
                     break
-                print(px,py)
-                self.board.set_motor_speed([[1, px-py], [2, px+py], [3, -px-py], [4, -px+py]])
-
+                print(px, py)
+                self.board.set_motor_speed([[1, px - py], [2, px + py], [3, -px - py], [4, -px + py]])
 
         print("矫正结束")
 
-    def first_dected_object_rs(self):
-        target_color=self.camera.object_result('target_color')
-        target_shape=self.camera.object_result('target_shape')
-        now_color=self.camera.object_result('color')
-        now_shape=self.camera.object_result('shape')
-        print("当前检测结果和目标:",target_color,target_shape,now_color,now_shape)
-        if(target_color == now_color and target_shape == now_shape):
-            return True
-        else:
-            return False
+
+
+    # 水平对线
+    def align_horizontal_lines(self):
+        last_error = 0
+        lineColorSet = 0
+        screen_rotation = False
+        l_speed = 0.2
+        r_speed = 0.2
+        lf = 0
+        rf = 0
+        for l in range(0, 3):
+            frame = self.camera.get_frame()
+        while True:
+            img = self.camera.get_frame()
+            # 处理图片
+            c1, c2, img = self.camera.detect_vertical_black_line_for_align(img)
+            print(c1, c2)
+            if (c1 > 160):
+                l_speed = 0
+                lf = 1
+            if (c2 > 160):
+                r_speed = 0
+                rf = 1
+            if (lf == 1 and rf == 1):
+                self.chassis.stop()
+                break
+            self.board.set_motor_speed([[1, l_speed], [2, -r_speed], [3, l_speed], [4, -r_speed]])
+
+        l_speed = 0.2
+        r_speed = 0.2
+        lf = 0
+        rf = 0
+        while True:
+            img = self.camera.get_frame()
+            # 处理图片
+            c1, c2, img = self.camera.detect_vertical_black_line_for_align(img)
+            print(c1, c2)
+            if (c1 < 150):
+                l_speed = 0
+                lf = 1
+            if (c2 < 150):
+                r_speed = 0
+                rf = 1
+            if (lf == 1 and rf == 1):
+                self.chassis.stop()
+                break
+            self.board.set_motor_speed([[1, -l_speed], [2, r_speed], [3, -l_speed], [4, r_speed]])
+            # elif(error>3):
+            #
+            # else:
+            # robot.board.set_motor_speed([[1, -0.3], [2, 0.3], [3, -0.3], [4, 0.3]])
 
 
 if __name__ == '__main__':
     my = Unibot()
```

### Comparing `unibot_hn-0.1.0/PKG-INFO` & `unibot_hn-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unibot_hn
-Version: 0.1.0
+Version: 0.1.1
 Summary: unibot_hn
 License: MIT
 Author: QuWan
 Requires-Python: >=3.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```

