# Comparing `tmp/nonebot_plugin_cyberfurry-1.3.tar.gz` & `tmp/nonebot_plugin_cyberfurry-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_cyberfurry-1.3.tar", last modified: Tue Apr 23 14:23:46 2024, max compression
+gzip compressed data, was "nonebot_plugin_cyberfurry-1.4.tar", last modified: Wed Apr 24 16:08:43 2024, max compression
```

## Comparing `nonebot_plugin_cyberfurry-1.3.tar` & `nonebot_plugin_cyberfurry-1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:23:46.214848 nonebot_plugin_cyberfurry-1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-23 14:23:39.000000 nonebot_plugin_cyberfurry-1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44010 2024-04-23 14:23:46.214848 nonebot_plugin_cyberfurry-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-23 14:23:39.000000 nonebot_plugin_cyberfurry-1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:23:46.210848 nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-23 14:23:39.000000 nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-23 14:23:39.000000 nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry/callapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-23 14:23:39.000000 nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-23 14:23:39.000000 nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry/cyberfurry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-23 14:23:39.000000 nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry/cyberfurrymodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-23 14:23:39.000000 nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry/cyberhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-23 14:23:39.000000 nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry/cyberinit.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-23 14:23:39.000000 nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-23 14:23:39.000000 nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry/jsondata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-23 14:23:39.000000 nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry/plugins_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:23:46.214848 nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44010 2024-04-23 14:23:46.000000 nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-23 14:23:46.000000 nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:23:46.000000 nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-23 14:23:46.000000 nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-23 14:23:46.000000 nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-23 14:23:39.000000 nonebot_plugin_cyberfurry-1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:23:46.214848 nonebot_plugin_cyberfurry-1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:08:43.054686 nonebot_plugin_cyberfurry-1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44121 2024-04-24 16:08:43.054686 nonebot_plugin_cyberfurry-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:08:43.050686 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/callapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/cyberfurry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/cyberfurrymodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/cyberhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/cyberinit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/jsondata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/plugins_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:08:43.054686 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44121 2024-04-24 16:08:43.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-24 16:08:43.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:08:43.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-24 16:08:43.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 16:08:43.000000 nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-24 16:08:36.000000 nonebot_plugin_cyberfurry-1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 16:08:43.054686 nonebot_plugin_cyberfurry-1.4/setup.cfg
```

### Comparing `nonebot_plugin_cyberfurry-1.3/LICENSE` & `nonebot_plugin_cyberfurry-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.3/PKG-INFO` & `nonebot_plugin_cyberfurry-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cyberfurry
-Version: 1.3
+Version: 1.4
 Summary: nonebot插件 cyberfurry-与赛博狼狼对话吧~
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -712,20 +712,21 @@
 </a>
 <img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">
 
 </div>
 
 ## 📖 介绍
 
