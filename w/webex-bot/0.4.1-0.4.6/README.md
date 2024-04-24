# Comparing `tmp/webex_bot-0.4.1.tar.gz` & `tmp/webex_bot-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webex_bot-0.4.1.tar", last modified: Thu Sep  7 15:01:54 2023, max compression
+gzip compressed data, was "webex_bot-0.4.6.tar", last modified: Wed Apr 24 10:26:51 2024, max compression
```

## Comparing `webex_bot-0.4.1.tar` & `webex_bot-0.4.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 15:01:54.720028 webex_bot-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2023-09-07 15:01:17.000000 webex_bot-0.4.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-09-07 15:01:17.000000 webex_bot-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      221 2023-09-07 15:01:17.000000 webex_bot-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10628 2023-09-07 15:01:54.720028 webex_bot-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9974 2023-09-07 15:01:17.000000 webex_bot-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 15:01:54.720028 webex_bot-0.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2023-09-07 15:01:17.000000 webex_bot-0.4.1/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)     4800 2023-09-07 15:01:17.000000 webex_bot-0.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-09-07 15:01:17.000000 webex_bot-0.4.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-09-07 15:01:17.000000 webex_bot-0.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2023-09-07 15:01:17.000000 webex_bot-0.4.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      771 2023-09-07 15:01:17.000000 webex_bot-0.4.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-09-07 15:01:17.000000 webex_bot-0.4.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      451 2023-09-07 15:01:54.720028 webex_bot-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2023-09-07 15:01:17.000000 webex_bot-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 15:01:54.720028 webex_bot-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-09-07 15:01:17.000000 webex_bot-0.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2023-09-07 15:01:17.000000 webex_bot-0.4.1/tests/test_webex_bot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 15:01:54.720028 webex_bot-0.4.1/webex_bot/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-09-07 15:01:17.000000 webex_bot-0.4.1/webex_bot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 15:01:54.720028 webex_bot-0.4.1/webex_bot/cards/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 15:01:17.000000 webex_bot-0.4.1/webex_bot/cards/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 15:01:54.720028 webex_bot-0.4.1/webex_bot/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 15:01:17.000000 webex_bot-0.4.1/webex_bot/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2023-09-07 15:01:17.000000 webex_bot-0.4.1/webex_bot/commands/echo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2023-09-07 15:01:17.000000 webex_bot-0.4.1/webex_bot/commands/help.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2023-09-07 15:01:17.000000 webex_bot-0.4.1/webex_bot/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2023-09-07 15:01:17.000000 webex_bot-0.4.1/webex_bot/formatting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 15:01:54.720028 webex_bot-0.4.1/webex_bot/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 15:01:17.000000 webex_bot-0.4.1/webex_bot/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2023-09-07 15:01:17.000000 webex_bot-0.4.1/webex_bot/models/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2023-09-07 15:01:17.000000 webex_bot-0.4.1/webex_bot/models/response.py
--rw-r--r--   0 runner    (1001) docker     (127)    19410 2023-09-07 15:01:17.000000 webex_bot-0.4.1/webex_bot/webex_bot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 15:01:54.720028 webex_bot-0.4.1/webex_bot/websockets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-07 15:01:17.000000 webex_bot-0.4.1/webex_bot/websockets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7600 2023-09-07 15:01:17.000000 webex_bot-0.4.1/webex_bot/websockets/webex_websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 15:01:54.720028 webex_bot-0.4.1/webex_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10628 2023-09-07 15:01:54.000000 webex_bot-0.4.1/webex_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      790 2023-09-07 15:01:54.000000 webex_bot-0.4.1/webex_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-07 15:01:54.000000 webex_bot-0.4.1/webex_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-07 15:01:46.000000 webex_bot-0.4.1/webex_bot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-09-07 15:01:54.000000 webex_bot-0.4.1/webex_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-09-07 15:01:54.000000 webex_bot-0.4.1/webex_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:26:51.700759 webex_bot-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-24 10:26:12.000000 webex_bot-0.4.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-24 10:26:12.000000 webex_bot-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-24 10:26:12.000000 webex_bot-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-04-24 10:26:51.700759 webex_bot-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10235 2024-04-24 10:26:12.000000 webex_bot-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:26:51.696759 webex_bot-0.4.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-24 10:26:12.000000 webex_bot-0.4.6/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4800 2024-04-24 10:26:12.000000 webex_bot-0.4.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-24 10:26:12.000000 webex_bot-0.4.6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-24 10:26:12.000000 webex_bot-0.4.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-24 10:26:12.000000 webex_bot-0.4.6/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-24 10:26:12.000000 webex_bot-0.4.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 10:26:12.000000 webex_bot-0.4.6/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-24 10:26:51.700759 webex_bot-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-24 10:26:12.000000 webex_bot-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:26:51.696759 webex_bot-0.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-24 10:26:12.000000 webex_bot-0.4.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-24 10:26:12.000000 webex_bot-0.4.6/tests/test_webex_bot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:26:51.696759 webex_bot-0.4.6/webex_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-24 10:26:12.000000 webex_bot-0.4.6/webex_bot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:26:51.696759 webex_bot-0.4.6/webex_bot/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:26:12.000000 webex_bot-0.4.6/webex_bot/cards/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:26:51.696759 webex_bot-0.4.6/webex_bot/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:26:12.000000 webex_bot-0.4.6/webex_bot/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-24 10:26:12.000000 webex_bot-0.4.6/webex_bot/commands/echo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-24 10:26:12.000000 webex_bot-0.4.6/webex_bot/commands/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-24 10:26:12.000000 webex_bot-0.4.6/webex_bot/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-24 10:26:12.000000 webex_bot-0.4.6/webex_bot/formatting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:26:51.696759 webex_bot-0.4.6/webex_bot/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:26:12.000000 webex_bot-0.4.6/webex_bot/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-24 10:26:12.000000 webex_bot-0.4.6/webex_bot/models/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-24 10:26:12.000000 webex_bot-0.4.6/webex_bot/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20449 2024-04-24 10:26:12.000000 webex_bot-0.4.6/webex_bot/webex_bot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:26:51.700759 webex_bot-0.4.6/webex_bot/websockets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:26:12.000000 webex_bot-0.4.6/webex_bot/websockets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9427 2024-04-24 10:26:12.000000 webex_bot-0.4.6/webex_bot/websockets/webex_websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:26:51.696759 webex_bot-0.4.6/webex_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-04-24 10:26:51.000000 webex_bot-0.4.6/webex_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-24 10:26:51.000000 webex_bot-0.4.6/webex_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:26:51.000000 webex_bot-0.4.6/webex_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:26:43.000000 webex_bot-0.4.6/webex_bot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-24 10:26:51.000000 webex_bot-0.4.6/webex_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 10:26:51.000000 webex_bot-0.4.6/webex_bot.egg-info/top_level.txt
```

### Comparing `webex_bot-0.4.1/CONTRIBUTING.rst` & `webex_bot-0.4.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.1/LICENSE` & `webex_bot-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.1/PKG-INFO` & `webex_bot-0.4.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: webex_bot
-Version: 0.4.1
+Version: 0.4.6
 Summary: Python package for a Webex Bot based on websockets.
 Home-page: https://github.com/fbradyirl/webex_bot
 Author: Finbarr Brady
