# Comparing `tmp/nonebot-plugin-hx-yinying-1.0.4.tar.gz` & `tmp/nonebot-plugin-hx-yinying-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-hx-yinying-1.0.4.tar", last modified: Tue Apr 23 13:07:15 2024, max compression
+gzip compressed data, was "nonebot-plugin-hx-yinying-1.0.5.tar", last modified: Wed Apr 24 16:29:01 2024, max compression
```

## Comparing `nonebot-plugin-hx-yinying-1.0.4.tar` & `nonebot-plugin-hx-yinying-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 13:07:15.954148 nonebot-plugin-hx-yinying-1.0.4/
--rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     4083 2024-04-23 13:07:15.954148 nonebot-plugin-hx-yinying-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3643 2024-04-22 08:30:49.000000 nonebot-plugin-hx-yinying-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 13:07:15.822305 nonebot-plugin-hx-yinying-1.0.4/nonebot_plugin_hx_yinying/
--rw-rw-rw-   0        0        0    37733 2024-04-23 13:05:59.000000 nonebot-plugin-hx-yinying-1.0.4/nonebot_plugin_hx_yinying/__init__.py
--rw-rw-rw-   0        0        0    51005 2024-04-23 13:04:51.000000 nonebot-plugin-hx-yinying-1.0.4/nonebot_plugin_hx_yinying/chat.py
--rw-rw-rw-   0        0        0      434 2024-04-23 13:03:24.000000 nonebot-plugin-hx-yinying-1.0.4/nonebot_plugin_hx_yinying/config.py
-drwxrwxrwx   0        0        0        0 2024-04-23 13:07:15.906799 nonebot-plugin-hx-yinying-1.0.4/nonebot_plugin_hx_yinying.egg-info/
--rw-rw-rw-   0        0        0     4083 2024-04-23 13:07:15.000000 nonebot-plugin-hx-yinying-1.0.4/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-04-23 13:07:15.000000 nonebot-plugin-hx-yinying-1.0.4/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 13:07:15.000000 nonebot-plugin-hx-yinying-1.0.4/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      141 2024-04-23 13:07:15.000000 nonebot-plugin-hx-yinying-1.0.4/nonebot_plugin_hx_yinying.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-23 13:07:15.000000 nonebot-plugin-hx-yinying-1.0.4/nonebot_plugin_hx_yinying.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-23 13:07:15.970339 nonebot-plugin-hx-yinying-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      859 2024-04-23 13:06:51.000000 nonebot-plugin-hx-yinying-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:29:01.298565 nonebot-plugin-hx-yinying-1.0.5/
+-rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3487 2024-04-24 16:29:01.298565 nonebot-plugin-hx-yinying-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3047 2024-04-24 16:28:33.000000 nonebot-plugin-hx-yinying-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 16:29:01.165185 nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying/
+-rw-rw-rw-   0        0        0    43992 2024-04-24 16:03:12.000000 nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying/__init__.py
+-rw-rw-rw-   0        0        0    55886 2024-04-24 16:27:18.000000 nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying/chat.py
+-rw-rw-rw-   0        0        0      396 2024-04-24 16:19:18.000000 nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying/config.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:29:01.293431 nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying.egg-info/
+-rw-rw-rw-   0        0        0     3487 2024-04-24 16:29:00.000000 nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-04-24 16:29:00.000000 nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 16:29:00.000000 nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      141 2024-04-24 16:29:00.000000 nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-24 16:29:00.000000 nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-24 16:29:01.312319 nonebot-plugin-hx-yinying-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      859 2024-04-24 16:28:55.000000 nonebot-plugin-hx-yinying-1.0.5/setup.py
```

### Comparing `nonebot-plugin-hx-yinying-1.0.4/LICENSE` & `nonebot-plugin-hx-yinying-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.0.4/PKG-INFO` & `nonebot-plugin-hx-yinying-1.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.0.4
+Version: 1.0.5
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -93,56 +93,32 @@
 ### yinying_token
 
 - 类型：`str`
 - 默认值：`None`
 - 说明：这里写你找秩乱获取到的api_key
 - 重要：必填
 
-
-### hx_api_yinying(已于0.0.7版本移除)
-
-- 类型：`str`
-- 默认值：`None`
-- 说明：yinying的api地址
-- 重要：必填
-
-### yinying_model(已于0.0.7版本移除)
-
+### hx_path
 - 类型：`str`
 - 默认值：`None`
-- 说明：选择使用银影的模型
-- 注意 该配置项即将移除（转为插件内配置！）
+- 说明：这里是插件本地配置的存储目录
+- 重要：非必填
 
-## hx_path
-- 类型：`str`
+### SUPERUSERS
+- 类型：`list`
 - 默认值：`None`