-官方网站 : https://chat.wingmark.cn
+官方网站 : [CyberFurry](https://chat.wingmark.cn/)
+
 API申请请通过官方群聊找 群主 申请
 
 ### ⚠ 重要
 
-请务必遵守用户协议 https://tailnet.cn/?page=yinyingzc
+请务必遵守 [用户协议](https://tailnet.cn/?page=yinyingzc)
 
 
 easycf模型还未填坑,后续更新适配
 
 ## 💿 安装
 
 <details open>
@@ -767,21 +768,25 @@
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
-若未配置必填项此插件将不会工作!!!!
+
+> [!WARNING]
+> 若未配置必填项此插件将不会工作!!!!
+
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | cf_appid | 是 | 无 | API的appid |
 | cf_token | 是 | 无 | API的token |
 | cubplugin_datadir | 否 | "" | 插件数据文件夹 |
+| cf_enableistome | 否 | False | 在消息是对bot时是否启用chat |
 
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | /chat /cf /yy | 群员 | 否 | 任意 | 触发对话 |
```

### Comparing `nonebot_plugin_cyberfurry-1.3/README.md` & `nonebot_plugin_cyberfurry-1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -19,20 +19,21 @@
 </a>
 <img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">
 
 </div>
 
 ## 📖 介绍
 
-官方网站 : https://chat.wingmark.cn
+官方网站 : [CyberFurry](https://chat.wingmark.cn/)
+
 API申请请通过官方群聊找 群主 申请
 
 ### ⚠ 重要
 
-请务必遵守用户协议 https://tailnet.cn/?page=yinyingzc
+请务必遵守 [用户协议](https://tailnet.cn/?page=yinyingzc)
 
 
 easycf模型还未填坑,后续更新适配
 
 ## 💿 安装
 
 <details open>
@@ -74,21 +75,25 @@
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
-若未配置必填项此插件将不会工作!!!!
+
+> [!WARNING]
+> 若未配置必填项此插件将不会工作!!!!
+
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | cf_appid | 是 | 无 | API的appid |
 | cf_token | 是 | 无 | API的token |
 | cubplugin_datadir | 否 | "" | 插件数据文件夹 |
+| cf_enableistome | 否 | False | 在消息是对bot时是否启用chat |
 
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | /chat /cf /yy | 群员 | 否 | 任意 | 触发对话 |
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
            # nonebot-plugin-cyberfurry _â¨ nonebotæä»¶ cyberfurry
              ä¸èµåç¼ç¼å¯¹è¯å§~ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
-## ð ä»ç» å®æ¹ç½ç« : https://chat.wingmark.cn
-APIç³è¯·è¯·éè¿å®æ¹ç¾¤èæ¾ ç¾¤ä¸» ç³è¯· ### â  éè¦
-è¯·å¡å¿éµå®ç¨æ·åè®® https://tailnet.cn/?page=yinyingzc
+## ð ä»ç» å®æ¹ç½ç« : [CyberFurry](https://chat.wingmark.cn/
+) APIç³è¯·è¯·éè¿å®æ¹ç¾¤èæ¾ ç¾¤ä¸» ç³è¯· ### â  éè¦
+è¯·å¡å¿éµå® [ç¨æ·åè®®](https://tailnet.cn/?page=yinyingzc)
 easycfæ¨¡åè¿æªå¡«å,åç»­æ´æ°éé ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£
 å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-cyberfurry
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-cyberfurry pdm pdm add nonebot-plugin-cyberfurry
 poetry poetry add nonebot-plugin-cyberfurry conda conda install nonebot-plugin-
 cyberfurry æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_cyberfurry"] ##
 âï¸ éç½® å¨ nonebot2
-é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½®
+é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® > [!WARNING] >
 è¥æªéç½®å¿å¡«é¡¹æ­¤æä»¶å°ä¸ä¼å·¥ä½!!!! | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | cf_appid | æ¯ | æ  |
 APIçappid | | cf_token | æ¯ | æ  | APIçtoken | | cubplugin_datadir | å¦
-| "" | æä»¶æ°æ®æä»¶å¤¹ | ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé |
-éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | /chat /cf /
-yy | ç¾¤å | å¦ | ä»»æ | è§¦åå¯¹è¯ | | cfå·æ°å¯¹è¯ | ç¾¤å | å¦ |
-ä»»æ | å·æ°å¯¹è¯ | | cfè®¾å®æ¨¡å | ç¾¤å | å¦ | ä»»æ |
+| "" | æä»¶æ°æ®æä»¶å¤¹ | | cf_enableistome | å¦ | False |
+å¨æ¶æ¯æ¯å¯¹botæ¶æ¯å¦å¯ç¨chat | ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ |
+æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | /
+chat /cf /yy | ç¾¤å | å¦ | ä»»æ | è§¦åå¯¹è¯ | | cfå·æ°å¯¹è¯ | ç¾¤å
+| å¦ | ä»»æ | å·æ°å¯¹è¯ | | cfè®¾å®æ¨¡å | ç¾¤å | å¦ | ä»»æ |
 è®¾å®ä½¿ç¨çyinyingæ¨¡å,æ³¨æ,æ­¤ä¸ºä¸ªäººéç½® | | cfå½åæ¨¡å |
 ç¾¤å | å¦ | ä»»æ | æ¥çå½åæ¨¡å | | cfè®¾å® furåå­ furç§æ |
 ç¾¤å | å¦ | ä»»æ | è®¾å®ä¼ å¥yinyingçèªèº«è®¾å® |
```

### Comparing `nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry/__init__.py` & `nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry/callapi.py` & `nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/callapi.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry/cyberfurry.py` & `nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/cyberfurry.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 from loguru import logger
 
 from .callapi import api
 from .cyberfurrymodel import (
     cyberfurry_001,
     easycyberfurry_001,
     yinyingllm_v123,
-    config
+    config,
+    loadmodel
 )
 cftype = cyberfurry_001 | easycyberfurry_001 | yinyingllm_v123
 
 apiurl = "https://api-yinying-ng.wingmark.cn/v1/chatWithCyberFurry"
 
 
 
@@ -30,24 +31,26 @@
 
 
 class cyberfurry:
     headers = {
         'Content-type': 'application/json',
         'Authorization': f'Bearer {config.cf_token}'
     }
-    model = {
+    basemodel = {
         #多模型示例
         "cyberfurry": cyberfurry_001(),
-        #"cyberfurry-性格2": cyberfurry_001(),
-        #"cyberfurry-beta": cyberfurry_001(),
         "easycyberfurry": easycyberfurry_001(),
         "yinyingllm-v1": yinyingllm_v123(),
         "yinyingllm-v2": yinyingllm_v123(),
         "yinyingllm-v3": yinyingllm_v123()
     }
+    model ={
+        **basemodel,
+        **loadmodel()
+        }
     localdata=loaddata()
     maxtimes = 16
     userchat = localdata.get('userchat',{})
     usertimes = localdata.get('usertimes',{})
     
     localdata={}
```

### Comparing `nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry/cyberhistory.py` & `nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/cyberhistory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from nonebot.adapters.onebot.v11 import (
-   Bot,MessageEvent
+   Bot,MessageEvent 
 )
 from nonebot.adapters.onebot.v11 import GroupMessageEvent as onebotV11GroupMessageEvent
 from nonebot.params import CommandArg
 from nonebot import on_command
 from nonebot.matcher import Matcher
 from .cyberfurry import *
 from .jsondata import gethistorylist,gethistorytxt
```

### Comparing `nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry/cyberinit.py` & `nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/cyberinit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 
 from nonebot.adapters.onebot.v11 import (
-   Bot ,MessageSegment
+   Bot ,MessageSegment , PrivateMessageEvent
 )
 from nonebot.matcher import Matcher
 from .cyberfurry import *
 
 from nonebot.adapters.onebot.v11 import MessageEvent as obV11event
 from nonebot.params import CommandArg
-from nonebot import on_command
+from nonebot import on_command , on_message
+from nonebot.rule import to_me ,Rule
+from .config import config
 try:
     from nonebot.adapters.telegram.event import MessageEvent as TGevent
 except:
     TGevent = obV11event
 
-MessageEvent = TGevent | obV11event
+MessageEvent = obV11event | TGevent
+
+async def is_enable():
+    return config.cf_enableistome
+
+autorun = on_message(
+    rule=to_me() & Rule(is_enable),
+    priority=900
+)
 
 run = on_command(
     "/chat",
     aliases={"/yy","/cf"} ,
+    block=True,
     priority=25
 )
 init = on_command(
     "cf刷新对话",
     aliases={ "cf初始化"} ,
     priority=25
 )
@@ -64,24 +75,25 @@
 def checkethnic(ethnic):
     liste = list(bashethnic)
     if ethnic in liste:
         return True ,""
     msg ="\n种族只支持:\n[" +"|".join(liste) + "]"
     return False ,msg
 
+    
 @run.handle()
 async def cyberfurryrun(
     bot:Bot,
     event:MessageEvent,
     matcher:Matcher,
     data: list = CommandArg(),  
 ):
     if len(data)==0:
         return 0
-    msg = data[0]
+    msg = str(data[0])
     user_id = str(event.user_id)
     matchObj ,_= checkmsg(msg)
     if not matchObj:
         await matcher.send("[幼龙云V5]:参数体不当...停止响应")
         return 0
     userinfo = await bot.get_stranger_info(user_id=user_id)
     name = userinfo.get("nickname","未知")
@@ -91,22 +103,36 @@
     retmsg , times = await cf.chat(user_id,name,msg)
     maxtimes = cf.maxtimes
     await matcher.send(
         MessageSegment.reply(event.message_id) +
         retmsg +
         (f"\n({times}/{maxtimes},将开启新对话)" if times >=maxtimes else f"\n({times}/{maxtimes}轮对话)")
     )
+    
+@autorun.handle()
+async def cyberfurryautorun(
+    bot:Bot,
+    event:MessageEvent,
+    matcher:Matcher,
+):
+    await cyberfurryrun(
+        bot=bot,
+        event=event,
+        matcher=matcher,
+        data=[event.get_message()]
+    )
+
 @setuser.handle()
 async def cyberfurrysetuser(
     event:MessageEvent,matcher:Matcher ,args: list = CommandArg()
 ):
     user_id = str(event.user_id)
     if len(args) <1:
         return 0
-    data = args[0].split(" ")
+    data = str(args[0]).split(" ")
     if (len(data)>=2):
         name = data[0]
         ethnic = data[1]
         msg = "[幼龙云V5]:出现问题"
         key1 ,msg1=checkmsg(name)
         key2 ,msg2= checkethnic(ethnic)
         msg+=msg1+msg2
@@ -140,15 +166,15 @@
     await matcher.send(msg)
 
 @set.handle()
 async def cyberfurryset(
     event:MessageEvent,matcher:Matcher,
     data: list = CommandArg()
 ):
-    modelname = data[0]
+    modelname = str(data[0])
     user_id = str(event.user_id)
     msg="[幼龙云V5]"
     if cf.model.get(modelname,None) != None:
         try:
             defqqmodel(user_id,modelname)
         except:
             defqqname(user_id,{
```

### Comparing `nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry/data_source.py` & `nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry/jsondata.py` & `nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/jsondata.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry/plugins_data.py` & `nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry/plugins_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,21 +13,20 @@
     data_dir = store.get_data_dir("cubplugins")
 
     logger.warning("未配置自定义数据文件夹,将使用localstore路径->"+str(data_dir))
 else:
     path_name=config.cubplugin_datadir
     data_dir = Path(Path(path_name)).absolute()
     logger.debug("已配置自定义数据文件夹!->"+str(data_dir))
-
     if data_dir.is_dir():
-        logger.opt(colors=True).debug(f"[plugin_data]\033[0m根目录正常-\<{path_name}\>")
+        logger.opt(colors=True).debug(f"[plugin_data]根目录正常-\<{path_name}\>")
     else:
         #os.mkdir(path_name)
         os.mkdir(data_dir)
-        logger.opt(colors=True).debug(f"[plugin_data]\033[0m初始化根目录\<{path_name}\>")
+        logger.opt(colors=True).debug(f"[plugin_data]初始化根目录\<{path_name}\>")
 
 def initdata(
     conf_name,
     bashdata:dict={"status":1}
 ):
     conf_path = Path(data_dir / conf_name).absolute()
     config_init(conf_path,conf_name,"plugin_data",bashdata)
@@ -53,16 +52,16 @@
 def config_init(
     _path_ ,
     conf_name:str ,
     module_name:str="None" ,
     data:dict={"status":1}
 ):
     if _path_.is_file():
-        logger.opt(colors=True).debug(f"\033[1;36;43m[util]\033[0m>>><W>{module_name}</>>>>{conf_name}-OK!")
+        logger.opt(colors=True).debug(f"[cubutil]>>><W>{module_name}</>>>>{conf_name}-OK!")
     else:
-        logger.opt(colors=True).debug(f"\033[1;36;43m[util]\033[0m>>><W>{module_name}</>>>>Create-{conf_name}!")
+        logger.opt(colors=True).debug(f"[cubutil]>>><W>{module_name}</>>>>Create-{conf_name}!")
         with open(_path_, "w", encoding="utf-8") as f:
             f.write(json.dumps(data, indent=4))
             f.close()
 
 #本插件由 cubstaryow 编写
 # plugins_data 为 cubplugins_util.plugins_data 移植
```

### Comparing `nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry.egg-info/PKG-INFO` & `nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cyberfurry
-Version: 1.3
+Version: 1.4
 Summary: nonebot插件 cyberfurry-与赛博狼狼对话吧~
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -712,20 +712,21 @@
 </a>
 <img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">
 
 </div>
 
 ## 📖 介绍
 
-官方网站 : https://chat.wingmark.cn
+官方网站 : [CyberFurry](https://chat.wingmark.cn/)
+
 API申请请通过官方群聊找 群主 申请
 
 ### ⚠ 重要
 
-请务必遵守用户协议 https://tailnet.cn/?page=yinyingzc
+请务必遵守 [用户协议](https://tailnet.cn/?page=yinyingzc)
 
 
 easycf模型还未填坑,后续更新适配
 
 ## 💿 安装
 
 <details open>
@@ -767,21 +768,25 @@
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
-若未配置必填项此插件将不会工作!!!!
+
+> [!WARNING]
+> 若未配置必填项此插件将不会工作!!!!
+
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | cf_appid | 是 | 无 | API的appid |
 | cf_token | 是 | 无 | API的token |
 | cubplugin_datadir | 否 | "" | 插件数据文件夹 |
+| cf_enableistome | 否 | False | 在消息是对bot时是否启用chat |
 
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | /chat /cf /yy | 群员 | 否 | 任意 | 触发对话 |
```

### Comparing `nonebot_plugin_cyberfurry-1.3/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt` & `nonebot_plugin_cyberfurry-1.4/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.3/pyproject.toml` & `nonebot_plugin_cyberfurry-1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-cyberfurry"
-version = "1.3"
+version = "1.4"
 description = "nonebot插件 cyberfurry-与赛博狼狼对话吧~"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = ["egg", "bacon", "sausage", "tomatoes", "Lobster Thermidor"]
 authors = [
   {email = "cub_staryow@outlook.com"},
```

