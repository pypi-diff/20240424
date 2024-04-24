# Comparing `tmp/nonebot_plugin_ai_timetable-0.3.6.tar.gz` & `tmp/nonebot_plugin_ai_timetable-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ai_timetable-0.3.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_ai_timetable-0.3.7.tar", max compression
```

## Comparing `nonebot_plugin_ai_timetable-0.3.6.tar` & `nonebot_plugin_ai_timetable-0.3.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-09-02 05:52:20.435566 nonebot_plugin_ai_timetable-0.3.6/LICENSE
--rw-r--r--   0        0        0     8453 2023-09-02 05:52:20.435566 nonebot_plugin_ai_timetable-0.3.6/README.md
--rw-r--r--   0        0        0    11618 2023-09-02 05:52:20.435566 nonebot_plugin_ai_timetable-0.3.6/nonebot_plugin_ai_timetable/__init__.py
--rw-r--r--   0        0        0      359 2023-09-02 05:52:20.435566 nonebot_plugin_ai_timetable-0.3.6/nonebot_plugin_ai_timetable/config.py
--rw-r--r--   0        0        0    20535 2023-09-02 05:52:20.435566 nonebot_plugin_ai_timetable-0.3.6/nonebot_plugin_ai_timetable/utils.py
--rw-r--r--   0        0        0      496 2023-09-02 05:52:20.435566 nonebot_plugin_ai_timetable-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     9172 1970-01-01 00:00:00.000000 nonebot_plugin_ai_timetable-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-24 15:46:45.382998 nonebot_plugin_ai_timetable-0.3.7/LICENSE
+-rw-r--r--   0        0        0     8925 2024-04-24 15:46:45.382998 nonebot_plugin_ai_timetable-0.3.7/README.md
+-rw-r--r--   0        0        0    12197 2024-04-24 15:46:45.382998 nonebot_plugin_ai_timetable-0.3.7/nonebot_plugin_ai_timetable/__init__.py
+-rw-r--r--   0        0        0      359 2024-04-24 15:46:45.382998 nonebot_plugin_ai_timetable-0.3.7/nonebot_plugin_ai_timetable/config.py
+-rw-r--r--   0        0        0    20688 2024-04-24 15:46:45.382998 nonebot_plugin_ai_timetable-0.3.7/nonebot_plugin_ai_timetable/utils.py
+-rw-r--r--   0        0        0      511 2024-04-24 15:46:45.382998 nonebot_plugin_ai_timetable-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     9692 1970-01-01 00:00:00.000000 nonebot_plugin_ai_timetable-0.3.7/PKG-INFO
```

### Comparing `nonebot_plugin_ai_timetable-0.3.6/LICENSE` & `nonebot_plugin_ai_timetable-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ai_timetable-0.3.6/README.md` & `nonebot_plugin_ai_timetable-0.3.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -23,29 +23,31 @@
 ## 💿安装
 
 1. 通过`pip`或`nb`安装；
     - 使用nb(极度推荐)
   
        在机器人目录下命令行使用`nb plugin install nonebot_plugin_ai_timetable`
 
-    - 使用pip(不推荐):
+    - 使用pip:
   
-      ~~既然不推荐就不要想着这样安装了啊喂~~
+      `pip plugin install nonebot_plugin_ai_timetable`
+
+      然后在机器人`pyproject.toml`里的`plugins = []`列表追加`"nonebot_plugin_ai_timetable"`
 
 2. 本地数据保存在`data/ai_timetable/userdata.json`以及`data/ai_timetable/usertable.json`，分别对应用户发送的链接和本地保存的课表
 
 ## 📖简介
 
 1. 傻瓜式一键导入小爱课表，让你的bot实现小爱课表的功能
 
 2. 用户课表数据隔离，无需担心课程时间冲突、不同学校课表不同等问题
 
-3. ~~所以为什么不直接用小爱课表呢~~
+3. 适配多平台，即使是电报涩涩群也要好好学习！🥵🥵
 
-4. ⚙️插件配置
+## ⚙️插件配置
 
 这些配置都已设好默认值，如果想要修改配置，在机器人目录下的.env.*里面可以填写以下选项(可选)
 
 |         config          | type  | default |          example           | usage                                                                                                 |
 | :---------------------: | :---: | :-----: | :------------------------: | :---------------------------------------------------------------------------------------------------- |
 |      TIMETABLE_PIC      | bool  |  true   |    TIMETABLE_PIC=false     | 可选择某日课表以图片/文字发送，默认以图片发送(true)                                                   |
 | TIMETABLE_ALOCK_SOMEDAY |  int  |   22    | TIMETABLE_ALOCK_SOMEDAY=15 | 订阅某日课表的发送时间，必须是0-24的数字                                                              |
@@ -53,92 +55,79 @@
 |   TIMETABLE_SEND_TIME   | float |   0.5   |   TIMETABLE_SEND_TIME=1    | 订阅课程提前发送的时间，单位是`小时`，可以是整数也可以是小数，建议不要设的太大，避免出现无法预料的bug |
 
 ## 💿依赖
 
 ```python
 nb plugin install nonebot_plugin_htmlrender
 nb plugin install nonebot_plugin_apscheduler
+nb plugin install nonebot_plugin_alconna
 ```