-- 说明：银影对话的用户数据存储路径(不写将使用默认配置)
-
-## hx_reply(已于0.0.7版本移除)
-- 类型：`bool`
-- 默认值：`False`
-- 说明：bot发送chat消息时是否回复
-- 注意：该项启用时hx_reply_at将被忽略
-
-## hx_reply_at(已于0.0.7版本移除)
-- 类型：`bool`
-- 默认值：`False`
-- 说明：bot发送chat消息时不回复时是否艾特
-
-## yinying_limit(已于0.0.7版本移除)
-- 类型：`int`
-- 默认值：`12`
-- 说明：对于银影对话限制的次数
-
+- 说明：这里是超级管理员（插件）
+- 重要：必填（你需要这个来管理该插件）
 
 配置文件示例（默认模板）
 
 ```dotenv
 yinying_appid=你的appid
 yinying_token=你的token(不带bearer)
+hx_path=C:\Users\user\Desktop
 ```
 
 
 ## Contributors ✨
 
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.0.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.0.5 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
@@ -22,24 +22,16 @@
 [å®ç½é¾æ¥](https://chat.wingmark.cn/) . > [!WARNING] >
 è¯·æ³¨æï¼è¯¥é¡¹ç®æ¯æ¥å¥äºä¹±ä¹±çé¡¹ç®ï¼ä½ éè¦éµå®apiä½¿ç¨ç
 [è§è](https://wingmark.feishu.cn/docx/NFgJddgQAotygKxXiu6cpyg5nqr)ã
 éç½®æ¹å¼ï¼ç´æ¥å¨ NoneBot
 å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã ### yinying_appid -
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼ä½ çappid - éè¦ï¼å¿å¡«
 ### yinying_token - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
-è¯´æï¼è¿éåä½ æ¾ç§©ä¹±è·åå°çapi_key - éè¦ï¼å¿å¡« ###
-hx_api_yinying(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
-è¯´æï¼yinyingçapiå°å - éè¦ï¼å¿å¡« ### yinying_model
-(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
-è¯´æï¼éæ©ä½¿ç¨é¶å½±çæ¨¡å - æ³¨æ
-è¯¥éç½®é¡¹å³å°ç§»é¤ï¼è½¬ä¸ºæä»¶åéç½®ï¼ï¼ ## hx_path -
-ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
-è¯´æï¼é¶å½±å¯¹è¯çç¨æ·æ°æ®å­å¨è·¯å¾(ä¸åå°ä½¿ç¨é»è®¤éç½®)
-## hx_reply(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
-è¯´æï¼botåéchatæ¶æ¯æ¶æ¯å¦åå¤ -
-æ³¨æï¼è¯¥é¡¹å¯ç¨æ¶hx_reply_atå°è¢«å¿½ç¥ ## hx_reply_at
-(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
-è¯´æï¼botåéchatæ¶æ¯æ¶ä¸åå¤æ¶æ¯å¦è¾ç¹ ## yinying_limit
-(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`int` - é»è®¤å¼ï¼`12` -
-è¯´æï¼å¯¹äºé¶å½±å¯¹è¯éå¶çæ¬¡æ° éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼
-```dotenv yinying_appid=ä½ çappid yinying_token=ä½ çtoken(ä¸å¸¦bearer) ```
-## Contributors â¨
+è¯´æï¼è¿éåä½ æ¾ç§©ä¹±è·åå°çapi_key - éè¦ï¼å¿å¡« ### hx_path
+- ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
+è¯´æï¼è¿éæ¯æä»¶æ¬å°éç½®çå­å¨ç®å½ - éè¦ï¼éå¿å¡« ###
+SUPERUSERS - ç±»åï¼`list` - é»è®¤å¼ï¼`None` -
+è¯´æï¼è¿éæ¯è¶çº§ç®¡çåï¼æä»¶ï¼ -
+éè¦ï¼å¿å¡«ï¼ä½ éè¦è¿ä¸ªæ¥ç®¡çè¯¥æä»¶ï¼
+éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼ ```dotenv yinying_appid=ä½ çappid
+yinying_token=ä½ çtoken(ä¸å¸¦bearer) hx_path=C:\Users\user\Desktop ``` ##
+Contributors â¨
```

### Comparing `nonebot-plugin-hx-yinying-1.0.4/README.md` & `nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: nonebot-plugin-hx-yinying
+Version: 1.0.5
+Summary: chat with yinying
+Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
+Author: Huan Xin
+Author-email: mc.xiaolang@foxmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <!--
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
  * @Author         : huanxin996
  * @Date           : 2024-4-17
@@ -80,56 +93,32 @@
 ### yinying_token
 
 - 类型：`str`
 - 默认值：`None`
 - 说明：这里写你找秩乱获取到的api_key
 - 重要：必填
 
-
-### hx_api_yinying(已于0.0.7版本移除)
-
+### hx_path
 - 类型：`str`
 - 默认值：`None`
-- 说明：yinying的api地址
-- 重要：必填
-
-### yinying_model(已于0.0.7版本移除)
+- 说明：这里是插件本地配置的存储目录
+- 重要：非必填
 
-- 类型：`str`
+### SUPERUSERS
+- 类型：`list`
 - 默认值：`None`
-- 说明：选择使用银影的模型
-- 注意 该配置项即将移除（转为插件内配置！）
-
-## hx_path
-- 类型：`str`
-- 默认值：`None`
-- 说明：银影对话的用户数据存储路径(不写将使用默认配置)
-
-## hx_reply(已于0.0.7版本移除)
-- 类型：`bool`
-- 默认值：`False`
-- 说明：bot发送chat消息时是否回复
-- 注意：该项启用时hx_reply_at将被忽略
-
-## hx_reply_at(已于0.0.7版本移除)
-- 类型：`bool`
-- 默认值：`False`
-- 说明：bot发送chat消息时不回复时是否艾特
-
-## yinying_limit(已于0.0.7版本移除)
-- 类型：`int`
-- 默认值：`12`
-- 说明：对于银影对话限制的次数
-
+- 说明：这里是超级管理员（插件）
+- 重要：必填（你需要这个来管理该插件）
 
 配置文件示例（默认模板）
 
 ```dotenv
 yinying_appid=你的appid
 yinying_token=你的token(不带bearer)
+hx_path=C:\Users\user\Desktop
 ```
 
 
 ## Contributors ✨
 
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
```

#### html2text {}

```diff
@@ -1,11 +1,17 @@
-[![All Contributors](https://img.shields.io/badge/all_contributors-2-
-orange.svg?style=flat-square)](#contributors-) * @Author : huanxin996 * @Date :
-2024-4-17 * @LastEditors : huanxin996 * @LastEditTime : 2024-4-22 *
-@Description : None * @GitHub : https://github.com/huanxin996 -->
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.0.5 Summary:
+chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
+yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Description-Content-
+Type: text/markdown License-File: LICENSE [![All Contributors](https://
+img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
+(#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
+huanxin996 * @LastEditTime : 2024-4-22 * @Description : None * @GitHub : https:
+//github.com/huanxin996 -->
                                    _[_n_o_n_e_b_o_t_]
                 # nonebot_plugin_hx-yinying _â¨ Hx vs YinYing
                   (å¨çº¿ä¸é¶å½±è¿è¡å¯¹è¯çæä»¶) â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## å®è£ pipå®è£ ```dotenv pip install nonebot-plugin-hx-yinying ``` nb
 pluginå®è£ ```dotenv nb plugin install nonebot-plugin-hx-yinying ``` ##
 ä½¿ç¨æ¹å¼ éç¨: - @Bot æèåå¤å³å¯ OneBot: - @Bot - åå¤Bot ##
@@ -16,24 +22,16 @@
 [å®ç½é¾æ¥](https://chat.wingmark.cn/) . > [!WARNING] >
 è¯·æ³¨æï¼è¯¥é¡¹ç®æ¯æ¥å¥äºä¹±ä¹±çé¡¹ç®ï¼ä½ éè¦éµå®apiä½¿ç¨ç
 [è§è](https://wingmark.feishu.cn/docx/NFgJddgQAotygKxXiu6cpyg5nqr)ã
 éç½®æ¹å¼ï¼ç´æ¥å¨ NoneBot
 å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã ### yinying_appid -
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼ä½ çappid - éè¦ï¼å¿å¡«
 ### yinying_token - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
-è¯´æï¼è¿éåä½ æ¾ç§©ä¹±è·åå°çapi_key - éè¦ï¼å¿å¡« ###
-hx_api_yinying(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
-è¯´æï¼yinyingçapiå°å - éè¦ï¼å¿å¡« ### yinying_model
-(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
-è¯´æï¼éæ©ä½¿ç¨é¶å½±çæ¨¡å - æ³¨æ
-è¯¥éç½®é¡¹å³å°ç§»é¤ï¼è½¬ä¸ºæä»¶åéç½®ï¼ï¼ ## hx_path -
-ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
-è¯´æï¼é¶å½±å¯¹è¯çç¨æ·æ°æ®å­å¨è·¯å¾(ä¸åå°ä½¿ç¨é»è®¤éç½®)
-## hx_reply(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
-è¯´æï¼botåéchatæ¶æ¯æ¶æ¯å¦åå¤ -
-æ³¨æï¼è¯¥é¡¹å¯ç¨æ¶hx_reply_atå°è¢«å¿½ç¥ ## hx_reply_at
-(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
-è¯´æï¼botåéchatæ¶æ¯æ¶ä¸åå¤æ¶æ¯å¦è¾ç¹ ## yinying_limit
-(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`int` - é»è®¤å¼ï¼`12` -
-è¯´æï¼å¯¹äºé¶å½±å¯¹è¯éå¶çæ¬¡æ° éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼
-```dotenv yinying_appid=ä½ çappid yinying_token=ä½ çtoken(ä¸å¸¦bearer) ```
-## Contributors â¨
+è¯´æï¼è¿éåä½ æ¾ç§©ä¹±è·åå°çapi_key - éè¦ï¼å¿å¡« ### hx_path
+- ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
+è¯´æï¼è¿éæ¯æä»¶æ¬å°éç½®çå­å¨ç®å½ - éè¦ï¼éå¿å¡« ###
+SUPERUSERS - ç±»åï¼`list` - é»è®¤å¼ï¼`None` -
+è¯´æï¼è¿éæ¯è¶çº§ç®¡çåï¼æä»¶ï¼ -
+éè¦ï¼å¿å¡«ï¼ä½ éè¦è¿ä¸ªæ¥ç®¡çè¯¥æä»¶ï¼
+éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼ ```dotenv yinying_appid=ä½ çappid
+yinying_token=ä½ çtoken(ä¸å¸¦bearer) hx_path=C:\Users\user\Desktop ``` ##
+Contributors â¨
```

### Comparing `nonebot-plugin-hx-yinying-1.0.4/nonebot_plugin_hx_yinying/__init__.py` & `nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     get_config_global,
     send_msg_reject,
     easycyber_in,
     json_replace,
     json_get_text,
     easycyber_in_tg,
     place,
+    config_list,
 )
 
 __plugin_meta__ = PluginMetadata(
     name="Hx_YinYing",
     description="快来和可爱的赛博狼狼聊天！",
     usage=(
         "通过QQ艾特机器人来进行对话"
@@ -54,15 +55,15 @@
     },
 )
 
 
 hx_config = get_plugin_config(Config)
 log_dir = path_in()
    
-new_verision = update_hx()
+new_verision, time = update_hx()
 if new_verision <= hx_config.hx_version:
     logger.success(f"[Hx_YinYing]:你的Hx_YinYing已经是最新版本了！当前版本为{hx_config.hx_version}")
 else:
     logger.success("[Hx_YinYing]:检查到Hx_YinYing有新版本！")
     logger.warning("【Hx】正在自动更新中")
     os.system(f'pip install nonebot-plugin-hx-yinying=={new_verision} -i https://pypi.Python.org/simple/')
     logger.success(f"[Hx_YinYing]:更新完成！最新版本为{new_verision}|当前使用版本为{hx_config.hx_version}")
@@ -85,14 +86,90 @@
 model_handoff = on_command("切换模型", aliases={"qhmodel","切换chat模型"}, priority=0, block=True)
 rule_reply = on_command("对话回复", aliases={"chat回复"}, priority=0, block=True)
 rule_reply_at = on_command("回复艾特", aliases={"chat回复艾特"}, priority=0, block=True)
 private = on_command("私聊回复", aliases={"私聊chat"}, priority=0, block=True)
 at_reply = on_command("艾特回复", aliases={"bot艾特回复"}, priority=0, block=True)
 easycyber_set = on_command("easycyber", aliases={"easycyber设置","hxworld"}, priority=0, block=True)
 admin_set = on_command("控制台操作", aliases={"管理控制台","setstart"}, priority=0, block=True)
+verision = on_command("确认版本", aliases={"旅行伙伴确认","版本确认"}, priority=0, block=True)
+character = on_command("sd", aliases={"旅行伙伴加入","设定加入"}, priority=0, block=True)
+
+@character.handle()
+async def verision_get(matcher: Matcher,bot:Bot, event: MessageEvent, events:Event, msg: Message = CommandArg()):
+    user = get_id(event)
+    nick = await get_nick(bot,event)
+    config = config_in_user(user,nick)
+    config_get = json_get(config,user)
+    text = msg.extract_plain_text()
+    if text == "" or text == None:
+        msg = "没有获取到要加入伙伴的设定哦"
+        await send_msg(matcher, event, msg)
+    else:
+        try:
+            msg = text.split(" ")
+            if int(len(msg)) == 1:
+                config_get["nick"] = nick
+                config_get["character"] = text
+                config[f"{user}"] = config_get
+                with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
+                    json.dump(config,file)
+                    msg = f"{nick}加入成功"
+            elif int(len(msg)) == 2:
+                config_get["nick"] = msg[1]
+                config_get["character"] = msg[0]
+                config[f"{user}"] = config_get
+                with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
+                    json.dump(config,file)
+                    msg = f"{msg[0]}加入成功！"
+            else:
+                msg = "没有获取到要加入伙伴的设定哦"
+            await send_msg(matcher, event, msg)
+        except Exception as e:
+            msg = False
+            logger.opt(colors=True).error(f"{e}")
+        
+@verision.handle()
+async def verision_get(matcher: Matcher, event: MessageEvent, events:Event):
+    new_verision, time = update_hx()
+    if isinstance(events, GroupMessageEvent):
+        config = json_get(config_in_group(get_groupid(event)),get_groupid(event))
+        model = json_get(config,"use_model")
+        if new_verision > hx_config.hx_version:
+            if model == "easycyberfurry-001":
+                model_in = json_get(config,"easycharacter_in")
+                if model_in or not model_in:
+                    msg =f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[已过时(]\n你的插件版本已过时，当前最新版本为v{new_verision}\n当前群聊使用模型:{model}\n当前模型载入角色:Hx\n最后更新时间:====>\n{time}\n======================"
+                msg = f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[已过时(]\n你的插件版本已过时，当前最新版本为v{new_verision}\n当前群聊使用模型:{model}\n当前模型载入角色:{model_in}\n最后更新时间:====>\n{time}\n======================"
+            msg = f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[已过时(]\n你的插件版本已过时，当前最新版本为v{new_verision}\n当前群聊使用模型:{model}\n最后更新时间:====>\n{time}\n======================"
+        else:
+            if model == "easycyberfurry-001":
+                model_in = json_get(config,"easycharacter_in")
+                if model_in or not model_in:
+                    msg =f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前群聊使用模型:{model}\n当前模型载入角色:Hx\n最后更新时间:====>\n{time}\n======================"
+                msg = f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前群聊使用模型:{model}\n当前模型载入角色:{model_in}\n最后更新时间:====>\n{time}\n======================"
+            msg = f"(点头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前群聊使用模型:\n最后更新时间:====>\n{time}\n======================"
+        await send_msg(matcher, event, msg)
+    else:
+        config = json_get(config_in_user(get_id(event),False),get_id(event))
+        model = json_get(config,"private_model")
+        if new_verision > hx_config.hx_version:
+            if model == "easycyberfurry-001":
+                model_in = json_get(config,"easycharacter_in")
+                if model_in or not model_in:
+                    msg =f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[已过时(]\n你的插件版本已过时，当前最新版本为v{new_verision}\n当前私聊使用模型:{model}\n当前模型载入角色:Hx\n最后更新时间:====>\n{time}\n======================"
+                msg = f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[已过时(]\n你的插件版本已过时，当前最新版本为v{new_verision}\n当前私聊使用模型:{model}\n当前模型载入角色:{model_in}\n最后更新时间:====>\n{time}\n======================"
+            msg = f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[已过时(]\n你的插件版本已过时，当前最新版本为v{new_verision}\n当前私聊使用模型:{model}\n最后更新时间:====>\n{time}\n======================"
+        else:
+            if model == "easycyberfurry-001":
+                model_in = json_get(config,"easycharacter_in")
+                if model_in or not model_in:
+                    msg =f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前私聊使用模型:{model}\n当前模型载入角色:Hx\n最后更新时间:====>\n{time}\n======================"
+                msg = f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前私聊使用模型:{model}\n当前模型载入角色:{model_in}\n最后更新时间:====>\n{time}\n======================"
+            msg = f"(点头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前私聊使用模型:\n最后更新时间:====>\n{time}\n======================"
+        await send_msg(matcher, event, msg)
 
 @msg_at.handle()
 async def at(matcher: Matcher, event: MessageEvent, bot: Bot, events:Event):
     config_global = config_in_global()
     at_reply = json_get(config_global,"at_reply")
     if not at_reply:
         logger.opt(colors=True).warning("由于艾特回复被设置为false，此条消息忽略")
@@ -122,175 +199,164 @@
 @set_global_config.got(
     "msg",
     prompt=f"发送以下选项执行相应功能\n修改 #修改全局配置项\n查看 #查看全局配置项\n追加 #向全局配置里追加配置项，通常用于插件更新后配置不存在导致的出错\n查看所有配置 #列出所有全局配置\n发送非预期命令则退出",
 )
 async def set_global(matcher: Matcher, bot:Bot, event: MessageEvent,events: Event, s: T_State):
     id = get_id(event)
     text = unescape(event.get_plaintext().strip())
-    if isinstance(events, GroupMessageEvent):
-        if "last" not in s:
-            s["last"] = ""
-        if s["last"]:
-            if s["last"] == "查看":
-                config = config_in_global()
-                get_config = json_get_text(config,text)
-                if get_config == None:
-                    s["last"] = True
-                    msg = f"无法查找到该配置项！，请检查其是否为正确的配置名{text}"
-                    await send_msg(matcher,event,msg)
+    if "last" not in s:
+        s["last"] = ""
+    if s["last"]:
+        if s["last"] == "查看":
+            config = config_in_global()
+            get_config = json_get_text(config,text)
+            if get_config == 0:
+                s["last"] = True
+                msg = f"无法查找到该配置项！，请检查其是否为正确的配置名{text}"
+                await send_msg(matcher,event,msg)
+            else:
                 s["last"] = True
                 msg = f"{text}状态为:{get_config}"
                 await send_msg(matcher,event,msg)
 
-            if s["last"] == "修改":
-                config = config_in_global()
-                get_config = json_get_text(config,text)
-                if get_config == None:
-                    s["last"] = True
-                    msg = "无法查找到该配置项！，请检查其是否为正确的配置名"
-                    await send_msg(matcher,event,msg)
-                s["last"] = "修改next"
-                s["set"] = text
-                msg = "请发送开启或关闭【也可以是on或者off或者开和关】"
-                await send_msg_reject(matcher,event,msg)
-
-            if s["last"] == "修改next":
-                config = config_in_global()
-                config_name = s["set"]
-                get_config = json_get_text(config,config_name)
-                if text == "on" or text == "开" or text == True:
-                    set = True
-                elif text == "off" or text == "关" or text == False:
-                    set = False
-                text = set
+        if s["last"] == "修改":
+            config = config_in_global()
+            get_config = json_get_text(config,text)
+            if get_config == 0:
+                s["last"] = True
+                msg = "无法查找到该配置项！，请检查其是否为正确的配置名"
+                await send_msg(matcher,event,msg)
+            else:
+                TFkey, Wkey, Listkey, app_key = config_list(config)
+                if text in TFkey:
+                    s["last"] = "修改TF"
+                    s["set"] = text
+                    msg = "请发送开启或关闭【也可以是on或者off或者开和关】"
+                    await send_msg_reject(matcher,event,msg)
+                elif text in Wkey:
+                    s["last"] = "修改w"
+                    s["set"] = text
+                    msg = "请发送id（群号或者QQ号，看你改哪个配置项）"
+                    await send_msg_reject(matcher,event,msg)
+                elif text in Listkey:
+                    s["last"] = "updata_LK"
+                    s["set"] = text
+                    msg = "请发送添加或删除【也可以是增加或者移除】"
+                    await send_msg_reject(matcher,event,msg)
+                else:
+                    return
+        
+        if s["last"] == "修改TF":
+            config = config_in_global()
+            config_name = s["set"]
+            get_config = json_get_text(config,config_name)
+            if text == "on" or text == "开" or text == True:
+                text = True
+            elif text == "off" or text == "关" or text == False:
+                text = False
                 if get_config and text:
                     msg = f"该配置项[{config_name}]已经开启了，不需要重复开启噢"
                 elif not get_config and not text:
                     msg = f"该配置项[{config_name}]已经关闭了，不需要重复关闭噢"
                 elif text:
                     config[f"{config_name}"] = True
                     with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
                         json.dump(config,file)
                     msg = f"{config_name}的状态已更改为{text}"
                 elif not text:
                     config[f"{config_name}"] = False
                     with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
                         json.dump(config,file)
                     msg = f"{config_name}的状态已更改为{text}"
-                s["last"] = True
-                if msg == None:
-                    msg = "未知的状态信息"
-                await send_msg(matcher,event,msg)
-        #查看
-        if text == "查看" or text == "查看配置":
-            s["last"] = "查看"
-            msg = "请输入配置项(具体名称)\n【ps:如果不知道建议先查看所有配置一下,[]内为具体名称】"
-            await send_msg_reject(matcher,event,msg)
+            s["last"] = True
+            if text == "退出":
+                msg = "已退出"
+            await send_msg(matcher,event,msg)        
         
-        if text == "修改" or text == "修改配置":
-            s["last"] = "修改"
-            msg = "请输入配置项(具体名称)\n【ps:如果不知道建议先查看所有配置一下,[]内为具体名称】"
-            await send_msg_reject(matcher,event,msg)
-
-        if text == "追加" or text == "追加配置":
+        if s["last"] == "修改w":
+            config = config_in_global()
+            config_name = s["set"]
+            get_config = json_get_text(config,config_name)
+            config[f"{config_name}"] = text
+            with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
+                json.dump(config,file)
+            msg = f"{config_name}的id已更改为{text}"
             s["last"] = True
-            msg = "在写了在写了😭"
             await send_msg(matcher,event,msg)
 
-        if text == "查看所有配置":
-            msg_list = await get_config_global()
-            s["last"] = True
-            await bot.send_group_forward_msg(group_id=event.group_id, messages=msg_list)
-
-        # 退出
-        if s["last"]:
-            return
-        else:
-            msg = f"未知命令“{text}”，已退出"
-            await send_msg(matcher,event,msg)
-    else:
-        if "last" not in s:
-            s["last"] = ""
-        if s["last"]:
-            if s["last"] == "查看":
-                config = config_in_global()
-                get_config = json_get_text(config,text)
-                if get_config == None:
-                    s["last"] = True
-                    msg = f"无法查找到该配置项！，请检查其是否为正确的配置名{text}"
-                    await send_msg(matcher,event,msg)
+        if s["last"] == "updata_LK":
+            s["type"] = text
+            if text == "增加" or text == "添加":
+                s["last"] = "修改LKt"
+                msg = "请发送要添加的id(存在时会失败！)"
+            elif text == "移除" or text == "删除":
+                s["last"] = "修改LKt"
+                msg = "请发送要删除的id(不存在时会失败！)"
+            else:
                 s["last"] = True
-                msg = f"{text}状态为:{get_config}"
-                await send_msg(matcher,event,msg)
-
-            if s["last"] == "修改":
-                config = config_in_global()
-                get_config = json_get_text(config,text)
-                if get_config == None:
-                    s["last"] = True
-                    msg = "无法查找到该配置项！，请检查其是否为正确的配置名"
-                    await send_msg(matcher,event,msg)
-                s["last"] = "修改next"
-                s["set"] = text
-                msg = "请发送开启或关闭【也可以是on或者off或者开和关】"
-                await send_msg_reject(matcher,event,msg)
+                msg = "未知方式"
+            await send_msg_reject(matcher,event,msg)
 
-            if s["last"] == "修改next":
-                config = config_in_global()
-                config_name = s["set"]
-                get_config = json_get_text(config,config_name)
-                if text == "on" or text == "开" or text == True:
-                    set = True
-                elif text == "off" or text == "关" or text == False:
-                    set = False
-                text = set
-                if get_config and text:
-                    msg = f"该配置项[{config_name}]已经开启了，不需要重复开启噢"
-                elif not get_config and not text:
-                    msg = f"该配置项[{config_name}]已经关闭了，不需要重复关闭噢"
-                elif text:
-                    config[f"{config_name}"] = True
+        if s["last"] == "修改LKt":
+            config_name = s["set"]
+            config_set_type = s["type"]
+            s["last"] = True
+            config = config_in_global()
+            config_get = json_get(config,config_name)
+            if config_set_type == "增加" or config_set_type == "添加":
+                if text in config_get:
+                    msg = "该id已经在这个配置项里了，不可以重复添加哦"
+                else:
+                    config_get.append(text)
+                    config["config_name"] = config_get
                     with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
                         json.dump(config,file)
-                    msg = f"{config_name}的状态已更改为{text}"
-                elif not text:
-                    config[f"{config_name}"] = False
+                        msg = "该id已添加在这个配置项里"
+            elif config_set_type == "移除" or config_set_type == "删除":
+                if text not in config_get:
+                    msg = "该id不在这个配置项里，无法重复删除"
+                else:
+                    config_get.remove(text)
+                    config["config_name"] = config_get
                     with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
                         json.dump(config,file)
-                    msg = f"{config_name}的状态已更改为{text}"
-                s["last"] = True
-                if msg == None:
-                    msg = "未知的状态信息"
-                await send_msg(matcher,event,msg)
-        #查看
-        if text == "查看" or text == "查看配置":
-            s["last"] = "查看"
-            msg = "请输入配置项(具体名称)\n【ps:如果不知道建议先查看所有配置一下,[]内为具体名称】"
-            await send_msg_reject(matcher,event,msg)
+                        msg = "该id已在这个配置项里被移除"
+            await send_msg(matcher,event,msg) 
         
-        if text == "修改" or text == "修改配置":
-            s["last"] = "修改"
-            msg = "请输入配置项(具体名称)\n【ps:如果不知道建议先查看所有配置一下,[]内为具体名称】"
-            await send_msg_reject(matcher,event,msg)
+        
+    #查看
+    if text == "查看" or text == "查看配置":
+        s["last"] = "查看"
+        msg = "请输入配置项(具体名称)\n【ps:如果不知道建议先查看所有配置一下,[]内为具体名称】"
+        await send_msg_reject(matcher,event,msg)
+    
+    if text == "修改" or text == "修改配置":
+        s["last"] = "修改"
+        msg = "请输入配置项(具体名称)\n【ps:如果不知道建议先查看所有配置一下,[]内为具体名称】"
+        await send_msg_reject(matcher,event,msg)
 
-        if text == "追加" or text == "追加配置":
-            s["last"] = True
-            msg = "在写了在写了😭"
-            await send_msg(matcher,event,msg)
+    if text == "追加" or text == "追加配置":
+        s["last"] = True
+        msg = "在写了在写了😭"
+        await send_msg(matcher,event,msg)
 
-        if text == "查看所有配置":
-            msg_list = await get_config_global()
-            s["last"] = True
-            await bot.send_private_forward_msg(user_id=id, messages=msg_list)
-        # 退出
-        if s["last"]:
-            return
+    if text == "查看所有配置":
+        msg_list = await get_config_global()
+        s["last"] = True
+        if isinstance(events, GroupMessageEvent):
+            await bot.send_group_forward_msg(group_id=event.group_id, messages=msg_list)
         else:
-            msg = f"未知命令“{text}”，已退出"
-            await send_msg(matcher,event,msg)
+            await bot.send_private_forward_msg(user_id=id, messages=msg_list)
+
+    # 退出
+    if s["last"]:
+        return
+    else:
+        msg = f"未知命令“{text}”，已退出"
+        await send_msg(matcher,event,msg)
 
 @history_get.handle()
 async def history(bot: Bot, event: MessageEvent,events: Event):
     id = get_id(events)
     msg_list = await get_history(id,bot,event)
     if isinstance(events, GroupMessageEvent):
         await bot.send_group_forward_msg(group_id=event.group_id, messages=msg_list)  # type: ignore
@@ -505,27 +571,29 @@
         s["last"] = ""
     if s["last"]:
         if s["last"] == "增加":
             if text == "Hx" or text == "HX" or text == "幻歆":
                 s["last"] = True
                 msg = "easycyber预设“Hx”不能删除或修改，如要改动请改源码"
                 await send_msg(matcher,event,msg)
-            s["cfnickname"] = text
-            s["last"] = "cfSpecies"
-            msg = "请输入角色物种"
-            await send_msg_reject(matcher,event,msg)
+            else:
+                s["cfnickname"] = text
+                s["last"] = "cfSpecies"
+                msg = "请输入角色物种"
+                await send_msg_reject(matcher,event,msg)
         if s["last"] == "cfSpecies":
             if text == "退出":
                 s["last"] = True
                 msg = "已退出"
                 await send_msg(matcher,event,msg)
-            s["cfSpecies"] = text
-            s["last"] = "cfconage"
-            msg = "请输入角色表现:(比如\n child--[幼年]\n young--[青年]\n adult--[成年]\nps:只输入--前面的英文即可"
-            await send_msg_reject(matcher,event,msg)
+            else:
+                s["cfSpecies"] = text
+                s["last"] = "cfconage"
+                msg = "请输入角色表现:(比如\n child--[幼年]\n young--[青年]\n adult--[成年]\nps:只输入--前面的英文即可"
+                await send_msg_reject(matcher,event,msg)
 
         if s["last"] == "cfconage":
             if text == "退出":
                 s["last"] = True
                 msg = "已退出"
                 await send_msg(matcher,event,msg)
             key = ['child','young','adult']
@@ -556,135 +624,157 @@
                 await send_msg_reject(matcher,event,msg)
 
         if s["last"] == "cfstory":
             if text == "退出":
                 s["last"] = True
                 msg = "已退出"
                 await send_msg(matcher,event,msg)
-            s["cfstory"] = text
-            s["last"] = "public"
-            msg = "该角色是否公开？(最后一步)完成将发送到bot管理站进行审核，审核通过后即可使用"
-            await send_msg_reject(matcher,event,msg)
+            else:
+                s["cfstory"] = text
+                s["last"] = "public"
+                msg = "该角色是否公开？(最后一步)完成将发送到bot管理站进行审核，审核通过后即可使用"
+                await send_msg_reject(matcher,event,msg)
 
         if s["last"] == "public":
             if text == "退出":
                 s["last"] = True
                 msg = "已退出"
                 await send_msg(matcher,event,msg)
-            name = s["cfnickname"]
-            species = s["cfSpecies"]
-            age = s["cfconage"]
-            stytle = s["cfconstyle"]
-            story = s["cfstory"]
-            easycyber_package["cfNickname"] = s["cfnickname"]
-            easycyber_package["cfSpecies"] = s["cfSpecies"]
-            easycyber_package["cfConAge"] = s["cfconage"]
-            easycyber_package["cfConStyle"] = s["cfconstyle"]
-            easycyber_package["cfStory"] = s["cfstory"]
-            easycyber_package["public"] = text
-            easycyber_package["creator"] = id
-            s["last"] = True
-            cybernick = s["cfnickname"]
-            if not json_get(config_in_global(),"admin_pro") and not json_get(config_in_global(),"admin_group"):
-                msg ="bot管理者未配置，超级管理员和bot控制台,审核失败！"
-            elif json_get(config_in_global(),"admin_pro") == None and json_get(config_in_global(),"admin_group") == None:
-                msg ="bot管理者未配置，超级管理员和bot控制台,审核失败！"
-            elif json_get(config_in_global(),"admin_pro") == None and json_get(config_in_global(),"admin_group_switch"):
-                easycyber_in_tg(cybernick,easycyber_package)
-                groupid = json_get(config_in_global(),"admin_group")
-                msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\n物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
-                await bot.call_api("send_group_msg",group_id=groupid, message=msg_tg)
-                msg = "投稿成功！，等待审核(问就是权限还没写好)]"
-            elif json_get(config_in_global(),"admin_group") == None and json_get(config_in_global(),"admin_user_switch"):
-                easycyber_in_tg(cybernick,easycyber_package)
-                adminid = json_get(config_in_global(),"admin_pro")
-                msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
-                await bot.call_api("send_private_msg",user_id=adminid, messages=msg_tg)
-                msg = "投稿成功！，等待审核(问就是权限还没写好)]"
-            elif json_get(config_in_global(),"admin_user_switch") and json_get(config_in_global(),"admin_group_switch"):
-                easycyber_in_tg(cybernick,easycyber_package)
-                groupid = json_get(config_in_global(),"admin_group")
-                adminid = json_get(config_in_global(),"admin_pro")
-                msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
-                await bot.call_api("send_group_msg",group_id=groupid, message=msg_tg)
-                await bot.call_api("send_private_msg",user_id=adminid, messages=msg_tg)
-                msg = "投稿成功！，等待审核(问就是权限还没写好)]"
-            elif json_get(config_in_global(),"admin_user_switch"):
-                easycyber_in_tg(cybernick,easycyber_package)
-                adminid = json_get(config_in_global(),"admin_pro")
-                msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
-                await bot.call_api("send_private_msg",user_id=adminid, messages=msg_tg)
-            else:
-                easycyber_in_tg(cybernick,easycyber_package)
-                groupid = json_get(config_in_global(),"admin_group")
-                msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\n物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
-                await bot.call_api("send_group_msg",group_id=groupid, message=msg_tg)
-                msg = "投稿成功！，等待审核(问就是权限还没写好)]"
-            await send_msg(matcher,event,msg)
+            else:
+                name = s["cfnickname"]
+                species = s["cfSpecies"]
+                age = s["cfconage"]
+                stytle = s["cfconstyle"]
+                story = s["cfstory"]
+                easycyber_package["cfNickname"] = s["cfnickname"]
+                easycyber_package["cfSpecies"] = s["cfSpecies"]
+                easycyber_package["cfConAge"] = s["cfconage"]
+                easycyber_package["cfConStyle"] = s["cfconstyle"]
+                easycyber_package["cfStory"] = s["cfstory"]
+                easycyber_package["public"] = text
+                easycyber_package["creator"] = id
+                s["last"] = True
+                cybernick = s["cfnickname"]
+                g = json_get(config_in_global(),"admin_group")
+                u = json_get(config_in_global(),"admin_pro")
+                g_k = json_get(config_in_global(),"admin_group_switch")
+                u_k = json_get(config_in_global(),"admin_user_switch")
+                if not g and u:
+                    logger.opt(colors=True).success(f"{g},{u}")
+                    msg ="bot管理者未配置，超级管理员和bot控制台,审核失败！"
+                elif u == None and g == None:
+                    logger.opt(colors=True).success("false")
+                    msg ="bot管理者未配置，超级管理员和bot控制台,审核失败！"
+                elif u == None and g_k:
+                    easycyber_in_tg(cybernick,easycyber_package)
+                    groupid = json_get(config_in_global(),"admin_group")
+                    msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\n物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
+                    await bot.call_api("send_group_msg",group_id=groupid, message=msg_tg)
+                    msg = "投稿成功！，等待审核(问就是权限还没写好)]"
+                elif g == None and u_k:
+                    easycyber_in_tg(cybernick,easycyber_package)
+                    adminid = json_get(config_in_global(),"admin_pro")
+                    msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
+                    await bot.call_api("send_private_msg",user_id=adminid, messages=msg_tg)
+                    msg = "投稿成功！，等待审核(问就是权限还没写好)]"
+                elif u_k and g_k:
+                    easycyber_in_tg(cybernick,easycyber_package)
+                    groupid = json_get(config_in_global(),"admin_group")
+                    adminid = json_get(config_in_global(),"admin_pro")
+                    msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
+                    await bot.call_api("send_group_msg",group_id=groupid, message=msg_tg)
+                    await bot.call_api("send_private_msg",user_id=adminid, messages=msg_tg)
+                    msg = "投稿成功！，等待审核(问就是权限还没写好)]"
+                elif g_k:
+                    easycyber_in_tg(cybernick,easycyber_package)
+                    adminid = json_get(config_in_global(),"admin_pro")
+                    msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
+                    await bot.call_api("send_private_msg",user_id=adminid, messages=msg_tg)
+                else:
+                    easycyber_in_tg(cybernick,easycyber_package)
+                    groupid = json_get(config_in_global(),"admin_group")
+                    msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\n物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
+                    await bot.call_api("send_group_msg",group_id=groupid, message=msg_tg)
+                    msg = "投稿成功！，等待审核(问就是权限还没写好)]"
+                await send_msg(matcher,event,msg)
 
 
         if s["last"] == "载入":
             if text == "退出":
                 s["last"] = True
                 msg = "已退出"
                 await send_msg(matcher,event,msg)
-            s["last"] = True
-            if isinstance(events, GroupMessageEvent):
-                groupid = event.group_id
-                config_user = config_in_group(id,False)
-                user = json_get(config_user,f"{id}")
-                promte = json_get(easycyber_in(False,False),f"{text}")
-                public = json_get(promte,"public")
-                if not public:
-                    msg = f"{text}模型拒绝被加载(可能是模型不存在或者模型非公开！)"      
-                else:
-                    if user["character_in"]== text:
-                        msg = f"{text}模型已加载，请勿重新加载"  
+            else:
+                s["last"] = True
+                if isinstance(events, GroupMessageEvent):
+                    groupid = get_groupid(event)
+                    config = config_in_group(groupid)
+                    config_group = json_get(config,groupid)
+                    promte = json_get(easycyber_in(False,False),f"{text}")
+                    public = json_get(promte,"public")
+                    if not public:
+                        msg = f"{text}模型拒绝被加载(可能是模型不存在或者模型非公开！)"      
                     else:
-                        user["character_in"] = f"{text}"
-                        config_user[f"{id}"] = user
-                        with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
-                            json.dump(config_user,file)
-                            msg = f"{text}加载成功！" 
-            else:
-                config_user = config_in_user(id,False)
-                user = json_get(config_user,f"{id}")
-                promte = json_get(easycyber_in(False,False),f"{text}")
-                public = json_get(promte,"public")
-                if not public:
-                    msg = f"{text}模型拒绝被加载(可能是模型不存在或者模型非公开！)"      
+                        if config_group["character_in"] == text:
+                            msg = f"{text}模型已加载，请勿重新加载"  
+                        else:
+                            config_group["character_in"] = f"{text}"
+                            config[f"{groupid}"] = config_group
+                            with open(f'{log_dir}/config/config_group.json','w',encoding='utf-8') as file:
+                                json.dump(config,file)
+                                msg = f"{text}加载成功！" 
                 else:
-                    if user["character_in"]== text:
-                        msg = f"{text}模型已加载，请勿重新加载"  
+                    config_user = config_in_user(id,False)
+                    user = json_get(config_user,f"{id}")
+                    promte = json_get(easycyber_in(False,False),f"{text}")
+                    public = json_get(promte,"public")
+                    creator = json_get(promte,"creator")
+                    if creator == id:
+                        if user["character_in"]== text:
+                            msg = f"{text}模型已加载，请勿重新加载"  
+                        else:
+                            user["character_in"] = f"{text}"
+                            config_user[f"{id}"] = user
+                            with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
+                                json.dump(config_user,file)
+                                msg = f"{text}加载成功！"
+                    elif not public:
+                        msg = f"{text}模型拒绝被加载(可能是模型不存在或者模型非公开！)"      
                     else:
-                        user["character_in"] = f"{text}"
-                        config_user[f"{id}"] = user
-                        with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
-                            json.dump(config_user,file)
-                            msg = f"{text}加载成功！" 
-            await send_msg(matcher,event,msg)
+                        if user["character_in"] == text:
+                            msg = f"{text}模型已加载，请勿重新加载"  
+                        else:
+                            user["character_in"] = f"{text}"
+                            config_user[f"{id}"] = user
+                            with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
+                                json.dump(config_user,file)
+                                msg = f"{text}加载成功！" 
+                await send_msg(matcher,event,msg)
     # 增加预设
     if text == "投稿":
         s["last"] = "增加"
         msg = "请输入角色昵称"
         await send_msg_reject(matcher,event,msg)
     if text == "载入":
         s["last"] = "载入"
         msg = "请输入公开的角色昵称【非公开会载入失败！】"
         await send_msg_reject(matcher,event,msg)
     if text == "查看列表":
         s["last"] = True
         list_in = easycyber_in(False,False)
-        list_got = []
-        for key in list_in:
-            if list_in[f"{key}"]["public"]:
-                list_got.append(format(key))
-            else:
-                return
-        msg = f"{list_got}"
+        try:
+            list_got = []
+            for key in list_in:
+                if list_in[f"{key}"]["public"]:
+                    list_got.append(format(key))
+                else:
+                    return
+            msg = f"{list_got}"
+        except Exception as e:
+            msg = "当前没有公开的角色哦"
         await send_msg(matcher,event,msg)
     # 退出
     if s["last"]:
         return
     else:
         msg = f"未知命令“{text}”，已退出"
         await send_msg(matcher,event,msg)
@@ -697,62 +787,55 @@
     id = get_id(event)
     text = unescape(event.get_plaintext().strip())
     place_user = place(id)
     if place_user >= 9:
         if "last" not in s:
             s["last"] = ""
         if s["last"]:
-            if s["last"] == "通过":
-                if text == "Hx" or text == "HX" or text == "幻歆":
-                    s["last"] = True
-                    msg = "easycyber预设“Hx”不能删除或修改，如要改动请改源码"
-                    await send_msg(matcher,event,msg)
-                s["last"] = True
-                json_data = easycyber_in_tg(False,False)
+            if s["last"] == "通过1":
+                json_1 = easycyber_in_tg(False,False)
+                json_data = json_get(json_1,text)
                 json_data["tg_admin"] = id
                 user = json_data["creator"]
-                easycyber_in(text,json_data)
-                del json_data[f"{text}"]
+                in_ok = easycyber_in(text,json_data)
+                end_json = json_1.pop(f"{text}")
                 with open(f'{log_dir}/file/easycyber_tg.json','w',encoding='utf-8') as file:
-                    json.dump(json_data,file)
+                    json.dump(json_1,file)
+                    s["last"] = True
                     msg = f"已通过投稿用户为{user}关于角色{text}的投稿"
                 await send_msg(matcher,event,msg)
 
             if s["last"] == "拒绝":
                 s["last"] = True
-                json_data = easycyber_in_tg(False,False)
+                json_1 = easycyber_in_tg(False,False)
+                json_data = json_get(json_1,text)
                 user = json_data["creator"]
-                del json_data[f"{text}"]
+                end_json = json_1.pop(f"{text}")
                 with open(f'{log_dir}/file/easycyber_tg.json','w',encoding='utf-8') as file:
-                    json.dump(json_data,file)
+                    json.dump(json_1,file)
                     msg = f"已拒绝投稿用户为{user}关于角色{text}的投稿"
                 await send_msg(matcher,event,msg)
-            await send_msg_reject(matcher,event,msg)
-
 
         if text == "通过":
-            s["last"] = "通过"
+            s["last"] = "通过1"
             msg = "请输入要加入角色昵称"
-        await send_msg_reject(matcher,event,msg)
+            await send_msg_reject(matcher,event,msg)
 
         if text == "查看投稿列表":
             s["last"] = True
             list_in = easycyber_in_tg(False,False)
+            msg_list = []
             for key in list_in:
-                if list_in[f"{key}"]["public"]:
-                    msg = msg , format(key)
-                else:
-                    return
-        msg = f"{msg}"
-        await send_msg(matcher,event,msg)
+                msg_list.append(format(key))
+            await send_msg(matcher,event,f"{msg_list}")
 
         if text == "拒绝":
             s["last"] = "拒绝"
             msg = "请输入要离开角色昵称"
-        await send_msg_reject(matcher,event,msg)
+            await send_msg_reject(matcher,event,msg)
 
         if s["last"]:
             return
         else:
             msg = f"未知命令“{text}”，已退出"
             await send_msg(matcher,event,msg)
```

### Comparing `nonebot-plugin-hx-yinying-1.0.4/nonebot_plugin_hx_yinying/chat.py` & `nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying/chat.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -- coding: utf-8 --**
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, MessageEvent ,MessageSegment ,Message
 from html import unescape
 from typing import List
 import os,httpx, json, time, requests
 from .config import Config
-from nonebot import get_plugin_config, logger, require
+from nonebot import get_plugin_config, logger, require,get_driver
 hx_config = get_plugin_config(Config)
 from pathlib import Path
 require("nonebot_plugin_localstore")
+import operator
 import nonebot_plugin_localstore as store
 
 
 if hx_config.hx_path == None:
     logger.warning("找不到配置里的路径，将使用默认配置")
     history_dir = store.get_data_dir("Hx_YingYing")
     log_dir = Path(f"{history_dir}\yinying_chat").absolute()
@@ -20,14 +21,15 @@
     logger.success("找到配置里的路径，载入成功")
     history_dir = store.get_data_dir(f"{hx_config.hx_path}")
     log_dir = Path(f"{history_dir}\yinying_chat").absolute()
     log_dir.mkdir(parents=True, exist_ok=True)
 
 #判断模型
 def model_got(msg) -> str:
+    back = "yinyingllm-v2"
     try:
         if msg == "1" or msg == "yinyingllm-v1" or msg == "yinyingllmv1":
             back = "yinyingllm-v1"
         elif msg == "2" or msg == "yinyingllm-v2" or msg == "yinyingllmv2":
             back = "yinyingllm-v2"
         elif msg == "3" or msg == "yinyingllm-v3" or msg == "yinyingllmv3":
             back = "yinyingllm-v3"
@@ -49,33 +51,34 @@
     else:
         history_dir = store.get_data_dir(f"{hx_config.hx_path}")
         log_dir = Path(f"{history_dir}\yinying_chat").absolute()
         log_dir.mkdir(parents=True, exist_ok=True)
         return log_dir
 
 #update-----Hx
-def update_hx() -> str:
+def update_hx():
     fails = 0
     while True:
         try:
             if fails >= 20:
                 break
             headers = {'content-type': 'application/json'}
             ret = requests.get(url="https://pypi.org/pypi/nonebot-plugin-hx-yinying/json", headers=headers ,timeout=10)
             if ret.status_code == 200:
                 json = ret.json()
                 verision = json["info"]["version"]
+                time = json["releases"][f"{verision}"][0]["upload_time"]
             else:
                 continue
         except:
             fails += 1
             logger.warning("网络状况不佳，检查最新版本失败，正在重新尝试")
         else:
             break
-    return verision
+    return verision,time
 
 #获取用户id
 def get_id(event) -> int:
     """获取会话id"""
     if isinstance(event, GroupMessageEvent):
             id = f"{event.user_id}"
     else:
@@ -231,15 +234,15 @@
                     t = int(dt)
                     dw = int(len(json_data) + 1)
                     package_easycyberfurry = json_1
                     package_easycyberfurry["create_time"] = t
                     package_easycyberfurry["last_update"] = t
                     package_easycyberfurry["id"] = dw
                     json_data[f"{cybernick}"] = package_easycyberfurry
-                    with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
+                    with open(f'{log_dir}/config/easycyber.json','w',encoding='utf-8') as file:
                         json.dump(json_data,file)
                     back = json_data
         else:
             create_dir_usr(f"{log_dir}/config")
             with open(f'{log_dir}/config/easycyber.json','w',encoding='utf-8') as file:
                 dt = time.time()
                 t = int(dt)
@@ -260,14 +263,34 @@
                 packages_easycyberfurry["create_time"] = t
                 packages_easycyberfurry["last_update"] = t
                 packages_easycyberfurry["id"] = 1
                 global_easycyberfurry[f"{cybernick}"] = packages_easycyberfurry
                 json.dump(global_easycyberfurry,file)
                 back = global_easycyberfurry
     except Exception as e:
+        if json_1 == False and cybernick == False:
+            dt = time.time()
+            t = int(dt)
+            easycyber_package = {}
+            json_data = {}
+            easycyber_package["cfNickname"] = "Hx"
+            easycyber_package["cfSpecies"] = "狼龙"
+            easycyber_package["cfConAge"] = "child"
+            easycyber_package["cfConStyle"] = "social_anxiety"
+            easycyber_package["cfStory"] = "你的名字叫Hx,相传Hx诞生于幻歆的幻梦破碎之歆中，是终结和新生的象征。"
+            easycyber_package["public"] = True
+            easycyber_package["creator"] = 3485462167
+            easycyber_package["create_time"] = t
+            easycyber_package["last_update"] = t
+            easycyber_package["id"] = 0
+            json_data["Hx"] = easycyber_package
+            with open(f'{log_dir}/config/easycyber.json','w',encoding='utf-8') as file:
+                json.dump(json_data,file)
+            back = json_data
+        else:
             logger.error(f"加载本地cyberfurry预设时失败！，请不要随意修改bot插件本地文件。。。。！")
             logger.warning("你要为你的行为负责，来自不知名开发者")
             logger.warning(f"报错捕获{e}")
             back = False
     return back
 
 #载入本地投稿的easycyber预设(载入失败会被清空
@@ -300,30 +323,50 @@
                 packages_easycyberfurry["create_time"] = t
                 packages_easycyberfurry["last_update"] = t
                 packages_easycyberfurry["id"] = 0
                 global_easycyberfurry[f"{cybernick}"] = packages_easycyberfurry
                 json.dump(global_easycyberfurry,file)
                 back = global_easycyberfurry
     except Exception as e:
-            logger.error(f"加载本地投稿easycyberfurry时失败！，请不要随意修改bot插件本地文件。。。。！")
-            logger.warning("你要为你的行为负责，来自不知名开发者")
-            logger.warning(f"报错捕获{e}")
-            create_dir_usr(f"{log_dir}/file")
-            with open(f'{log_dir}/file/easycyber_tg.json','w',encoding='utf-8') as file:
+            if json_1 == False and cybernick == False:
                 dt = time.time()
                 t = int(dt)
+                easycyber_package = {}
                 global_easycyberfurry = {}
-                packages_easycyberfurry = json_1
-                packages_easycyberfurry["create_time"] = t
-                packages_easycyberfurry["last_update"] = t
-                packages_easycyberfurry["id"] = 0
-                global_easycyberfurry[f"{cybernick}"] = packages_easycyberfurry
-                json.dump(global_easycyberfurry,file)
+                easycyber_package["cfNickname"] = "保留查询"
+                easycyber_package["cfSpecies"] = "狼龙"
+                easycyber_package["cfConAge"] = "child"
+                easycyber_package["cfConStyle"] = "social_anxiety"
+                easycyber_package["cfStory"] = "你的名字叫Hx,相传Hx诞生于幻歆的幻梦破碎之歆中，是终结和新生的象征。"
+                easycyber_package["public"] = True
+                easycyber_package["creator"] = 3485462167
+                easycyber_package["create_time"] = t
+                easycyber_package["last_update"] = t
+                easycyber_package["id"] = 0
+                global_easycyberfurry["保留查询"] = easycyber_package
+                with open(f'{log_dir}/file/easycyber_tg.json','w',encoding='utf-8') as file:
+                    json.dump(global_easycyberfurry,file)
                 back = global_easycyberfurry
-            back = False
+            else:
+                logger.error(f"加载本地投稿easycyberfurry时失败！，请不要随意修改bot插件本地文件。。。。！")
+                logger.warning("你要为你的行为负责，来自不知名开发者")
+                logger.warning(f"报错捕获{e}")
+                create_dir_usr(f"{log_dir}/file")
+                with open(f'{log_dir}/file/easycyber_tg.json','w',encoding='utf-8') as file:
+                    dt = time.time()
+                    t = int(dt)
+                    global_easycyberfurry = {}
+                    packages_easycyberfurry = json_1
+                    packages_easycyberfurry["create_time"] = t
+                    packages_easycyberfurry["last_update"] = t
+                    packages_easycyberfurry["id"] = 0
+                    global_easycyberfurry[f"{cybernick}"] = packages_easycyberfurry
+                    json.dump(global_easycyberfurry,file)
+                    back = global_easycyberfurry
+                back = False
     return back
 
 #载入全局本地配置
 def config_in_global() -> str:
     try:
         if os.path.exists(f"{log_dir}/config/config_global.json"):
             with open(f'{log_dir}/config/config_global.json','r',encoding='utf-8') as file:
@@ -493,20 +536,41 @@
 
 #载入个人本地配置
 def config_in_user(id,nick) -> str:
     try:
         if os.path.exists(f"{log_dir}/config/config_user.json"):
             with open(f'{log_dir}/config/config_user.json','r',encoding='utf-8') as file:
                 json_data = json.load(file)
-                if id in json_data or not nick:
+                if id in json_data and nick:
+                    back = json_data
+                elif id in json_data and not nick:
                     back = json_data
+                elif id not in json_data and not nick:
+                    dt = time.time()
+                    t = int(dt)
+                    id_package = {}
+                    id_package['nick'] = False
+                    id_package['character'] = f"我是一只可爱的毛毛龙嗷呜"
+                    id_package['character_in'] = True
+                    id_package['easycharacter_in'] = True
+                    id_package['private_model'] = "yinyingllm-v2"
+                    id_package['chat_alltimes'] = 0
+                    id_package['times'] = 1
+                    id_package['time'] = 1713710000
+                    id_package['first_chattime'] = t
+                    id_package['last_chattime'] = t
+                    json_data[f"{id}"] = id_package
+                    with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
+                        json.dump(json_data,file)
+                        back = json_data
                 else:
                     dt = time.time()
                     t = int(dt)
                     id_package = {}
+                    id_package['nick'] = f"{nick}"
                     id_package['character'] = f"我是{nick}，是一只可爱的毛毛龙嗷呜"
                     id_package['character_in'] = True
                     id_package['easycharacter_in'] = True
                     id_package['private_model'] = "yinyingllm-v2"
                     id_package['chat_alltimes'] = 0
                     id_package['times'] = 1
                     id_package['time'] = 1713710000
@@ -519,14 +583,15 @@
         else:
             create_dir_usr(f"{log_dir}/config")
             with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
                 dt = time.time()
                 t = int(dt)
                 json_data = {}
                 id_package = {}
+                id_package['nick'] = nick
                 id_package['character'] = f"我是{nick}，是一只可爱的毛毛龙嗷呜"
                 id_package['character_in'] = True
                 id_package['easycharacter_in'] = True
                 id_package['private_model'] = "yinyingllm-v2"
                 id_package['chat_alltimes'] = 0
                 id_package['times'] = 1
                 id_package['time'] = 1713710000
@@ -540,43 +605,75 @@
             logger.warning("你要为你的行为负责，来自不知名开发者")
             logger.warning(f"报错捕获{e}")
             with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
                 dt = time.time()
                 t = int(dt)
                 json_data = {}
                 id_package = {}
+                id_package['nick'] = False
                 id_package['character'] = f"我是{nick}，是一只可爱的毛毛龙嗷呜"
                 id_package['character_in'] = True
                 id_package['private_model'] = "yinyingllm-v2"
                 id_package['chat_alltimes'] = 0
                 id_package['times'] = 1
                 id_package['time'] = 1713710000
                 id_package['first_chattime'] = t
                 id_package['last_chattime'] = t
                 json_data[f"{id}"] = id_package
                 json.dump(json_data,file)
                 back = json_data
     return back
 
+#获取配置内键值并列表化
+def config_list(config):
+    try:
+        tf_key = []
+        w_key = []
+        list_key = []
+        app_key = []
+        if config:
+            for key in config:
+                get_config = json_get(config,format(key))
+                if get_config == True or get_config == False:
+                    tf_key.append(format(key))
+                elif operator.contains(f"{get_config}","{") and operator.contains(f"{get_config}","}"):
+                    app_key.append(format(key))
+                elif operator.contains(f"{get_config}","[") and operator.contains(f"{get_config}","]"):
+                    list_key.append(format(key))
+                elif get_config == "null":
+                    w_key.append(format(key))
+                else:
+                    w_key.append(format(key))
+        else:
+            logger.error(f"配置文件不存在！")
+    except Exception as e:
+        logger.warning(f"报错捕获{e}")
+        logger.error(f"报错定位于获取配置内鉴值")
+    return tf_key, w_key, list_key ,app_key
+
 #全局权限检查！！！！！（总算写出来了）
 def place(id) -> int:
     try:
         config = config_in_global()
         admin_pro = json_get(config,"admin_pro")
         admin_user = json_get(config,"admin_user")
         black_list = json_get(config,"blacklist_user")
-        if f"{id}" in hx_config.SUPERUSERS:
+        superuser = get_driver().config.superusers
+        logger.warning(f"user捕获{superuser}")
+        if superuser:
+            if id in superuser:
+                place_user = 10
+        elif id == admin_pro:
             place_user = 10
-        elif f"{id}" == f"{admin_pro}":
-            place_user = 10
-        elif f"{id}" in f"{admin_user}":
+        elif id in admin_user:
             place_user = 9
-        elif f"{id}" in f"{black_list}":
+        elif id in black_list:
             place_user = 1
         else:
+            logger.warning(f"没有找到超级管理员！")
             place_user = 5
     except Exception as e:
             logger.warning(f"报错捕获{e}")
             place_user = 5
     return place_user
 
 #尝试获取bot本地文件夹文件
@@ -671,15 +768,15 @@
                 nickname="AAA星佑批发（Hx限定）",
                 content=Message(f"投稿发送到控制台[admin_group_switch]:{admin_group_switch}"),                    
                 ))
         msg_list.append(
                 MessageSegment.node_custom(
                 user_id=3202123263,
                 nickname="AAA星佑批发（Hx限定）",
-                content=Message(f"投稿发送到超级管理员[admin_group_switch]:{admin_group_switch}"),                    
+                content=Message(f"投稿发送到超级管理员[admin_user_switch]:{admin_user_switch}"),                    
                 ))
         msg_list.append(
                 MessageSegment.node_custom(
                 user_id=3202123263,
                 nickname="AAA星佑批发（Hx限定）",
                 content=Message(f"bot管理员列表[admin_user]:{admin_user}"),                    
                 ))
@@ -785,15 +882,15 @@
         back = False
     return back
 
 def json_get_text(json,key) -> str:
     try:
         back = json[f"{key}"]
     except Exception as e:
-        back = None
+        back = 0
     return back
 
 #手动刷新对话
 def clear_id(id,nick) -> str:
     data = log_in()
     dt = time.time()
     t = int(dt)
@@ -808,57 +905,64 @@
                 json.dump(config,user)
                 zt = True
     except Exception as e:
             zt = False
     return zt
 
 #初始化传参（整理data）
-def data_in(groupid,id,text,nick) -> str:
+def data_in(groupid,id,text,nick0) -> str:
     """构建data"""
     data = {}
     packages_data = json.loads(json.dumps(data))
     allvariables = {}
     packages_data['appId'] = f'{hx_config.yinying_appid}'
-    user_config = config_in_user(id,nick)
+    user_config = config_in_user(id,nick0)
     id_config = json_get(user_config,id)
     character = json_get(id_config,"character")
     time = json_get(id_config,"time")
+    nick = json_get(id_config,"nick")
+    if not nick:
+        nick == nick0
     try:
         if groupid == None:
             model = json_get(id_config,"private_model")
+            packages_data['model'] = f'{model}'
             if model == None or model == "yinyingllm-v2":
                 logger.warning("找不到配置里的yinying_model或你设置的模型为yinyingllm-v2,将使用默认模型llm2")
                 packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-yinyingllm-v2'
                 packages_data['model'] = 'yinyingllm-v2'
                 package = {}
                 package['nickName'] = f'{nick}'
                 package['furryCharacter'] = f'{character}'
                 allvariables.update(package)
                 packages_data['variables'] = allvariables
                 packages_data['message'] = f'{text}'
             elif model == "yinyingllm-v1":
                 packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-yinyingllm-v1'
+                package = {}
+                package['nickName'] = f'{nick}'
+                package['furryCharacter'] = f'{character}'
+                allvariables.update(package)
+                packages_data['variables'] = allvariables
                 packages_data['message'] = f'{text}'
             elif model == "yinyingllm-v3":
                 packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-yinyingllm-v3'
                 package = {}
                 package['nickName'] = f'{nick}'
                 package['furryCharacter'] = f'{character}'
                 allvariables.update(package)
                 packages_data['variables'] = allvariables
                 packages_data['message'] = f'{text}'
             elif model == "cyberfurry-001":
                 packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-cyberfurry-001'
-                packages_data['model'] = 'cyberfurry-001'
                 packages_data['systemPrompt'] = "你的名字叫Hx"
                 packages_data['message'] = f'{text}'
             elif model == "easycyberfurry-001":
                 if json_get(id_config,"easycharacter_in") == True or not json_get(id_config,"easycharacter_in"):
                     packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-easycyberfurry-001'
-                    packages_data['model'] = 'easycyberfurry-001'
                     characterSet = {}
                     package = {}
                     package['nickName'] = f'{nick}'
                     package['furryCharacter'] = f'{character}'
                     allvariables.update(package)
                     new_package = {}
                     new_package['cfNickname'] = 'Hx'
@@ -871,15 +975,14 @@
                     packages_data['characterSet'] = characterSet
                     packages_data['message'] = f'{text}'
                 else:
                     promte_model = json_get(id_config,"easycharacter_in")
                     promte = json_get(easycyber_in(promte_model,False),promte_model)
                     if not promte:
                         packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-easycyberfurry-001'
-                        packages_data['model'] = 'easycyberfurry-001'
                         characterSet = {}
                         package = {}
                         package['nickName'] = f'{nick}'
                         package['furryCharacter'] = f'{character}'
                         allvariables.update(package)
                         new_package = {}
                         new_package['cfNickname'] = 'Hx'
@@ -889,15 +992,14 @@
                         new_package['cfStory'] = '你的名字叫Hx,相传Hx诞生于幻歆的幻梦破碎之歆中，是终结和新生的象征。'
                         characterSet.update(new_package)
                         packages_data['variables'] = allvariables
                         packages_data['characterSet'] = characterSet
                         packages_data['message'] = f'{text}'
                     else:
                         packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-easycyberfurry-001'
-                        packages_data['model'] = 'easycyberfurry-001'
                         package = {}
                         package['nickName'] = f'{nick}'
                         package['furryCharacter'] = f'{character}'
                         allvariables.update(package)
                         characterSet = {}
                         new_package = {}
                         new_package['cfNickname'] = f"{promte['cfNickname']}"
@@ -917,46 +1019,47 @@
                 package['furryCharacter'] = f'{character}'
                 allvariables.update(package)
                 packages_data['variables'] = allvariables
                 packages_data['message'] = f'{text}'
         else:
             group_config = config_in_group(groupid)
             group_config = json_get(group_config,groupid)
-            model_group = json_get(group_config,"use_model")
-            model = model_group
+            model = json_get(group_config,"use_model")
+            packages_data['model'] = f'{model}'
             if model == None or model == "yinyingllm-v2":
                 logger.warning("找不到配置里的yinying_model或你设置的模型为yinyingllm-v2,将使用默认模型llm2")
                 packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-yinyingllm-v2'
-                packages_data['model'] = 'yinyingllm-v2'
                 package = {}
                 package['nickName'] = f'{nick}'
                 package['furryCharacter'] = f'{character}'
                 allvariables.update(package)
                 packages_data['variables'] = allvariables
                 packages_data['message'] = f'{text}'
             elif model == "yinyingllm-v1":
                 packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-yinyingllm-v1'
+                package = {}
+                package['nickName'] = f'{nick}'
+                package['furryCharacter'] = f'{character}'
+                allvariables.update(package)
                 packages_data['message'] = f'{text}'
             elif model == "yinyingllm-v3":
                 packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-yinyingllm-v3'
                 package = {}
                 package['nickName'] = f'{nick}'
                 package['furryCharacter'] = f'{character}'
                 allvariables.update(package)
                 packages_data['variables'] = allvariables
                 packages_data['message'] = f'{text}'
             elif model == "cyberfurry-001":
                 packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-cyberfurry-001'
-                packages_data['model'] = 'cyberfurry-001'
                 packages_data['systemPrompt'] = "你的名字叫Hx"
                 packages_data['message'] = f'{text}'
             elif model == "easycyberfurry-001":
                 if json_get(id_config,"easycharacter_in") == True or not json_get(group_config,"easycharacter_in"):
                     packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-easycyberfurry-001'
-                    packages_data['model'] = 'easycyberfurry-001'
                     characterSet = {}
                     package = {}
                     package['nickName'] = f'{nick}'
                     package['furryCharacter'] = f'{character}'
                     allvariables.update(package)
                     new_package = {}
                     new_package['cfNickname'] = 'Hx'
@@ -969,15 +1072,14 @@
                     packages_data['characterSet'] = characterSet
                     packages_data['message'] = f'{text}'
                 else:
                     promte_model = json_get(group_config,"easycharacter_in")
                     promte = json_get(easycyber_in(promte_model,False),promte_model)
                     if not promte:
                         packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-easycyberfurry-001'
-                        packages_data['model'] = 'easycyberfurry-001'
                         characterSet = {}
                         package = {}
                         package['nickName'] = f'{nick}'
                         package['furryCharacter'] = f'{character}'
                         allvariables.update(package)
                         new_package = {}
                         new_package['cfNickname'] = 'Hx'
@@ -987,15 +1089,14 @@
                         new_package['cfStory'] = '你的名字叫Hx,相传Hx诞生于幻歆的幻梦破碎之歆中，是终结和新生的象征。'
                         characterSet.update(new_package)
                         packages_data['variables'] = allvariables
                         packages_data['characterSet'] = characterSet
                         packages_data['message'] = f'{text}'
                     else:
                         packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-easycyberfurry-001'
-                        packages_data['model'] = 'easycyberfurry-001'
                         package = {}
                         package['nickName'] = f'{nick}'
                         package['furryCharacter'] = f'{character}'
                         allvariables.update(package)
                         characterSet = {}
                         new_package = {}
                         new_package['cfNickname'] = f"{promte['cfNickname']}"
@@ -1059,17 +1160,20 @@
     except Exception as e:
         back_msg = f"{back}\n\n{osu}\n\n未知错误，错误定位于#主要构建函数。"
     return back_msg
 
 #获取回复（被艾特）
 async def get_answer_at(matcher, event, bot):
     text = unescape(await gen_chat_text(event, bot))
-    if  text == "" or text is None or text == "！d" or text == "/！d":
-        msg = "诶唔，你叫我是有什么事嘛？"
-        await send_msg(matcher,event,msg)
+    if  text == "" or text == None or text == "！d" or text == "/！d":
+        if text == "！d" or text == "/！d":
+            return
+        else:
+            msg = "诶唔，你叫我是有什么事嘛？"
+            await send_msg(matcher,event,msg)
     else:
         try:
             groupid = get_groupid(event)
             id = get_id(event)
             nick = await get_nick(bot,event)
             user_in(id,json_replace(text))
             back_msg = str(await yinying(groupid,id,text,nick))
```

### Comparing `nonebot-plugin-hx-yinying-1.0.4/nonebot_plugin_hx_yinying.egg-info/PKG-INFO` & `nonebot-plugin-hx-yinying-1.0.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: nonebot-plugin-hx-yinying
-Version: 1.0.4
-Summary: chat with yinying
-Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
-Author: Huan Xin
-Author-email: mc.xiaolang@foxmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <!--
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
  * @Author         : huanxin996
  * @Date           : 2024-4-17
@@ -93,56 +80,32 @@
 ### yinying_token
 
 - 类型：`str`
 - 默认值：`None`
 - 说明：这里写你找秩乱获取到的api_key
 - 重要：必填
 
-
-### hx_api_yinying(已于0.0.7版本移除)
-
+### hx_path
 - 类型：`str`
 - 默认值：`None`
-- 说明：yinying的api地址
-- 重要：必填
-
-### yinying_model(已于0.0.7版本移除)
+- 说明：这里是插件本地配置的存储目录
+- 重要：非必填
 
-- 类型：`str`
+### SUPERUSERS
+- 类型：`list`
 - 默认值：`None`
-- 说明：选择使用银影的模型
-- 注意 该配置项即将移除（转为插件内配置！）
-
-## hx_path
-- 类型：`str`
-- 默认值：`None`
-- 说明：银影对话的用户数据存储路径(不写将使用默认配置)
-
-## hx_reply(已于0.0.7版本移除)
-- 类型：`bool`
-- 默认值：`False`
-- 说明：bot发送chat消息时是否回复
-- 注意：该项启用时hx_reply_at将被忽略
-
-## hx_reply_at(已于0.0.7版本移除)
-- 类型：`bool`
-- 默认值：`False`
-- 说明：bot发送chat消息时不回复时是否艾特
-
-## yinying_limit(已于0.0.7版本移除)
-- 类型：`int`
-- 默认值：`12`
-- 说明：对于银影对话限制的次数
-
+- 说明：这里是超级管理员（插件）
+- 重要：必填（你需要这个来管理该插件）
 
 配置文件示例（默认模板）
 
 ```dotenv
 yinying_appid=你的appid
 yinying_token=你的token(不带bearer)
+hx_path=C:\Users\user\Desktop
 ```
 
 
 ## Contributors ✨
 
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
```

#### html2text {}

```diff
@@ -1,17 +1,11 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.0.4 Summary:
-chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
-yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Description-Content-
-Type: text/markdown License-File: LICENSE [![All Contributors](https://
-img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
-(#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
-huanxin996 * @LastEditTime : 2024-4-22 * @Description : None * @GitHub : https:
-//github.com/huanxin996 -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-2-
+orange.svg?style=flat-square)](#contributors-) * @Author : huanxin996 * @Date :
+2024-4-17 * @LastEditors : huanxin996 * @LastEditTime : 2024-4-22 *
+@Description : None * @GitHub : https://github.com/huanxin996 -->
                                    _[_n_o_n_e_b_o_t_]
                 # nonebot_plugin_hx-yinying _â¨ Hx vs YinYing
                   (å¨çº¿ä¸é¶å½±è¿è¡å¯¹è¯çæä»¶) â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## å®è£ pipå®è£ ```dotenv pip install nonebot-plugin-hx-yinying ``` nb
 pluginå®è£ ```dotenv nb plugin install nonebot-plugin-hx-yinying ``` ##
 ä½¿ç¨æ¹å¼ éç¨: - @Bot æèåå¤å³å¯ OneBot: - @Bot - åå¤Bot ##
@@ -22,24 +16,16 @@
 [å®ç½é¾æ¥](https://chat.wingmark.cn/) . > [!WARNING] >
 è¯·æ³¨æï¼è¯¥é¡¹ç®æ¯æ¥å¥äºä¹±ä¹±çé¡¹ç®ï¼ä½ éè¦éµå®apiä½¿ç¨ç
 [è§è](https://wingmark.feishu.cn/docx/NFgJddgQAotygKxXiu6cpyg5nqr)ã
 éç½®æ¹å¼ï¼ç´æ¥å¨ NoneBot
 å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã ### yinying_appid -
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼ä½ çappid - éè¦ï¼å¿å¡«
 ### yinying_token - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
-è¯´æï¼è¿éåä½ æ¾ç§©ä¹±è·åå°çapi_key - éè¦ï¼å¿å¡« ###
-hx_api_yinying(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
-è¯´æï¼yinyingçapiå°å - éè¦ï¼å¿å¡« ### yinying_model
-(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
-è¯´æï¼éæ©ä½¿ç¨é¶å½±çæ¨¡å - æ³¨æ
-è¯¥éç½®é¡¹å³å°ç§»é¤ï¼è½¬ä¸ºæä»¶åéç½®ï¼ï¼ ## hx_path -
-ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
-è¯´æï¼é¶å½±å¯¹è¯çç¨æ·æ°æ®å­å¨è·¯å¾(ä¸åå°ä½¿ç¨é»è®¤éç½®)
-## hx_reply(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
-è¯´æï¼botåéchatæ¶æ¯æ¶æ¯å¦åå¤ -
-æ³¨æï¼è¯¥é¡¹å¯ç¨æ¶hx_reply_atå°è¢«å¿½ç¥ ## hx_reply_at
-(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
-è¯´æï¼botåéchatæ¶æ¯æ¶ä¸åå¤æ¶æ¯å¦è¾ç¹ ## yinying_limit
-(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`int` - é»è®¤å¼ï¼`12` -
-è¯´æï¼å¯¹äºé¶å½±å¯¹è¯éå¶çæ¬¡æ° éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼
-```dotenv yinying_appid=ä½ çappid yinying_token=ä½ çtoken(ä¸å¸¦bearer) ```
-## Contributors â¨
+è¯´æï¼è¿éåä½ æ¾ç§©ä¹±è·åå°çapi_key - éè¦ï¼å¿å¡« ### hx_path
+- ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
+è¯´æï¼è¿éæ¯æä»¶æ¬å°éç½®çå­å¨ç®å½ - éè¦ï¼éå¿å¡« ###
+SUPERUSERS - ç±»åï¼`list` - é»è®¤å¼ï¼`None` -
+è¯´æï¼è¿éæ¯è¶çº§ç®¡çåï¼æä»¶ï¼ -
+éè¦ï¼å¿å¡«ï¼ä½ éè¦è¿ä¸ªæ¥ç®¡çè¯¥æä»¶ï¼
+éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼ ```dotenv yinying_appid=ä½ çappid
+yinying_token=ä½ çtoken(ä¸å¸¦bearer) hx_path=C:\Users\user\Desktop ``` ##
+Contributors â¨
```

### Comparing `nonebot-plugin-hx-yinying-1.0.4/setup.py` & `nonebot-plugin-hx-yinying-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-hx-yinying",
-    version="1.0.4",
+    version="1.0.5",
     author="Huan Xin",
     author_email="mc.xiaolang@foxmail.com",
     description="chat with yinying",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     packages=setuptools.find_packages(),
```