-Author-email: finbarr.brady@gmail.com
+Author-email: finbarr@somemail.com
 License: MIT license
 Keywords: webex_bot
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -343,14 +343,22 @@
 * Bot will reply in response to the original message via the thread ID. This is not always possible in the case of a
   card action response due to some server side issue.
 
 ### 0.4.1 (2023-Sept-07)
 
 * Always ensure there is a thread ID in the Activity before accessing it
 
+### 0.4.6 (2024-Apr-24)
+
+* Add max backoff time (#55)
+* Attached files. Help, threading and log level overrides. (#54)
+* add stop() call to gracefully exit the bot (#42)
+* feat(20231212): add help image size parameter (#46)
+* update websockets to 11.0.3 (#43)
+
 [1]: https://github.com/aaugustin/websockets
 
 [2]: https://github.com/CiscoDevNet/webexteamssdk
 
 [3]: https://developer.webex.com/docs/bots
 
 [4]: https://github.com/fbradyirl/webex_bot/blob/main/example.py
```

### Comparing `webex_bot-0.4.1/README.md` & `webex_bot-0.4.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -323,14 +323,22 @@
 * Bot will reply in response to the original message via the thread ID. This is not always possible in the case of a
   card action response due to some server side issue.
 
 ### 0.4.1 (2023-Sept-07)
 
 * Always ensure there is a thread ID in the Activity before accessing it
 
+### 0.4.6 (2024-Apr-24)
+
+* Add max backoff time (#55)
+* Attached files. Help, threading and log level overrides. (#54)
+* add stop() call to gracefully exit the bot (#42)
+* feat(20231212): add help image size parameter (#46)
+* update websockets to 11.0.3 (#43)
+
 [1]: https://github.com/aaugustin/websockets
 
 [2]: https://github.com/CiscoDevNet/webexteamssdk
 
 [3]: https://developer.webex.com/docs/bots
 
 [4]: https://github.com/fbradyirl/webex_bot/blob/main/example.py
```

### Comparing `webex_bot-0.4.1/docs/Makefile` & `webex_bot-0.4.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.1/docs/conf.py` & `webex_bot-0.4.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.1/docs/installation.rst` & `webex_bot-0.4.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.1/docs/make.bat` & `webex_bot-0.4.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.1/setup.py` & `webex_bot-0.4.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
-requirements = ['webexteamssdk==1.6.1', 'coloredlogs', 'websockets==10.2', 'backoff']
+requirements = ['webexteamssdk==1.6.1', 'coloredlogs', 'websockets==11.0.3', 'backoff']
 
 setup_requirements = ['pytest-runner', ]
 
 test_requirements = ['pytest>=3', ]
 
 setup(
     author="Finbarr Brady",
-    author_email='finbarr.brady@gmail.com',
+    author_email='finbarr@somemail.com',
     python_requires='>=3.8',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3.8',
@@ -34,10 +34,10 @@
     keywords='webex_bot',
     name='webex_bot',
     packages=find_packages(include=['webex_bot', 'webex_bot.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/fbradyirl/webex_bot',
-    version='0.4.1',
+    version='0.4.6',
     zip_safe=False,
 )
```

### Comparing `webex_bot-0.4.1/tests/test_webex_bot.py` & `webex_bot-0.4.6/tests/test_webex_bot.py`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.1/webex_bot/commands/echo.py` & `webex_bot-0.4.6/webex_bot/commands/echo.py`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.1/webex_bot/commands/help.py` & `webex_bot-0.4.6/webex_bot/commands/help.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 log = logging.getLogger(__name__)
 
 HELP_COMMAND_KEYWORD = "help"
 
 
 class HelpCommand(Command):
 
-    def __init__(self, bot_name, bot_help_subtitle, bot_help_image):
+    def __init__(self, bot_name, bot_help_subtitle, bot_help_image, bot_help_image_size=ImageSize.SMALL):
         self.commands = None
         super().__init__(
             command_keyword=HELP_COMMAND_KEYWORD,
             help_message="Get Help",
             card=None)
         self.card_callback = self.build_card
         self.card_populated = False
         self.bot_name = bot_name
         self.bot_help_subtitle = bot_help_subtitle
         self.bot_help_image = bot_help_image
+        self.bot_help_image_size = bot_help_image_size
 
     def execute(self, message, attachment_actions, activity):
         pass
 
     def build_card(self, message, attachment_actions, activity):
         """
         Construct a help message for users.
@@ -38,15 +39,15 @@
         :return:
         """
         heading = TextBlock(self.bot_name, weight=FontWeight.BOLDER, wrap=True, size=FontSize.LARGE)
         subtitle = TextBlock(self.bot_help_subtitle, wrap=True, size=FontSize.SMALL, color=Colors.LIGHT)
 
         image = Image(
             url=self.bot_help_image,
-            size=ImageSize.SMALL)
+            size=self.bot_help_image_size)
 
         header_column = Column(items=[heading, subtitle], width=2)
         header_image_column = Column(
             items=[image],
             width=1,
         )
```

### Comparing `webex_bot-0.4.1/webex_bot/exceptions.py` & `webex_bot-0.4.6/webex_bot/exceptions.py`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.1/webex_bot/models/command.py` & `webex_bot-0.4.6/webex_bot/models/command.py`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.1/webex_bot/models/response.py` & `webex_bot-0.4.6/webex_bot/models/response.py`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.1/webex_bot/webex_bot.py` & `webex_bot-0.4.6/webex_bot/webex_bot.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,77 +12,87 @@
 from webex_bot.exceptions import BotException
 from webex_bot.formatting import quote_info
 from webex_bot.models.command import CALLBACK_KEYWORD_KEY, Command, COMMAND_KEYWORD_KEY
 from webex_bot.models.response import Response
 from webex_bot.websockets.webex_websocket_client import WebexWebsocketClient, DEFAULT_DEVICE_URL
 
 log = logging.getLogger(__name__)
-coloredlogs.install(level=os.getenv("LOG_LEVEL", "INFO"),
-                    fmt='%(asctime)s  [%(levelname)s]  '
-                        '[%(module)s.%(name)s.%(funcName)'
-                        's]:%(lineno)s %(message)s')
 
 
 class WebexBot(WebexWebsocketClient):
 
     def __init__(self,
                  teams_bot_token,
                  approved_users=[],
                  approved_domains=[],
                  approved_rooms=[],
                  device_url=DEFAULT_DEVICE_URL,
                  include_demo_commands=False,
                  bot_name="Webex Bot",
-                 bot_help_subtitle="Here are my available commands. Click one to begin."):
+                 bot_help_subtitle="Here are my available commands. Click one to begin.",
+                 threads=True,
+                 help_command=None,
+                 log_level="INFO"):
         """
         Initialise WebexBot.
 
         @param teams_bot_token: Your token.
         @param approved_users: List of email address who are allowed to chat to this bot.
         @param approved_domains: List of domains which are allowed to chat to this bot.
         @param approved_rooms: List of rooms whose members are allowed to chat to this bot.
         @param device_url: WDM Url
         @param include_demo_commands: If True, any demo commands will be included.
         @param bot_name: Your custom name for the bot.
         @param bot_help_subtitle: Text to show in the help card.
+        @param threads: If True, respond to msg by creating a thread.
+        @param help_command: If None, use internal HelpCommand, otherwise override.
+        @param log_level: Set loggin level.
+
         """
 
+        coloredlogs.install(level=os.getenv("LOG_LEVEL", log_level),
+                            fmt='%(asctime)s  [%(levelname)s]  '
+                                '[%(module)s.%(name)s.%(funcName)'
+                                's]:%(lineno)s %(message)s')
         log.info("Registering bot with Webex cloud")
         WebexWebsocketClient.__init__(self,
                                       teams_bot_token,
                                       on_message=self.process_incoming_message,
                                       on_card_action=self.process_incoming_card_action,
                                       device_url=device_url)
 
         # A dictionary of commands this bot listens to
         # Each key in the dictionary is a command, with associated help
         # text and callback function
         # By default supports 2 command, echo and help
 
-        self.help_command = HelpCommand(
-            bot_name=bot_name,
-            bot_help_subtitle=bot_help_subtitle,
-            bot_help_image=self.teams.people.me().avatar)
+        if help_command is None:
+            self.help_command = HelpCommand(
+                bot_name=bot_name,
+                bot_help_subtitle=bot_help_subtitle,
+                bot_help_image=self.teams.people.me().avatar)
+            self.help_command.commands = self.commands
+            # Set default help message
+            self.help_message = "Hello!  I understand the following commands:  \n"
+        else:
+            self.help_command = help_command
         self.commands = {
             self.help_command
         }
         if include_demo_commands:
             self.add_command(EchoCommand())
 
-        self.help_command.commands = self.commands
-
         self.card_callback_commands = {}
         self.approved_users = approved_users
         self.approved_domains = approved_domains
         self.approved_rooms = approved_rooms
-        # Set default help message
-        self.help_message = "Hello!  I understand the following commands:  \n"
         self.approval_parameters_check()
         self.bot_display_name = ""
         self.get_me_info()
+        self.threads = threads
 
     @backoff.on_exception(backoff.expo, requests.exceptions.ConnectionError)
     def get_me_info(self):
         """
         Fetch me info from webexteamssdk
         """
         me = self.teams.people.me()
@@ -303,15 +313,15 @@
 
     def do_reply(self, reply, room_id, user_email, reply_one_to_one, is_one_on_one_space, conv_target_id):
         # allow command handlers to craft their own Teams message
         if reply and isinstance(reply, Response):
             # If the Response lacks a roomId, set it to the incoming room
             if not reply.roomId:
                 reply.roomId = room_id
-            if not reply.parentId and conv_target_id:
+            if not reply.parentId and conv_target_id and self.threads:
                 reply.parentId = conv_target_id
             reply = reply.as_dict()
             self.teams.messages.create(**reply)
             reply = "ok"
         # Support returning a list of Responses
         elif reply and isinstance(reply, list):
             for response in reply:
@@ -347,22 +357,33 @@
                                        is_one_on_one_space,
                                        reply,
                                        conv_target_id):
         default_move_to_one_to_one_heads_up = \
             quote_info(f"{user_email} I've messaged you 1-1. Please reply to me there.")
         if reply_one_to_one:
             if not is_one_on_one_space:
-                self.teams.messages.create(roomId=room_id,
-                                           markdown=default_move_to_one_to_one_heads_up,
+                if self.threads:
+                    self.teams.messages.create(roomId=room_id,
+                                               markdown=default_move_to_one_to_one_heads_up,
+                                               parentId=conv_target_id)
+                else:
+                    self.teams.messages.create(roomId=room_id,
+                                               markdown=default_move_to_one_to_one_heads_up)
+            if self.threads:
+                self.teams.messages.create(toPersonEmail=user_email,
+                                           markdown=reply,
                                            parentId=conv_target_id)
-            self.teams.messages.create(toPersonEmail=user_email,
-                                       markdown=reply,
-                                       parentId=conv_target_id)
+            else:
+                self.teams.messages.create(toPersonEmail=user_email,
+                                           markdown=reply)
         else:
-            self.teams.messages.create(roomId=room_id, markdown=reply, parentId=conv_target_id)
+            if self.threads:
+                self.teams.messages.create(roomId=room_id, markdown=reply, parentId=conv_target_id)
+            else:
+                self.teams.messages.create(roomId=room_id, markdown=reply)
 
     def run_pre_card_load_reply(self, command, message, teams_message, activity):
         """
         This allows a reply to be sent back before the command/card function is called. Useful if it takes a while for the card to generate.
         """
         try:
             return command.pre_card_load_reply(message, teams_message, activity), False
```

### Comparing `webex_bot-0.4.1/webex_bot/websockets/webex_websocket_client.py` & `webex_bot-0.4.6/webex_bot/websockets/webex_websocket_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,47 +24,76 @@
     "systemName": "python-spark-client",
     "systemVersion": "0.1"
 }
 
 ssl_context = ssl.create_default_context()
 ssl_context.load_verify_locations(certifi.where())
 
+MAX_BACKOFF_TIME = 240
+
 
 class WebexWebsocketClient(object):
     def __init__(self,
                  access_token,
                  device_url=DEFAULT_DEVICE_URL,
                  on_message=None,
                  on_card_action=None):
         self.access_token = access_token
         self.teams = WebexTeamsAPI(access_token=access_token)
         self.device_url = device_url
         self.device_info = None
         self.on_message = on_message
         self.on_card_action = on_card_action
         self.websocket = None
+        self.share_id = None
 
     def _process_incoming_websocket_message(self, msg):
         """
         Handle websocket data.
         :param msg: The raw websocket message
         """
+        logger.info(f"msg['data'] = {msg['data']}")
         if msg['data']['eventType'] == 'conversation.activity':
             activity = msg['data']['activity']
             if activity['verb'] == 'post':
                 logger.debug(f"activity={activity}")
 
                 message_base_64_id = self._get_base64_message_id(activity)
                 webex_message = self.teams.messages.get(message_base_64_id)
                 logger.debug(f"webex_message from message_base_64_id: {webex_message}")
                 if self.on_message:
                     # ack message first
                     self._ack_message(message_base_64_id)
                     # Now process it with the handler
                     self.on_message(teams_message=webex_message, activity=activity)
+            elif activity['verb'] == 'share':
+                logger.debug(f"activity={activity}")
+                self.share_id = activity['id']
+                return
+            elif activity['verb'] == 'update':
+                logger.debug(f"activity={activity}")
+
+                object = activity['object']
+                if object['objectType'] == 'content' and object['contentCategory'] == 'documents':
+                    if 'files' in object.keys():
+                        for item in object['files']['items']:
+                            if not item['malwareQuarantineState'] == 'safe':
+                                return
+                    else:
+                        return
+                else:
+                    return
+                message_base_64_id = self._get_base64_message_id(activity)
+                webex_message = self.teams.messages.get(message_base_64_id)
+                logger.debug(f"webex_message from message_base_64_id: {webex_message}")
+                if self.on_message:
+                    # ack message first
+                    self._ack_message(message_base_64_id)
+                    # Now process it with the handler
+                    self.on_message(teams_message=webex_message, activity=activity)
             elif activity['verb'] == 'cardAction':
                 logger.debug(f"activity={activity}")
 
                 message_base_64_id = self._get_base64_message_id(activity)
                 attachment_actions = self.teams.attachment_actions.get(message_base_64_id)
                 logger.info(f"attachment_actions from message_base_64_id: {attachment_actions}")
                 if self.on_card_action:
@@ -79,18 +108,22 @@
         """
         In order to geo-locate the correct DC to fetch the message from, you need to use the base64 Id of the
         message.
         @param activity: incoming websocket data
         @return: base 64 message id
         """
         activity_id = activity['id']
-        logger.debug(f"activity verb=post. message id={activity_id}")
+        logger.debug(f"activity verb={activity['verb']}. message id={activity_id}")
         conversation_url = activity['target']['url']
         conv_target_id = activity['target']['id']
-        verb = "messages" if activity['verb'] == "post" else "attachment/actions"
+        verb = "messages" if activity['verb'] in ["post", "update"] else "attachment/actions"
+        if activity['verb'] == "update" and self.share_id is not None:
+            activity_id = self.share_id
+            self.share_id = None
+        logger.debug(f"activity_id={activity_id}")
         conversation_message_url = conversation_url.replace(f"conversations/{conv_target_id}",
                                                             f"{verb}/{activity_id}")
         headers = {"Authorization": f"Bearer {self.access_token}"}
         conversation_message = requests.get(conversation_message_url,
                                             headers=headers).json()
         logger.debug(f"conversation_message={conversation_message}")
         return conversation_message['id']
@@ -130,14 +163,20 @@
         resp = self.teams._session.post(f"{self.device_url}/devices", json=DEVICE_DATA)
         if resp is None:
             raise Exception("could not create WDM device")
         self.device_info = resp
         logger.debug(f"self.device_info: {self.device_info}")
         return resp
 
+    def stop(self):
+        def terminate():
+            raise SystemExit()
+
+        asyncio.get_event_loop().create_task(terminate())
+
     def run(self):
         if self.device_info is None:
             if self._get_device_info() is None:
                 logger.error('could not get/create device info')
                 raise Exception("No WDM device info")
 
         async def _websocket_recv():
@@ -147,18 +186,18 @@
                 msg = json.loads(message)
                 loop = asyncio.get_event_loop()
                 loop.run_in_executor(None, self._process_incoming_websocket_message, msg)
             except Exception as messageProcessingException:
                 logger.warning(
                     f"An exception occurred while processing message. Ignoring. {messageProcessingException}")
 
-        @backoff.on_exception(backoff.expo, websockets.ConnectionClosedError)
-        @backoff.on_exception(backoff.expo, websockets.ConnectionClosedOK)
-        @backoff.on_exception(backoff.expo, websockets.ConnectionClosed)
-        @backoff.on_exception(backoff.expo, socket.gaierror)
+        @backoff.on_exception(backoff.expo, websockets.ConnectionClosedError, max_time=MAX_BACKOFF_TIME)
+        @backoff.on_exception(backoff.expo, websockets.ConnectionClosedOK, max_time=MAX_BACKOFF_TIME)
+        @backoff.on_exception(backoff.expo, websockets.ConnectionClosed, max_time=MAX_BACKOFF_TIME)
+        @backoff.on_exception(backoff.expo, socket.gaierror, max_time=MAX_BACKOFF_TIME)
         async def _connect_and_listen():
             ws_url = self.device_info['webSocketUrl']
             logger.info(f"Opening websocket connection to {ws_url}")
             async with websockets.connect(ws_url, ssl=ssl_context) as _websocket:
                 self.websocket = _websocket
                 logger.info("WebSocket Opened.")
                 msg = {'id': str(uuid.uuid4()),
```

### Comparing `webex_bot-0.4.1/webex_bot.egg-info/PKG-INFO` & `webex_bot-0.4.6/webex_bot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: webex-bot
-Version: 0.4.1
+Version: 0.4.6
 Summary: Python package for a Webex Bot based on websockets.
 Home-page: https://github.com/fbradyirl/webex_bot
 Author: Finbarr Brady
-Author-email: finbarr.brady@gmail.com
+Author-email: finbarr@somemail.com
 License: MIT license
 Keywords: webex_bot
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -343,14 +343,22 @@
 * Bot will reply in response to the original message via the thread ID. This is not always possible in the case of a
   card action response due to some server side issue.
 
 ### 0.4.1 (2023-Sept-07)
 
 * Always ensure there is a thread ID in the Activity before accessing it
 
+### 0.4.6 (2024-Apr-24)
+
+* Add max backoff time (#55)
+* Attached files. Help, threading and log level overrides. (#54)
+* add stop() call to gracefully exit the bot (#42)
+* feat(20231212): add help image size parameter (#46)
+* update websockets to 11.0.3 (#43)
+
 [1]: https://github.com/aaugustin/websockets
 
 [2]: https://github.com/CiscoDevNet/webexteamssdk
 
 [3]: https://developer.webex.com/docs/bots
 
 [4]: https://github.com/fbradyirl/webex_bot/blob/main/example.py
```

### Comparing `webex_bot-0.4.1/webex_bot.egg-info/SOURCES.txt` & `webex_bot-0.4.6/webex_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