-
-若不安装[nonebot_plugin_htmlrender](https://github.com/kexue-z/nonebot-plugin-htmlrender)插件会无法导入在线课表
-
-不安装[nonebot_plugin_apscheduler](https://github.com/nonebot/plugin-apscheduler)会无法使用定时任务,其他功能无影响
-
 ## 🌙更新日志
 
 <details>
 <summary>点击展开</summary>
 
-- 2023-03-05:
-
-    修复了无法取消订阅早八的bug
-
-- 2023-03-06:
-  
-    新增了私聊订阅课表|早八的功能
-
-- 2023-03-07:
-
-1. 修复了时间不会自己改变的bug
-2. 新增了上课/下节课 功能
-3. 优化了一些屎山代码
-
-- 2023-03-08:
-
-1. 修改部分代码，优化课表格式
-2. 修复了节数为11的课会排在节数为2的课程前面的bug(QAQ太蠢了别骂了别骂了)
-
-- 2023-03-11:
-
-1. 修复了如果未登录小米账户就分享课表时的报错,增加错误提示
-2. 新增3项配置项，某日课表可选择以图片发送（默认为图片）
-
-- 2023-03-13：
-
-    修复订阅早八的一些bug
-
-- 2023-03-29:
+- 0.3.7 / 2024-04-24:
+   1. 更新Nonebot2版本至2.2.0
+   2. 基于 [nonebot-plugin-alconna](https://github.com/nonebot/plugin-alconna) 适配多平台
+   3. 放宽httpx限制，移除onebot依赖
+
+- 0.3.6 / 2023-09-02:
+   1. 适配nonebot2.0.1版本：移除过时的RegexMatch方法
+   >如更新本插件后接受消息无响应，请更新你的nonebot版本或回退到旧版本使用
+
+- 0.3.5 / 2023-08-10:
+   1. 格式化代码
+   2. 优化配置读取
+   3. 更新插件元数据
+
+- 0.3.5 / 2023-06-09:
+   1. 更新httpx依赖版本
+
+- 0.3.3 / 2023-04-23:
+   1. 修复定时提醒重复发送的bug
+   2. 修改帮助
+
+- 0.3.2 / 2023-04-14:
+   1. 删去了文本中所有奇怪的口癖喵
+   2. 修复了订阅课程发送时间错误的bug
+
+- 0.3.0 / 2023-04-02:
+   1. 修复bug
+   2. 优化帮助图片
+   3. 定时任务随机延后0-60s，防止风控
+   4. 增加订阅指定课程的功能
+
+- 0.2.3 / 2023-03-29:
+   1. 重构了代码，优化了许多地方~~真的累死了~~
+   2. 修复了一些bug，优化了体验
+   3. 增加了早八|明日早八的查询
+   4. 更新版本后建议重新`导入课表`，避免出现某些bug
+
+- 0.2.1 / 2023-03-13:
+   1. 修复订阅早八的一些bug
+
+- 0.2.0 / 2023-03-11:
+   1. 修复了如果未登录小米账户就分享课表时的报错，增加错误提示
+   2. 新增3项配置项，某日课表可选择以图片发送（默认为图片）
+
+- 0.1.8 / 2023-03-08:
+   1. 修改部分代码，优化课表格式
+   2. 修复了节数为11的课会排在节数为2的课程前面的bug(QAQ太蠢了别骂了别骂了)
+
+- 0.1.7 / 2023-03-07:
+   1. 修复了时间不会自己改变的bug
+   2. 新增了上课/下节课功能
+   3. 优化了一些屎山代码
 
-1. 重构了代码，优化了许多地方~~真的累死了~~
-2. 修复了一些bug，优化了体验
-3. 增加了早八|明日早八的查询
-4. 更新版本后建议重新`导入课表`，避免出现某些bug
+- 0.1.5 / 2023-03-06:
+   1. 新增了私聊订阅课表|早八的功能
 
-- 2023-04-02:
-
-1. 修复bug
-2. 优化帮助图片
-3. 定时任务随机延后0-60s，防止风控
-4. 增加订阅指定课程的功能
-
-- 2023-04-14:
-
-1. 修复了订阅课程发送时间错误的bug
-2. 删去了文本中所有奇怪的口癖喵
-
-- 2023-04-23:
-
-1. 修改帮助
-2. 修复定时提醒重复发送的bug
-
-- 2023-06-09:
-
-1. 更新插件元数据
-2. 优化配置读取
-3. 格式化代码
-
-- 2023-06-09:
-
-    更新httpx依赖版本
-
-- 2023-09-02:
-
-   适配nonebot2.0.1版本：移除过时的RegexMatch方法
-
-    >如更新本插件后接受消息无响应，请更新你的nonebot版本或回退到旧版本使用
+- 0.1.4 / 2023-03-05:
+   1. 修复了无法取消订阅早八的bug
 
 </details>
 
 ## 🎉命令
 
 1. 我的课表|小爱课表|本周课表|下周课表：获取本周|下周的完全课表，使用前须先导入课表，这里的课表是在线课表
 
@@ -196,15 +185,21 @@
 
 - [x] 增加更多的配置项
 
 - [x] 重构代码
 
 - [x] 订阅指定的课
 
-- [ ] 适配插件datastore，接入数据库
+- [x] 多平台适配, 基于 [nonebot-plugin-alconna](https://github.com/nonebot/plugin-alconna) 
+
+- [ ] 支持定时任务本地存储
+
+- [ ] 适配[plugin-rom](https://github.com/nonebot/plugin-orm), 接入数据库
+
+- [ ] 适配更多课表、脱离小爱课表
 
 - [ ] 完善插件
 
 ## 🐛存在的问题
 
  1. 小爱课表分享的链接大概2周后会过期，会使得`我的课表\下周课表`无法使用，需要重新分享，但是仍能使用本地课表，也可以更新本地课表
```

#### html2text {}

```diff
@@ -1,64 +1,65 @@
                                    _[_n_o_n_e_b_o_t_]
                          # nonebot-plugin-ai-timetable
 â¨*åºäºNonebot2çå¯¹æ¥å°ç±è¯¾ç¨è¡¨çæä»¶*â¨_[_n_o_n_e_b_o_t_]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
 ## ð¿å®è£ 1. éè¿`pip`æ`nb`å®è£ï¼ - ä½¿ç¨nb(æåº¦æ¨è)
 å¨æºå¨äººç®å½ä¸å½ä»¤è¡ä½¿ç¨`nb plugin install
-nonebot_plugin_ai_timetable` - ä½¿ç¨pip(ä¸æ¨è):
-~~æ¢ç¶ä¸æ¨èå°±ä¸è¦æ³çè¿æ ·å®è£äºåå~~ 2.
-æ¬å°æ°æ®ä¿å­å¨`data/ai_timetable/userdata.json`ä»¥å`data/ai_timetable/
+nonebot_plugin_ai_timetable` - ä½¿ç¨pip: `pip plugin install
+nonebot_plugin_ai_timetable` ç¶åå¨æºå¨äºº`pyproject.toml`éç`plugins =
+[]`åè¡¨è¿½å `"nonebot_plugin_ai_timetable"` 2. æ¬å°æ°æ®ä¿å­å¨`data/
+ai_timetable/userdata.json`ä»¥å`data/ai_timetable/
 usertable.json`ï¼åå«å¯¹åºç¨æ·åéçé¾æ¥åæ¬å°ä¿å­çè¯¾è¡¨ ##
 ðç®ä» 1.
 å»çå¼ä¸é®å¯¼å¥å°ç±è¯¾è¡¨ï¼è®©ä½ çbotå®ç°å°ç±è¯¾è¡¨çåè½ 2.
 ç¨æ·è¯¾è¡¨æ°æ®éç¦»ï¼æ éæå¿è¯¾ç¨æ¶é´å²çªãä¸åå­¦æ ¡è¯¾è¡¨ä¸åç­é®é¢
-3. ~~æä»¥ä¸ºä»ä¹ä¸ç´æ¥ç¨å°ç±è¯¾è¡¨å¢~~ 4. âï¸æä»¶éç½®
+3. ééå¤å¹³å°ï¼å³ä½¿æ¯çµæ¥æ¶©æ¶©ç¾¤ä¹è¦å¥½å¥½å­¦ä¹ ï¼ð¥µð¥µ ##
+âï¸æä»¶éç½®
 è¿äºéç½®é½å·²è®¾å¥½é»è®¤å¼ï¼å¦ææ³è¦ä¿®æ¹éç½®ï¼å¨æºå¨äººç®å½ä¸ç.env.*éé¢å¯ä»¥å¡«åä»¥ä¸éé¡¹
 (å¯é) | config | type | default | example | usage | | :--------------------
 -: | :---: | :-----: | :------------------------: | :--------------------------
 -------------------------------------------------------------------------- | |
 TIMETABLE_PIC | bool | true | TIMETABLE_PIC=false |
 å¯éæ©ææ¥è¯¾è¡¨ä»¥å¾ç/æå­åéï¼é»è®¤ä»¥å¾çåé(true) | |
 TIMETABLE_ALOCK_SOMEDAY | int | 22 | TIMETABLE_ALOCK_SOMEDAY=15 |
 è®¢éææ¥è¯¾è¡¨çåéæ¶é´ï¼å¿é¡»æ¯0-24çæ°å­ | |
 TIMETABLE_ALOCK_8 | int | 21 | TIMETABLE_ALOCK_8=16 |
 è®¢éæ©å«çåéæ¶é´ï¼å¿é¡»æ¯0-
 24çæ°å­.è¿éåéçé½æ¯ç¬¬äºå¤©çï¼æä»¥å»ºè®®è®¾ç½®ä¸º18-23ç¹ |
 | TIMETABLE_SEND_TIME | float | 0.5 | TIMETABLE_SEND_TIME=1 |
 è®¢éè¯¾ç¨æååéçæ¶é´ï¼åä½æ¯`å°æ¶`ï¼å¯ä»¥æ¯æ´æ°ä¹å¯ä»¥æ¯å°æ°ï¼å»ºè®®ä¸è¦è®¾çå¤ªå¤§ï¼é¿ååºç°æ æ³é¢æçbug
 | ## ð¿ä¾èµ ```python nb plugin install nonebot_plugin_htmlrender nb plugin
-install nonebot_plugin_apscheduler ``` è¥ä¸å®è£[nonebot_plugin_htmlrender]
-(https://github.com/kexue-z/nonebot-plugin-
-htmlrender)æä»¶ä¼æ æ³å¯¼å¥å¨çº¿è¯¾è¡¨ ä¸å®è£
-[nonebot_plugin_apscheduler](https://github.com/nonebot/plugin-
-apscheduler)ä¼æ æ³ä½¿ç¨å®æ¶ä»»å¡,å¶ä»åè½æ å½±å ##
-ðæ´æ°æ¥å¿ ç¹å»å±å¼ - 2023-03-05:
-ä¿®å¤äºæ æ³åæ¶è®¢éæ©å«çbug - 2023-03-06:
-æ°å¢äºç§èè®¢éè¯¾è¡¨|æ©å«çåè½ - 2023-03-07: 1.
-ä¿®å¤äºæ¶é´ä¸ä¼èªå·±æ¹åçbug 2. æ°å¢äºä¸è¯¾/ä¸èè¯¾ åè½ 3.
-ä¼åäºä¸äºå±å±±ä»£ç  - 2023-03-08: 1.
-ä¿®æ¹é¨åä»£ç ï¼ä¼åè¯¾è¡¨æ ¼å¼ 2.
-ä¿®å¤äºèæ°ä¸º11çè¯¾ä¼æå¨èæ°ä¸º2çè¯¾ç¨åé¢çbug
-(QAQå¤ªè ¢äºå«éªäºå«éªäº) - 2023-03-11: 1.
-ä¿®å¤äºå¦ææªç»å½å°ç±³è´¦æ·å°±åäº«è¯¾è¡¨æ¶çæ¥é,å¢å éè¯¯æç¤º
-2.
-æ°å¢3é¡¹éç½®é¡¹ï¼ææ¥è¯¾è¡¨å¯éæ©ä»¥å¾çåéï¼é»è®¤ä¸ºå¾çï¼
-- 2023-03-13ï¼ ä¿®å¤è®¢éæ©å«çä¸äºbug - 2023-03-29: 1.
+install nonebot_plugin_apscheduler nb plugin install nonebot_plugin_alconna ```
+## ðæ´æ°æ¥å¿ ç¹å»å±å¼ - 0.3.7 / 2024-04-24: 1.
+æ´æ°Nonebot2çæ¬è³2.2.0 2. åºäº [nonebot-plugin-alconna](https://
+github.com/nonebot/plugin-alconna) ééå¤å¹³å° 3.
+æ¾å®½httpxéå¶ï¼ç§»é¤onebotä¾èµ - 0.3.6 / 2023-09-02: 1.
+éénonebot2.0.1çæ¬ï¼ç§»é¤è¿æ¶çRegexMatchæ¹æ³
+>å¦æ´æ°æ¬æä»¶åæ¥åæ¶æ¯æ ååºï¼è¯·æ´æ°ä½ çnonebotçæ¬æåéå°æ§çæ¬ä½¿ç¨
+- 0.3.5 / 2023-08-10: 1. æ ¼å¼åä»£ç  2. ä¼åéç½®è¯»å 3.
+æ´æ°æä»¶åæ°æ® - 0.3.5 / 2023-06-09: 1. æ´æ°httpxä¾èµçæ¬ - 0.3.3
+/ 2023-04-23: 1. ä¿®å¤å®æ¶æééå¤åéçbug 2. ä¿®æ¹å¸®å© - 0.3.2 /
+2023-04-14: 1. å å»äºææ¬ä¸­ææå¥æªçå£çåµ 2.
+ä¿®å¤äºè®¢éè¯¾ç¨åéæ¶é´éè¯¯çbug - 0.3.0 / 2023-04-02: 1.
+ä¿®å¤bug 2. ä¼åå¸®å©å¾ç 3. å®æ¶ä»»å¡éæºå»¶å0-60sï¼é²æ­¢é£æ§
+4. å¢å è®¢éæå®è¯¾ç¨çåè½ - 0.2.3 / 2023-03-29: 1.
 éæäºä»£ç ï¼ä¼åäºè®¸å¤å°æ¹~~ççç´¯æ­»äº~~ 2.
 ä¿®å¤äºä¸äºbugï¼ä¼åäºä½éª 3. å¢å äºæ©å«|ææ¥æ©å«çæ¥è¯¢
-4. æ´æ°çæ¬åå»ºè®®éæ°`å¯¼å¥è¯¾è¡¨`ï¼é¿ååºç°æäºbug - 2023-04-
-02: 1. ä¿®å¤bug 2. ä¼åå¸®å©å¾ç 3. å®æ¶ä»»å¡éæºå»¶å0-
-60sï¼é²æ­¢é£æ§ 4. å¢å è®¢éæå®è¯¾ç¨çåè½ - 2023-04-14: 1.
-ä¿®å¤äºè®¢éè¯¾ç¨åéæ¶é´éè¯¯çbug 2.
-å å»äºææ¬ä¸­ææå¥æªçå£çåµ - 2023-04-23: 1. ä¿®æ¹å¸®å© 2.
-ä¿®å¤å®æ¶æééå¤åéçbug - 2023-06-09: 1. æ´æ°æä»¶åæ°æ® 2.
-ä¼åéç½®è¯»å 3. æ ¼å¼åä»£ç  - 2023-06-09: æ´æ°httpxä¾èµçæ¬ -
-2023-09-02: éénonebot2.0.1çæ¬ï¼ç§»é¤è¿æ¶çRegexMatchæ¹æ³
->å¦æ´æ°æ¬æä»¶åæ¥åæ¶æ¯æ ååºï¼è¯·æ´æ°ä½ çnonebotçæ¬æåéå°æ§çæ¬ä½¿ç¨
-## ðå½ä»¤ 1.
+4. æ´æ°çæ¬åå»ºè®®éæ°`å¯¼å¥è¯¾è¡¨`ï¼é¿ååºç°æäºbug - 0.2.1 /
+2023-03-13: 1. ä¿®å¤è®¢éæ©å«çä¸äºbug - 0.2.0 / 2023-03-11: 1.
+ä¿®å¤äºå¦ææªç»å½å°ç±³è´¦æ·å°±åäº«è¯¾è¡¨æ¶çæ¥éï¼å¢å éè¯¯æç¤º
+2.
+æ°å¢3é¡¹éç½®é¡¹ï¼ææ¥è¯¾è¡¨å¯éæ©ä»¥å¾çåéï¼é»è®¤ä¸ºå¾çï¼
+- 0.1.8 / 2023-03-08: 1. ä¿®æ¹é¨åä»£ç ï¼ä¼åè¯¾è¡¨æ ¼å¼ 2.
+ä¿®å¤äºèæ°ä¸º11çè¯¾ä¼æå¨èæ°ä¸º2çè¯¾ç¨åé¢çbug
+(QAQå¤ªè ¢äºå«éªäºå«éªäº) - 0.1.7 / 2023-03-07: 1.
+ä¿®å¤äºæ¶é´ä¸ä¼èªå·±æ¹åçbug 2. æ°å¢äºä¸è¯¾/ä¸èè¯¾åè½ 3.
+ä¼åäºä¸äºå±å±±ä»£ç  - 0.1.5 / 2023-03-06: 1.
+æ°å¢äºç§èè®¢éè¯¾è¡¨|æ©å«çåè½ - 0.1.4 / 2023-03-05: 1.
+ä¿®å¤äºæ æ³åæ¶è®¢éæ©å«çbug ## ðå½ä»¤ 1.
 æçè¯¾è¡¨|å°ç±è¯¾è¡¨|æ¬å¨è¯¾è¡¨|ä¸å¨è¯¾è¡¨ï¼è·åæ¬å¨|ä¸å¨çå®å¨è¯¾è¡¨ï¼ä½¿ç¨åé¡»åå¯¼å¥è¯¾è¡¨ï¼è¿éçè¯¾è¡¨æ¯å¨çº¿è¯¾è¡¨
 2.
 å¯¼å¥è¯¾è¡¨ï¼éè¦æå°ç±è¯¾è¡¨åäº«åºæ¥çé¾æ¥ï¼æå¼å°ç±è¯¾ç¨è¡¨ï¼æå¨æ·»å è¯¾ç¨æä»æå¡å¯¼å¥
 (å·²ééäºå¤§é¨åé«æ ¡)è¯¾ç¨å ![Image text](https://github.com/maoxig/
 nonebot-plugin-ai-timetable/blob/main/resource/export.jpg)
 å¨åºæ¬è®¾ç½®éæå¼å§ä¸è¯¾æ¶é´ç­è°æ´å¥½ä¹å
 (å°¤å¶æ¯æ¶é´ãèæ°)ï¼æåäº«è¯¾è¡¨å¾å°çé¾æ¥åéç»botå³å¯å¯¼å¥æ¬å°
@@ -97,13 +98,16 @@
 -
 å¦æå¯¼å¥è¯¾è¡¨åå¨å°ç±è¯¾è¡¨åä¿®æ¹äºè¯¾ç¨ï¼ç´æ¥ç»botåéæ´æ°è¯¾è¡¨å³å¯æ´æ°æ¬å°è¯¾è¡¨
 -
 å½ä½ ä¸»é¡µçè¯¾è¡¨åå­¦æ ¡è¯¾è¡¨åºæ¬ä¸è´æ¶ï¼é£ä¹å°ç±è¯¾ç¨è¡¨å°±è¢«è°æå¥½äºï¼å¯ä»¥å¯¼å¥äº
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/
 resource/settings.jpg) ## ð¦è®¡å - [x] æ¥è¯¢ä¸èè¯¾çä¿¡æ¯ - [x]
 å¯éæ©æ¯å¦åéå¾çä»¥é¿åé£æ§ - [x] å¢å æ´å¤çéç½®é¡¹ - [x]
-éæä»£ç  - [x] è®¢éæå®çè¯¾ - [ ]
-ééæä»¶datastoreï¼æ¥å¥æ°æ®åº - [ ] å®åæä»¶ ##
+éæä»£ç  - [x] è®¢éæå®çè¯¾ - [x] å¤å¹³å°éé, åºäº [nonebot-
+plugin-alconna](https://github.com/nonebot/plugin-alconna) - [ ]
+æ¯æå®æ¶ä»»å¡æ¬å°å­å¨ - [ ] éé[plugin-rom](https://github.com/
+nonebot/plugin-orm), æ¥å¥æ°æ®åº - [ ]
+ééæ´å¤è¯¾è¡¨ãè±ç¦»å°ç±è¯¾è¡¨ - [ ] å®åæä»¶ ##
 ðå­å¨çé®é¢ 1.
 å°ç±è¯¾è¡¨åäº«çé¾æ¥å¤§æ¦2å¨åä¼è¿æï¼ä¼ä½¿å¾`æçè¯¾è¡¨\ä¸å¨è¯¾è¡¨`æ æ³ä½¿ç¨ï¼éè¦éæ°åäº«ï¼ä½æ¯ä»è½ä½¿ç¨æ¬å°è¯¾è¡¨ï¼ä¹å¯ä»¥æ´æ°æ¬å°è¯¾è¡¨
 2. æºå¨äººéå¯åå®æ¶ä»»å¡ä¼ä¸¢å¤± ##
 åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§QAQ
```

### Comparing `nonebot_plugin_ai_timetable-0.3.6/nonebot_plugin_ai_timetable/__init__.py` & `nonebot_plugin_ai_timetable-0.3.7/nonebot_plugin_ai_timetable/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,26 @@
     scheduler,
     logger,
     config,
     md_to_pic,
     userdata,
     usertable,
 )
-from nonebot.plugin import PluginMetadata
+from nonebot.plugin import PluginMetadata, inherit_supported_adapters
 from nonebot.params import RegexStr, ArgStr, CommandArg, ArgPlainText
 from nonebot.matcher import Matcher
-from nonebot import on_command, on_regex
+from nonebot import on_command, on_regex, require
 import datetime
 import re
 import random
-from nonebot.adapters.onebot.v11 import Bot, MessageSegment, MessageEvent, Message
+from nonebot.adapters import Message, Event, Bot
+
+require("nonebot_plugin_alconna")
+from nonebot_plugin_alconna import UniMessage
+
 from .config import Config
 
 logger.opt(colors=True).info(
     "已检测到软依赖<y>nonebot_plugin_apscheduler</y>, <g>开启定时任务功能</g>"
     if scheduler
     else "未检测到软依赖<y>nonebot_plugin_apscheduler</y>,<r>禁用定时任务功能</r>"
 )
@@ -26,181 +30,215 @@
 __plugin_meta__ = PluginMetadata(
     name="小爱课表",
     description="一键导入课表、查看课表、提醒上课、查询课程",
     usage=AiTimetable.ai_timetable__usage,
     type="application",
     homepage="https://github.com/maoxig/nonebot-plugin-ai-timetable",
     config=Config,
-    supported_adapters={"~onebot.v11"},
+    supported_adapters=inherit_supported_adapters("nonebot_plugin_alconna"),
 )
 
 
 my_table = on_regex(r"^(小爱|我的|本周|下周)(课表)", priority=20, block=False)
 new_table = on_command("导入课表", priority=20, block=False, aliases={"创建课表"})
-table_help = on_command("课表帮助", priority=20, block=False, aliases={"课表介绍", "课表怎么用"})
+table_help = on_command(
+    "课表帮助", priority=20, block=False, aliases={"课表介绍", "课表怎么用"}
+)
 someday_table = on_regex(
     r"^(((今|明|昨|后)(天|日))|(星期|周)(一|二|三|四|五|六|日|天))(课表|的课|课程|((上|有)(什么|啥)课))",
     priority=20,
     block=False,
 )
 add_alock_someday = on_regex(
-    r"^(订阅|提醒)((周|星期)(一|二|三|四|五|六|日|天))(课程|课表|的课)", priority=20, block=True
+    r"^(订阅|提醒)((周|星期)(一|二|三|四|五|六|日|天))(课程|课表|的课)",
+    priority=20,
+    block=True,
+)
+add_alock_morningcalss = on_command(
+    "订阅早八", priority=20, block=True, aliases={"提醒早八"}
 )
-add_alock_morningcalss = on_command("订阅早八", priority=20, block=True, aliases={"提醒早八"})
 remove_alock_someday = on_regex(
-    r"^(取消)(订阅|提醒)((周|星期)(一|二|三|四|五|六|日|天))(课程|的课|课表)", priority=20, block=False
+    r"^(取消)(订阅|提醒)((周|星期)(一|二|三|四|五|六|日|天))(课程|的课|课表)",
+    priority=20,
+    block=False,
 )
 sub_class = on_command("订阅课程", priority=25, block=False, aliases={"提醒课程"})
-remove_sub_class = on_command("取消订阅课程", priority=25, block=False, aliases={"取消提醒课程"})
+remove_sub_class = on_command(
+    "取消订阅课程", priority=25, block=False, aliases={"取消提醒课程"}
+)
 remove_alock_morningclass = on_command(
     "取消订阅早八", priority=20, block=False, aliases={"取消提醒早八"}
 )
 renew_table = on_command("更新本地课表", priority=20, block=False, aliases={"更新课表"})
 send_next_class = on_command("上课", priority=20, block=False, aliases={"下节课"})
-next_morningclass = on_command("早八", priority=20, block=False, aliases={"明日早八", "明天早八"})
+next_morningclass = on_command(
+    "早八", priority=20, block=False, aliases={"明日早八", "明天早八"}
+)
 
 
 @table_help.handle()
 async def _():
     """课表帮助"""
     if config.timetable_pic:
-        await table_help.finish(
-            MessageSegment.image(await md_to_pic(AiTimetable.ai_timetable__usage))
-        )
+        await UniMessage.image(
+            raw=await md_to_pic(AiTimetable.ai_timetable__usage)
+        ).send()
     else:
         await table_help.finish(AiTimetable.ai_timetable__usage)
 
 
 @my_table.handle()
-async def _(event: MessageEvent, key: str = RegexStr()):
+async def _(event: Event, key: str = RegexStr()):
     """获取本周/下周的课表"""
     uid = event.get_user_id()
     if uid in userdata:
         pic = await AiTimetable.my_table(uid=uid, key=key)
-        await my_table.finish(MessageSegment.image(pic))
+        await UniMessage.image(raw=pic).send()
     else:
-        await my_table.finish("你还没有导入课表,发送/导入课表来导入吧！", at_sender=True)
+        await my_table.finish(
+            "你还没有导入课表,发送/导入课表来导入吧！", at_sender=True
+        )
 
 
 @new_table.got("key", "请发送小爱课程表导出的链接,发送/取消以退出")
-async def _(event: MessageEvent, key: str = ArgStr()):
+async def _(event: Event, key: str = ArgStr()):
     """更新本地的课表"""
     uid = event.get_user_id()
     url = str(key)
     if re.match(AiTimetable.base_url_re, url):  # 用户发送的链接匹配
         msg = await AiTimetable.new_table(uid=uid, base_url=key)
         await new_table.finish(msg)
     else:
         await new_table.finish("出错了,请检查链接是否正确", at_sender=True)
 
 
 @someday_table.handle()
-async def _(event: MessageEvent, key: str = RegexStr()):
+async def _(event: Event, key: str = RegexStr()):
     """发送某天的课表"""
     uid = event.get_user_id()
     if uid not in userdata:
-        await someday_table.finish("你还没有导入课表,发送/导入课表来导入吧！", at_sender=True)
+        await someday_table.finish(
+            "你还没有导入课表,发送/导入课表来导入吧！", at_sender=True
+        )
     else:
         if config.timetable_pic:
             pic = await AiTimetable.someday_table(uid=uid, key=key)
-            await someday_table.finish(MessageSegment.image(pic))
+            await UniMessage.image(raw=pic).send()
         else:
             await someday_table.finish(
                 await AiTimetable.someday_table(uid=uid, key=key)
             )
 
 
 @renew_table.handle()  # 更新本地课表
-async def _(event: MessageEvent):
+async def _(event: Event):
     uid = event.get_user_id()
     if uid not in userdata:
-        await renew_table.finish("你还没有导入课表,发送/导入课表来导入吧！", at_sender=True)
+        await renew_table.finish(
+            "你还没有导入课表,发送/导入课表来导入吧！", at_sender=True
+        )
     else:
         msg = await AiTimetable.renew_table(uid=uid)
         await renew_table.finish(msg, at_sender=True)
 
 
 @send_next_class.handle()  # 发送本节课、以及下节课信息
-async def _(event: MessageEvent):
+async def _(event: Event):
     uid = event.get_user_id()
     if uid not in userdata:
-        await send_next_class.finish("你还没有导入课表,发送/导入课表来导入吧！", at_sender=True)
+        await send_next_class.finish(
+            "你还没有导入课表,发送/导入课表来导入吧！", at_sender=True
+        )
     else:
         msg = "现在时间是" + datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         msg += AiTimetable.now_class(uid)
         msg += AiTimetable.next_class(uid)
         await send_next_class.finish(msg, at_sender=True)
 
 
 @next_morningclass.handle()
-async def _(bot: Bot, event: MessageEvent):
+async def _(bot: Bot, event: Event):
     """发送早八"""
     uid = event.get_user_id()
     if uid not in userdata:
-        await send_next_class.finish("你还没有导入课表,发送/导入课表来导入吧！", at_sender=True)
+        await send_next_class.finish(
+            "你还没有导入课表,发送/导入课表来导入吧！", at_sender=True
+        )
     else:
         await AiTimetable.post_alock_morningclass(uid=uid, bot=bot, event=event)
 
 
 # -----------以下为定时任务----------------#
 
 
 @add_alock_someday.handle()
-async def _(bot: Bot, event: MessageEvent, key: str = RegexStr()):
+async def _(bot: Bot, event: Event, key: str = RegexStr()):
     """订阅课表"""
     uid = event.get_user_id()
     if uid not in userdata:
-        await add_alock_someday.finish("你还没有导入课表,发送/导入课表来导入吧！", at_sender=True)
+        await add_alock_someday.finish(
+            "你还没有导入课表,发送/导入课表来导入吧！", at_sender=True
+        )
     else:
         if scheduler:
             send_day = (AiTimetable.weekday_int(key) + 5) % 7
             if scheduler.get_job(str(uid + "post_alock" + str(send_day))):
-                await add_alock_someday.finish("出错了！你好像已经订阅过这天的课表了呢", at_sender=True)
+                await add_alock_someday.finish(
+                    "出错了！你好像已经订阅过这天的课表了呢", at_sender=True
+                )
             scheduler.add_job(
                 AiTimetable.post_alock,
                 "cron",
                 hour=config.timetable_alock_someday,
                 second=random.randint(0, 60),
                 id=str(uid + "post_alock" + str(send_day)),
                 day_of_week=send_day,
                 kwargs={"key": key, "uid": uid, "bot": bot, "event": event},
             )
             await add_alock_someday.finish("定时提醒添加成功！", at_sender=True)
         else:
-            await add_alock_someday.finish("apscheduler插件未载入,无法添加定时提醒", at_sender=True)
+            await add_alock_someday.finish(
+                "apscheduler插件未载入,无法添加定时提醒", at_sender=True
+            )
 
 
 @remove_alock_someday.handle()
-async def _(bot: Bot, event: MessageEvent, key: str = RegexStr()):
+async def _(bot: Bot, event: Event, key: str = RegexStr()):
     """删除订阅课表"""
     uid = event.get_user_id()
     if uid not in userdata:
-        await add_alock_someday.finish("你还没有导入课表,发送/导入课表来导入吧！", at_sender=True)
+        await add_alock_someday.finish(
+            "你还没有导入课表,发送/导入课表来导入吧！", at_sender=True
+        )
     else:
         if scheduler:
             send_day = (AiTimetable.weekday_int(key) + 5) % 7
             if scheduler.get_job(str(uid + "post_alock" + str(send_day))):
                 scheduler.remove_job(str(uid + "post_alock" + str(send_day)))
                 await remove_alock_someday.finish("定时提醒删除成功！", at_sender=True)
             else:
-                await remove_alock_someday.finish("出错了,好像没有订阅过这天的课表呢", at_sender=True)
+                await remove_alock_someday.finish(
+                    "出错了,好像没有订阅过这天的课表呢", at_sender=True
+                )
         else:
             await remove_alock_someday.finish(
                 "apscheduler插件未载入,无法删除定时提醒", at_sender=True
             )
 
 
 # -----------以下为订阅早八----------------#
 
 
 @add_alock_morningcalss.handle()
-async def _(bot: Bot, event: MessageEvent):
+async def _(bot: Bot, event: Event):
     uid = event.get_user_id()
     if uid not in userdata:
-        await add_alock_morningcalss.finish("你还没有导入课表,发送/导入课表来导入吧！", at_sender=True)
+        await add_alock_morningcalss.finish(
+            "你还没有导入课表,发送/导入课表来导入吧！", at_sender=True
+        )
     else:
         if scheduler:
             if scheduler.get_job(str(uid + "post_alock_morningclass")):
                 await add_alock_morningcalss.finish(
                     "出错了！你好像已经订阅过早八提醒了呢", at_sender=True
                 )
             scheduler.add_job(
@@ -215,60 +253,74 @@
         else:
             await add_alock_morningcalss.finish(
                 "apscheduler插件未载入,无法添加定时提醒", at_sender=True
             )
 
 
 @remove_alock_morningclass.handle()
-async def _(event: MessageEvent):
+async def _(event: Event):
     uid = event.get_user_id()
     if uid not in userdata:
-        await remove_alock_morningclass.finish("你还没有导入课表,发送/导入课表来导入吧！", at_sender=True)
+        await remove_alock_morningclass.finish(
+            "你还没有导入课表,发送/导入课表来导入吧！", at_sender=True
+        )
     else:
         if scheduler:
             if scheduler.get_job(str(uid + "post_alock_morningclass")):
                 scheduler.remove_job(str(uid + "post_alock_morningclass"))
-                await remove_alock_morningclass.finish("定时提醒删除成功！", at_sender=True)
+                await remove_alock_morningclass.finish(
+                    "定时提醒删除成功！", at_sender=True
+                )
             else:
-                await remove_alock_morningclass.finish("出错了,好像没有订阅过早八呢", at_sender=True)
+                await remove_alock_morningclass.finish(
+                    "出错了,好像没有订阅过早八呢", at_sender=True
+                )
         else:
             await remove_alock_morningclass.finish(
                 "apscheduler插件未载入,无法删除定时提醒", at_sender=True
             )
 
 
 @sub_class.handle()
 async def _(matcher: Matcher, args: Message = CommandArg()):
     if args.extract_plain_text():
         matcher.set_arg("text", args)
 
 
 @sub_class.got("text", prompt="请告诉我课程名~")
-async def sub_handler(bot: Bot, event: MessageEvent, text: str = ArgPlainText()):
+async def sub_handler(bot: Bot, event: Event, text: str = ArgPlainText()):
     uid = event.get_user_id()
     if uid not in userdata:
-        await sub_class.finish("你还没有导入课表,发送/导入课表来导入吧！", at_sender=True)
+        await sub_class.finish(
+            "你还没有导入课表,发送/导入课表来导入吧！", at_sender=True
+        )
     else:
         if scheduler:
             msg = AiTimetable.sub_class(uid=uid, key=text, event=event, bot=bot)
             await sub_class.finish(msg, at_sender=True)
         else:
-            await sub_class.finish("apscheduler插件未载入,无法添加定时提醒", at_sender=True)
+            await sub_class.finish(
+                "apscheduler插件未载入,无法添加定时提醒", at_sender=True
+            )
 
 
 @remove_sub_class.handle()
 async def _(matcher: Matcher, args: Message = CommandArg()):
     if args.extract_plain_text():
         matcher.set_arg("text", args)
 
 
 @remove_sub_class.got("text", prompt="请告诉我课程名~")
-async def remove_sub_handler(event: MessageEvent, text: str = ArgPlainText()):
+async def remove_sub_handler(event: Event, text: str = ArgPlainText()):
     uid = event.get_user_id()
     if uid not in userdata:
-        await remove_sub_class.finish("你还没有导入课表,发送/导入课表来导入吧！", at_sender=True)
+        await remove_sub_class.finish(
+            "你还没有导入课表,发送/导入课表来导入吧！", at_sender=True
+        )
     else:
         if scheduler:
             msg = AiTimetable.remove_sub_class(uid=uid, key=text)
             await remove_sub_class.finish(msg, at_sender=True)
         else:
-            await remove_sub_class.finish("apscheduler插件未载入,无法添加定时提醒", at_sender=True)
+            await remove_sub_class.finish(
+                "apscheduler插件未载入,无法添加定时提醒", at_sender=True
+            )
```

### Comparing `nonebot_plugin_ai_timetable-0.3.6/nonebot_plugin_ai_timetable/utils.py` & `nonebot_plugin_ai_timetable-0.3.7/nonebot_plugin_ai_timetable/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-from nonebot.adapters.onebot.v11 import ActionFailed, MessageSegment
-from nonebot import get_driver, logger, require
+from nonebot import logger, require, get_plugin_config
+from nonebot.exception import ActionFailed
 
 require("nonebot_plugin_htmlrender")
 require("nonebot_plugin_apscheduler")
+require("nonebot_plugin_alconna")
+from nonebot_plugin_alconna import UniMessage
 from nonebot_plugin_apscheduler import scheduler
 from nonebot_plugin_htmlrender import get_new_page, md_to_pic
 import os
 import re
 import json
 import time
 import datetime
 import httpx
 import random
 from .config import Config
 
-global_config = get_driver().config
-config = Config.parse_obj(global_config)
+
+config = get_plugin_config(Config)
+
 if os.path.exists("data/ai_timetable/userdata.json"):
     with open("data/ai_timetable/userdata.json", "r", encoding="utf-8") as f:
         userdata = json.load(f)
 else:
     if not os.path.exists("data/ai_timetable"):
         os.makedirs("data/ai_timetable")
     userdata = {}
@@ -380,15 +383,15 @@
                         + "\n"
                         + courses["teacher"]
                     )
             if count == 0:
                 msg += "\n你明天没有早八呢！享受夜生活吧！"
             else:
                 msg += f"\n你明天有{count}节早八呢！今晚早点休息吧！"
-            await bot.send(event, message=msg, at_sender=True)
+            await UniMessage.text(msg).send(target=event, bot=bot, at_sender=True)
         except ActionFailed as e:
             logger.warning(f"发送消息给{event.get_user_id()}失败：{e}")
 
     @classmethod
     async def post_alock(cls, **kwargs):
         """发送第二天课程消息"""
         key, uid, bot, event = (
@@ -399,17 +402,19 @@
         )
         if "一" in key:
             key = "明"
         msg = cls.table_msg(key=key, uid=uid)
         try:
             if config.timetable_pic:
                 pic = await md_to_pic(md=msg)
-                await bot.send(event, MessageSegment.image(file=pic), at_sender=True)
+                await UniMessage.image(raw=pic).send(
+                    target=event, bot=bot, at_sender=True
+                )
             else:
-                await bot.send(event, message=msg, at_sender=True)
+                await UniMessage.text(msg).send(target=event, bot=bot, at_sender=True)
         except ActionFailed as e:
             logger.warning(f"发送消息失败：{e}")
 
     @classmethod
     def sub_class(cls, **kwargs) -> str:
         """订阅一周内所有课程名中有key的课程"""
         uid, key, bot, event = (
@@ -429,15 +434,17 @@
                     class_section = int(courses["sections"].split(",")[0])
                     starttime = eval(usertable[uid]["data"]["setting"]["sectionTimes"])[
                         class_section - 1
                     ][
                         "s"
                     ]  # 获取课程开始时间
                     hours = int(config.timetable_send_time)  # 从设置中获取提前的小时数
-                    minutes = int((config.timetable_send_time - hours) * 60)  # 从设置中获取提前的分钟数
+                    minutes = int(
+                        (config.timetable_send_time - hours) * 60
+                    )  # 从设置中获取提前的分钟数
                     time_obj = datetime.datetime.strptime(
                         starttime, "%H:%M"
                     )  # 将字符串转换为datetime
                     new_time_obj = time_obj - datetime.timedelta(
                         hours=hours, minutes=minutes
                     )  # 进行时间的运算
                     sub_hour = new_time_obj.hour  # 获取发送时间的小时
@@ -491,10 +498,10 @@
             msg = "现在时间是" + datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
             msg += "\n还有{}小时，你订阅的课程就要开始啦！课程信息如下:\n{}\n{}\n{}".format(
                 config.timetable_send_time,
                 course["name"],
                 course["position"],
                 course["teacher"],
             )
-            await bot.send(event, message=MessageSegment.at(uid) + msg, at_sender=True)
+            await UniMessage.text(msg).send(target=event, bot=bot, at_sender=True)
         except ActionFailed as e:
             logger.warning(f"发送消息给{event.get_user_id()}失败：{e}")
```

### Comparing `nonebot_plugin_ai_timetable-0.3.6/PKG-INFO` & `nonebot_plugin_ai_timetable-0.3.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-ai-timetable
-Version: 0.3.6
+Version: 0.3.7
 Summary: 小爱课程表
 Author: maoxiog
 Author-email: 674550338@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: httpx (>=0.24.0,<0.25.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.1.0,<3.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: httpx (>=0.20.0,<1.0.0)
+Requires-Dist: nonebot-plugin-alconna (>=0.40.1,<1.0.0)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0,<0.3.0)
-Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0)
+Requires-Dist: nonebot2 (>=2.2.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 <div align="center">
 
@@ -42,29 +43,31 @@
 ## 💿安装
 
 1. 通过`pip`或`nb`安装；
     - 使用nb(极度推荐)
   
        在机器人目录下命令行使用`nb plugin install nonebot_plugin_ai_timetable`
 
-    - 使用pip(不推荐):
+    - 使用pip:
   
-      ~~既然不推荐就不要想着这样安装了啊喂~~
+      `pip plugin install nonebot_plugin_ai_timetable`
+
+      然后在机器人`pyproject.toml`里的`plugins = []`列表追加`"nonebot_plugin_ai_timetable"`
 
 2. 本地数据保存在`data/ai_timetable/userdata.json`以及`data/ai_timetable/usertable.json`，分别对应用户发送的链接和本地保存的课表
 
 ## 📖简介
 
 1. 傻瓜式一键导入小爱课表，让你的bot实现小爱课表的功能
 
 2. 用户课表数据隔离，无需担心课程时间冲突、不同学校课表不同等问题
 
-3. ~~所以为什么不直接用小爱课表呢~~
+3. 适配多平台，即使是电报涩涩群也要好好学习！🥵🥵
 
-4. ⚙️插件配置
+## ⚙️插件配置
 
 这些配置都已设好默认值，如果想要修改配置，在机器人目录下的.env.*里面可以填写以下选项(可选)
 
 |         config          | type  | default |          example           | usage                                                                                                 |
 | :---------------------: | :---: | :-----: | :------------------------: | :---------------------------------------------------------------------------------------------------- |
 |      TIMETABLE_PIC      | bool  |  true   |    TIMETABLE_PIC=false     | 可选择某日课表以图片/文字发送，默认以图片发送(true)                                                   |
 | TIMETABLE_ALOCK_SOMEDAY |  int  |   22    | TIMETABLE_ALOCK_SOMEDAY=15 | 订阅某日课表的发送时间，必须是0-24的数字                                                              |
@@ -72,92 +75,79 @@
 |   TIMETABLE_SEND_TIME   | float |   0.5   |   TIMETABLE_SEND_TIME=1    | 订阅课程提前发送的时间，单位是`小时`，可以是整数也可以是小数，建议不要设的太大，避免出现无法预料的bug |
 
 ## 💿依赖
 
 ```python
 nb plugin install nonebot_plugin_htmlrender
 nb plugin install nonebot_plugin_apscheduler
+nb plugin install nonebot_plugin_alconna
 ```
-
-若不安装[nonebot_plugin_htmlrender](https://github.com/kexue-z/nonebot-plugin-htmlrender)插件会无法导入在线课表
-
-不安装[nonebot_plugin_apscheduler](https://github.com/nonebot/plugin-apscheduler)会无法使用定时任务,其他功能无影响
-
 ## 🌙更新日志
 
 <details>
 <summary>点击展开</summary>
 
-- 2023-03-05:
-
-    修复了无法取消订阅早八的bug
-
-- 2023-03-06:
-  
-    新增了私聊订阅课表|早八的功能
-
-- 2023-03-07:
-
-1. 修复了时间不会自己改变的bug
-2. 新增了上课/下节课 功能
-3. 优化了一些屎山代码
-
-- 2023-03-08:
-
-1. 修改部分代码，优化课表格式
-2. 修复了节数为11的课会排在节数为2的课程前面的bug(QAQ太蠢了别骂了别骂了)
-
-- 2023-03-11:
-
-1. 修复了如果未登录小米账户就分享课表时的报错,增加错误提示
-2. 新增3项配置项，某日课表可选择以图片发送（默认为图片）
-
-- 2023-03-13：
-
-    修复订阅早八的一些bug
-
-- 2023-03-29:
+- 0.3.7 / 2024-04-24:
+   1. 更新Nonebot2版本至2.2.0
+   2. 基于 [nonebot-plugin-alconna](https://github.com/nonebot/plugin-alconna) 适配多平台
+   3. 放宽httpx限制，移除onebot依赖
+
+- 0.3.6 / 2023-09-02:
+   1. 适配nonebot2.0.1版本：移除过时的RegexMatch方法
+   >如更新本插件后接受消息无响应，请更新你的nonebot版本或回退到旧版本使用
+
+- 0.3.5 / 2023-08-10:
+   1. 格式化代码
+   2. 优化配置读取
+   3. 更新插件元数据
+
+- 0.3.5 / 2023-06-09:
+   1. 更新httpx依赖版本
+
+- 0.3.3 / 2023-04-23:
+   1. 修复定时提醒重复发送的bug
+   2. 修改帮助
+
+- 0.3.2 / 2023-04-14:
+   1. 删去了文本中所有奇怪的口癖喵
+   2. 修复了订阅课程发送时间错误的bug
+
+- 0.3.0 / 2023-04-02:
+   1. 修复bug
+   2. 优化帮助图片
+   3. 定时任务随机延后0-60s，防止风控
+   4. 增加订阅指定课程的功能
+
+- 0.2.3 / 2023-03-29:
+   1. 重构了代码，优化了许多地方~~真的累死了~~
+   2. 修复了一些bug，优化了体验
+   3. 增加了早八|明日早八的查询
+   4. 更新版本后建议重新`导入课表`，避免出现某些bug
+
+- 0.2.1 / 2023-03-13:
+   1. 修复订阅早八的一些bug
+
+- 0.2.0 / 2023-03-11:
+   1. 修复了如果未登录小米账户就分享课表时的报错，增加错误提示
+   2. 新增3项配置项，某日课表可选择以图片发送（默认为图片）
+
+- 0.1.8 / 2023-03-08:
+   1. 修改部分代码，优化课表格式
+   2. 修复了节数为11的课会排在节数为2的课程前面的bug(QAQ太蠢了别骂了别骂了)
+
+- 0.1.7 / 2023-03-07:
+   1. 修复了时间不会自己改变的bug
+   2. 新增了上课/下节课功能
+   3. 优化了一些屎山代码
 
-1. 重构了代码，优化了许多地方~~真的累死了~~
-2. 修复了一些bug，优化了体验
-3. 增加了早八|明日早八的查询
-4. 更新版本后建议重新`导入课表`，避免出现某些bug
+- 0.1.5 / 2023-03-06:
+   1. 新增了私聊订阅课表|早八的功能
 
-- 2023-04-02:
-
-1. 修复bug
-2. 优化帮助图片
-3. 定时任务随机延后0-60s，防止风控
-4. 增加订阅指定课程的功能
-
-- 2023-04-14:
-
-1. 修复了订阅课程发送时间错误的bug
-2. 删去了文本中所有奇怪的口癖喵
-
-- 2023-04-23:
-
-1. 修改帮助
-2. 修复定时提醒重复发送的bug
-
-- 2023-06-09:
-
-1. 更新插件元数据
-2. 优化配置读取
-3. 格式化代码
-
-- 2023-06-09:
-
-    更新httpx依赖版本
-
-- 2023-09-02:
-
-   适配nonebot2.0.1版本：移除过时的RegexMatch方法
-
-    >如更新本插件后接受消息无响应，请更新你的nonebot版本或回退到旧版本使用
+- 0.1.4 / 2023-03-05:
+   1. 修复了无法取消订阅早八的bug
 
 </details>
 
 ## 🎉命令
 
 1. 我的课表|小爱课表|本周课表|下周课表：获取本周|下周的完全课表，使用前须先导入课表，这里的课表是在线课表
 
@@ -215,15 +205,21 @@
 
 - [x] 增加更多的配置项
 
 - [x] 重构代码
 
 - [x] 订阅指定的课
 
-- [ ] 适配插件datastore，接入数据库
+- [x] 多平台适配, 基于 [nonebot-plugin-alconna](https://github.com/nonebot/plugin-alconna) 
+
+- [ ] 支持定时任务本地存储
+
+- [ ] 适配[plugin-rom](https://github.com/nonebot/plugin-orm), 接入数据库
+
+- [ ] 适配更多课表、脱离小爱课表
 
 - [ ] 完善插件
 
 ## 🐛存在的问题
 
  1. 小爱课表分享的链接大概2周后会过期，会使得`我的课表\下周课表`无法使用，需要重新分享，但是仍能使用本地课表，也可以更新本地课表
```

#### html2text {}

```diff
@@ -1,74 +1,76 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-ai-timetable Version: 0.3.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-ai-timetable Version: 0.3.7 Summary:
 å°ç±è¯¾ç¨è¡¨ Author: maoxiog Author-email: 674550338@qq.com Requires-Python:
 >=3.8,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Dist: httpx (>=0.24.0,<0.25.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.1.0,<3.0.0) Requires-Dist: nonebot-
-plugin-apscheduler (>=0.2.0,<0.3.0) Requires-Dist: nonebot-plugin-htmlrender
-(>=0.2.0,<0.3.0) Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0) Description-
-Content-Type: text/markdown
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-Dist: nonebot-
+plugin-alconna (>=0.40.1,<1.0.0) Requires-Dist: nonebot-plugin-apscheduler
+(>=0.2.0,<0.3.0) Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0,<0.3.0)
+Requires-Dist: nonebot2 (>=2.2.0,<3.0.0) Description-Content-Type: text/
+markdown
                                    _[_n_o_n_e_b_o_t_]
                          # nonebot-plugin-ai-timetable
 â¨*åºäºNonebot2çå¯¹æ¥å°ç±è¯¾ç¨è¡¨çæä»¶*â¨_[_n_o_n_e_b_o_t_]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
 ## ð¿å®è£ 1. éè¿`pip`æ`nb`å®è£ï¼ - ä½¿ç¨nb(æåº¦æ¨è)
 å¨æºå¨äººç®å½ä¸å½ä»¤è¡ä½¿ç¨`nb plugin install
-nonebot_plugin_ai_timetable` - ä½¿ç¨pip(ä¸æ¨è):
-~~æ¢ç¶ä¸æ¨èå°±ä¸è¦æ³çè¿æ ·å®è£äºåå~~ 2.
-æ¬å°æ°æ®ä¿å­å¨`data/ai_timetable/userdata.json`ä»¥å`data/ai_timetable/
+nonebot_plugin_ai_timetable` - ä½¿ç¨pip: `pip plugin install
+nonebot_plugin_ai_timetable` ç¶åå¨æºå¨äºº`pyproject.toml`éç`plugins =
+[]`åè¡¨è¿½å `"nonebot_plugin_ai_timetable"` 2. æ¬å°æ°æ®ä¿å­å¨`data/
+ai_timetable/userdata.json`ä»¥å`data/ai_timetable/
 usertable.json`ï¼åå«å¯¹åºç¨æ·åéçé¾æ¥åæ¬å°ä¿å­çè¯¾è¡¨ ##
 ðç®ä» 1.
 å»çå¼ä¸é®å¯¼å¥å°ç±è¯¾è¡¨ï¼è®©ä½ çbotå®ç°å°ç±è¯¾è¡¨çåè½ 2.
 ç¨æ·è¯¾è¡¨æ°æ®éç¦»ï¼æ éæå¿è¯¾ç¨æ¶é´å²çªãä¸åå­¦æ ¡è¯¾è¡¨ä¸åç­é®é¢
-3. ~~æä»¥ä¸ºä»ä¹ä¸ç´æ¥ç¨å°ç±è¯¾è¡¨å¢~~ 4. âï¸æä»¶éç½®
+3. ééå¤å¹³å°ï¼å³ä½¿æ¯çµæ¥æ¶©æ¶©ç¾¤ä¹è¦å¥½å¥½å­¦ä¹ ï¼ð¥µð¥µ ##
+âï¸æä»¶éç½®
 è¿äºéç½®é½å·²è®¾å¥½é»è®¤å¼ï¼å¦ææ³è¦ä¿®æ¹éç½®ï¼å¨æºå¨äººç®å½ä¸ç.env.*éé¢å¯ä»¥å¡«åä»¥ä¸éé¡¹
 (å¯é) | config | type | default | example | usage | | :--------------------
 -: | :---: | :-----: | :------------------------: | :--------------------------
 -------------------------------------------------------------------------- | |
 TIMETABLE_PIC | bool | true | TIMETABLE_PIC=false |
 å¯éæ©ææ¥è¯¾è¡¨ä»¥å¾ç/æå­åéï¼é»è®¤ä»¥å¾çåé(true) | |
 TIMETABLE_ALOCK_SOMEDAY | int | 22 | TIMETABLE_ALOCK_SOMEDAY=15 |
 è®¢éææ¥è¯¾è¡¨çåéæ¶é´ï¼å¿é¡»æ¯0-24çæ°å­ | |
 TIMETABLE_ALOCK_8 | int | 21 | TIMETABLE_ALOCK_8=16 |
 è®¢éæ©å«çåéæ¶é´ï¼å¿é¡»æ¯0-
 24çæ°å­.è¿éåéçé½æ¯ç¬¬äºå¤©çï¼æä»¥å»ºè®®è®¾ç½®ä¸º18-23ç¹ |
 | TIMETABLE_SEND_TIME | float | 0.5 | TIMETABLE_SEND_TIME=1 |
 è®¢éè¯¾ç¨æååéçæ¶é´ï¼åä½æ¯`å°æ¶`ï¼å¯ä»¥æ¯æ´æ°ä¹å¯ä»¥æ¯å°æ°ï¼å»ºè®®ä¸è¦è®¾çå¤ªå¤§ï¼é¿ååºç°æ æ³é¢æçbug
 | ## ð¿ä¾èµ ```python nb plugin install nonebot_plugin_htmlrender nb plugin
-install nonebot_plugin_apscheduler ``` è¥ä¸å®è£[nonebot_plugin_htmlrender]
-(https://github.com/kexue-z/nonebot-plugin-
-htmlrender)æä»¶ä¼æ æ³å¯¼å¥å¨çº¿è¯¾è¡¨ ä¸å®è£
-[nonebot_plugin_apscheduler](https://github.com/nonebot/plugin-
-apscheduler)ä¼æ æ³ä½¿ç¨å®æ¶ä»»å¡,å¶ä»åè½æ å½±å ##
-ðæ´æ°æ¥å¿ ç¹å»å±å¼ - 2023-03-05:
-ä¿®å¤äºæ æ³åæ¶è®¢éæ©å«çbug - 2023-03-06:
-æ°å¢äºç§èè®¢éè¯¾è¡¨|æ©å«çåè½ - 2023-03-07: 1.
-ä¿®å¤äºæ¶é´ä¸ä¼èªå·±æ¹åçbug 2. æ°å¢äºä¸è¯¾/ä¸èè¯¾ åè½ 3.
-ä¼åäºä¸äºå±å±±ä»£ç  - 2023-03-08: 1.
-ä¿®æ¹é¨åä»£ç ï¼ä¼åè¯¾è¡¨æ ¼å¼ 2.
-ä¿®å¤äºèæ°ä¸º11çè¯¾ä¼æå¨èæ°ä¸º2çè¯¾ç¨åé¢çbug
-(QAQå¤ªè ¢äºå«éªäºå«éªäº) - 2023-03-11: 1.
-ä¿®å¤äºå¦ææªç»å½å°ç±³è´¦æ·å°±åäº«è¯¾è¡¨æ¶çæ¥é,å¢å éè¯¯æç¤º
-2.
-æ°å¢3é¡¹éç½®é¡¹ï¼ææ¥è¯¾è¡¨å¯éæ©ä»¥å¾çåéï¼é»è®¤ä¸ºå¾çï¼
-- 2023-03-13ï¼ ä¿®å¤è®¢éæ©å«çä¸äºbug - 2023-03-29: 1.
+install nonebot_plugin_apscheduler nb plugin install nonebot_plugin_alconna ```
+## ðæ´æ°æ¥å¿ ç¹å»å±å¼ - 0.3.7 / 2024-04-24: 1.
+æ´æ°Nonebot2çæ¬è³2.2.0 2. åºäº [nonebot-plugin-alconna](https://
+github.com/nonebot/plugin-alconna) ééå¤å¹³å° 3.
+æ¾å®½httpxéå¶ï¼ç§»é¤onebotä¾èµ - 0.3.6 / 2023-09-02: 1.
+éénonebot2.0.1çæ¬ï¼ç§»é¤è¿æ¶çRegexMatchæ¹æ³
+>å¦æ´æ°æ¬æä»¶åæ¥åæ¶æ¯æ ååºï¼è¯·æ´æ°ä½ çnonebotçæ¬æåéå°æ§çæ¬ä½¿ç¨
+- 0.3.5 / 2023-08-10: 1. æ ¼å¼åä»£ç  2. ä¼åéç½®è¯»å 3.
+æ´æ°æä»¶åæ°æ® - 0.3.5 / 2023-06-09: 1. æ´æ°httpxä¾èµçæ¬ - 0.3.3
+/ 2023-04-23: 1. ä¿®å¤å®æ¶æééå¤åéçbug 2. ä¿®æ¹å¸®å© - 0.3.2 /
+2023-04-14: 1. å å»äºææ¬ä¸­ææå¥æªçå£çåµ 2.
+ä¿®å¤äºè®¢éè¯¾ç¨åéæ¶é´éè¯¯çbug - 0.3.0 / 2023-04-02: 1.
+ä¿®å¤bug 2. ä¼åå¸®å©å¾ç 3. å®æ¶ä»»å¡éæºå»¶å0-60sï¼é²æ­¢é£æ§
+4. å¢å è®¢éæå®è¯¾ç¨çåè½ - 0.2.3 / 2023-03-29: 1.
 éæäºä»£ç ï¼ä¼åäºè®¸å¤å°æ¹~~ççç´¯æ­»äº~~ 2.
 ä¿®å¤äºä¸äºbugï¼ä¼åäºä½éª 3. å¢å äºæ©å«|ææ¥æ©å«çæ¥è¯¢
-4. æ´æ°çæ¬åå»ºè®®éæ°`å¯¼å¥è¯¾è¡¨`ï¼é¿ååºç°æäºbug - 2023-04-
-02: 1. ä¿®å¤bug 2. ä¼åå¸®å©å¾ç 3. å®æ¶ä»»å¡éæºå»¶å0-
-60sï¼é²æ­¢é£æ§ 4. å¢å è®¢éæå®è¯¾ç¨çåè½ - 2023-04-14: 1.
-ä¿®å¤äºè®¢éè¯¾ç¨åéæ¶é´éè¯¯çbug 2.
-å å»äºææ¬ä¸­ææå¥æªçå£çåµ - 2023-04-23: 1. ä¿®æ¹å¸®å© 2.
-ä¿®å¤å®æ¶æééå¤åéçbug - 2023-06-09: 1. æ´æ°æä»¶åæ°æ® 2.
-ä¼åéç½®è¯»å 3. æ ¼å¼åä»£ç  - 2023-06-09: æ´æ°httpxä¾èµçæ¬ -
-2023-09-02: éénonebot2.0.1çæ¬ï¼ç§»é¤è¿æ¶çRegexMatchæ¹æ³
->å¦æ´æ°æ¬æä»¶åæ¥åæ¶æ¯æ ååºï¼è¯·æ´æ°ä½ çnonebotçæ¬æåéå°æ§çæ¬ä½¿ç¨
-## ðå½ä»¤ 1.
+4. æ´æ°çæ¬åå»ºè®®éæ°`å¯¼å¥è¯¾è¡¨`ï¼é¿ååºç°æäºbug - 0.2.1 /
+2023-03-13: 1. ä¿®å¤è®¢éæ©å«çä¸äºbug - 0.2.0 / 2023-03-11: 1.
+ä¿®å¤äºå¦ææªç»å½å°ç±³è´¦æ·å°±åäº«è¯¾è¡¨æ¶çæ¥éï¼å¢å éè¯¯æç¤º
+2.
+æ°å¢3é¡¹éç½®é¡¹ï¼ææ¥è¯¾è¡¨å¯éæ©ä»¥å¾çåéï¼é»è®¤ä¸ºå¾çï¼
+- 0.1.8 / 2023-03-08: 1. ä¿®æ¹é¨åä»£ç ï¼ä¼åè¯¾è¡¨æ ¼å¼ 2.
+ä¿®å¤äºèæ°ä¸º11çè¯¾ä¼æå¨èæ°ä¸º2çè¯¾ç¨åé¢çbug
+(QAQå¤ªè ¢äºå«éªäºå«éªäº) - 0.1.7 / 2023-03-07: 1.
+ä¿®å¤äºæ¶é´ä¸ä¼èªå·±æ¹åçbug 2. æ°å¢äºä¸è¯¾/ä¸èè¯¾åè½ 3.
+ä¼åäºä¸äºå±å±±ä»£ç  - 0.1.5 / 2023-03-06: 1.
+æ°å¢äºç§èè®¢éè¯¾è¡¨|æ©å«çåè½ - 0.1.4 / 2023-03-05: 1.
+ä¿®å¤äºæ æ³åæ¶è®¢éæ©å«çbug ## ðå½ä»¤ 1.
 æçè¯¾è¡¨|å°ç±è¯¾è¡¨|æ¬å¨è¯¾è¡¨|ä¸å¨è¯¾è¡¨ï¼è·åæ¬å¨|ä¸å¨çå®å¨è¯¾è¡¨ï¼ä½¿ç¨åé¡»åå¯¼å¥è¯¾è¡¨ï¼è¿éçè¯¾è¡¨æ¯å¨çº¿è¯¾è¡¨
 2.
 å¯¼å¥è¯¾è¡¨ï¼éè¦æå°ç±è¯¾è¡¨åäº«åºæ¥çé¾æ¥ï¼æå¼å°ç±è¯¾ç¨è¡¨ï¼æå¨æ·»å è¯¾ç¨æä»æå¡å¯¼å¥
 (å·²ééäºå¤§é¨åé«æ ¡)è¯¾ç¨å ![Image text](https://github.com/maoxig/
 nonebot-plugin-ai-timetable/blob/main/resource/export.jpg)
 å¨åºæ¬è®¾ç½®éæå¼å§ä¸è¯¾æ¶é´ç­è°æ´å¥½ä¹å
 (å°¤å¶æ¯æ¶é´ãèæ°)ï¼æåäº«è¯¾è¡¨å¾å°çé¾æ¥åéç»botå³å¯å¯¼å¥æ¬å°
@@ -107,13 +109,16 @@
 -
 å¦æå¯¼å¥è¯¾è¡¨åå¨å°ç±è¯¾è¡¨åä¿®æ¹äºè¯¾ç¨ï¼ç´æ¥ç»botåéæ´æ°è¯¾è¡¨å³å¯æ´æ°æ¬å°è¯¾è¡¨
 -
 å½ä½ ä¸»é¡µçè¯¾è¡¨åå­¦æ ¡è¯¾è¡¨åºæ¬ä¸è´æ¶ï¼é£ä¹å°ç±è¯¾ç¨è¡¨å°±è¢«è°æå¥½äºï¼å¯ä»¥å¯¼å¥äº
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/
 resource/settings.jpg) ## ð¦è®¡å - [x] æ¥è¯¢ä¸èè¯¾çä¿¡æ¯ - [x]
 å¯éæ©æ¯å¦åéå¾çä»¥é¿åé£æ§ - [x] å¢å æ´å¤çéç½®é¡¹ - [x]
-éæä»£ç  - [x] è®¢éæå®çè¯¾ - [ ]
-ééæä»¶datastoreï¼æ¥å¥æ°æ®åº - [ ] å®åæä»¶ ##
+éæä»£ç  - [x] è®¢éæå®çè¯¾ - [x] å¤å¹³å°éé, åºäº [nonebot-
+plugin-alconna](https://github.com/nonebot/plugin-alconna) - [ ]
+æ¯æå®æ¶ä»»å¡æ¬å°å­å¨ - [ ] éé[plugin-rom](https://github.com/
+nonebot/plugin-orm), æ¥å¥æ°æ®åº - [ ]
+ééæ´å¤è¯¾è¡¨ãè±ç¦»å°ç±è¯¾è¡¨ - [ ] å®åæä»¶ ##
 ðå­å¨çé®é¢ 1.
 å°ç±è¯¾è¡¨åäº«çé¾æ¥å¤§æ¦2å¨åä¼è¿æï¼ä¼ä½¿å¾`æçè¯¾è¡¨\ä¸å¨è¯¾è¡¨`æ æ³ä½¿ç¨ï¼éè¦éæ°åäº«ï¼ä½æ¯ä»è½ä½¿ç¨æ¬å°è¯¾è¡¨ï¼ä¹å¯ä»¥æ´æ°æ¬å°è¯¾è¡¨
 2. æºå¨äººéå¯åå®æ¶ä»»å¡ä¼ä¸¢å¤± ##
 åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§QAQ
```

