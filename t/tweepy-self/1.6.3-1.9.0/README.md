# Comparing `tmp/tweepy_self-1.6.3.tar.gz` & `tmp/tweepy_self-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweepy_self-1.6.3.tar", max compression
+gzip compressed data, was "tweepy_self-1.9.0.tar", max compression
```

## Comparing `tweepy_self-1.6.3.tar` & `tweepy_self-1.9.0.tar`

### file list

```diff
@@ -1,16 +1,23 @@
--rw-r--r--   0        0        0      647 2024-02-24 16:24:00.303183 tweepy_self-1.6.3/pyproject.toml
--rw-r--r--   0        0        0     8739 2024-02-24 09:08:27.795266 tweepy_self-1.6.3/README.md
--rw-r--r--   0        0        0      684 2024-02-20 13:47:29.647489 tweepy_self-1.6.3/twitter/__init__.py
--rw-r--r--   0        0        0     3015 2024-02-22 19:16:31.988794 tweepy_self-1.6.3/twitter/account.py
--rw-r--r--   0        0        0      133 2024-02-04 14:35:51.694463 tweepy_self-1.6.3/twitter/base/__init__.py
--rw-r--r--   0        0        0      478 2024-02-04 14:15:27.321006 tweepy_self-1.6.3/twitter/base/client.py
--rw-r--r--   0        0        0     2071 2024-02-15 12:06:46.926661 tweepy_self-1.6.3/twitter/base/session.py
--rw-r--r--   0        0        0    61346 2024-02-23 17:11:32.024777 tweepy_self-1.6.3/twitter/client.py
--rw-r--r--   0        0        0      270 2024-02-22 12:04:06.121519 tweepy_self-1.6.3/twitter/enums.py
--rw-r--r--   0        0        0     5007 2024-02-23 14:58:59.148174 tweepy_self-1.6.3/twitter/errors.py
--rw-r--r--   0        0        0     2063 2024-02-23 15:12:48.234927 tweepy_self-1.6.3/twitter/models.py
--rw-r--r--   0        0        0      589 2024-02-04 16:45:50.789563 tweepy_self-1.6.3/twitter/utils/__init__.py
--rw-r--r--   0        0        0     1120 2024-02-15 12:06:46.929662 tweepy_self-1.6.3/twitter/utils/file.py
--rw-r--r--   0        0        0     1971 2024-02-15 12:06:46.931665 tweepy_self-1.6.3/twitter/utils/html.py
--rw-r--r--   0        0        0      559 2024-02-15 12:06:46.923663 tweepy_self-1.6.3/twitter/utils/other.py
--rw-r--r--   0        0        0     9304 1970-01-01 00:00:00.000000 tweepy_self-1.6.3/PKG-INFO
+-rw-r--r--   0        0        0      762 2024-03-14 19:33:04.726776 tweepy_self-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8720 2024-03-14 19:33:04.726271 tweepy_self-1.9.0/README.md
+-rw-r--r--   0        0        0      732 2024-03-14 19:33:04.726776 tweepy_self-1.9.0/twitter/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 19:33:04.727782 tweepy_self-1.9.0/twitter/_capsolver/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 19:33:04.727782 tweepy_self-1.9.0/twitter/_capsolver/core/__init__.py
+-rw-r--r--   0        0        0     8883 2024-03-14 19:33:04.727782 tweepy_self-1.9.0/twitter/_capsolver/core/base.py
+-rw-r--r--   0        0        0     1054 2024-03-14 19:33:04.727782 tweepy_self-1.9.0/twitter/_capsolver/core/config.py
+-rw-r--r--   0        0        0     1741 2024-03-14 19:33:04.727782 tweepy_self-1.9.0/twitter/_capsolver/core/enum.py
+-rw-r--r--   0        0        0     2616 2024-03-14 19:33:04.728781 tweepy_self-1.9.0/twitter/_capsolver/core/serializer.py
+-rw-r--r--   0        0        0    10974 2024-03-14 19:33:04.728781 tweepy_self-1.9.0/twitter/_capsolver/fun_captcha.py
+-rw-r--r--   0        0        0     3142 2024-03-14 19:33:04.728781 tweepy_self-1.9.0/twitter/account.py
+-rw-r--r--   0        0        0      141 2024-03-14 19:33:04.728781 tweepy_self-1.9.0/twitter/base/__init__.py
+-rw-r--r--   0        0        0      482 2024-03-14 19:33:04.729780 tweepy_self-1.9.0/twitter/base/client.py
+-rw-r--r--   0        0        0     2071 2024-02-15 12:06:46.926661 tweepy_self-1.9.0/twitter/base/session.py
+-rw-r--r--   0        0        0    64199 2024-03-14 19:33:04.729780 tweepy_self-1.9.0/twitter/client.py
+-rw-r--r--   0        0        0      270 2024-02-22 12:04:06.121519 tweepy_self-1.9.0/twitter/enums.py
+-rw-r--r--   0        0        0     5088 2024-03-14 19:33:04.730781 tweepy_self-1.9.0/twitter/errors.py
+-rw-r--r--   0        0        0     4985 2024-03-14 19:33:04.730781 tweepy_self-1.9.0/twitter/models.py
+-rw-r--r--   0        0        0      663 2024-03-14 19:33:04.730781 tweepy_self-1.9.0/twitter/utils/__init__.py
+-rw-r--r--   0        0        0     1120 2024-02-15 12:06:46.929662 tweepy_self-1.9.0/twitter/utils/file.py
+-rw-r--r--   0        0        0     1971 2024-02-15 12:06:46.931665 tweepy_self-1.9.0/twitter/utils/html.py
+-rw-r--r--   0        0        0     1061 2024-03-14 19:33:04.730781 tweepy_self-1.9.0/twitter/utils/other.py
+-rw-r--r--   0        0        0     9437 1970-01-01 00:00:00.000000 tweepy_self-1.9.0/PKG-INFO
```

### Comparing `tweepy_self-1.6.3/pyproject.toml` & `tweepy_self-1.9.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 [tool.poetry]
 name = "tweepy-self"
-version = "1.6.3"
+version = "1.9.0"
 description = "Twitter (selfbot) for Python!"
 authors = ["Alen <alen.kimov@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/alenkimov/tweepy-self"
 packages = [{include = "twitter"}]
 
+[tool.poetry.urls]
+Source = "https://github.com/alenkimov/tweepy-self"
+
 [tool.poetry.dependencies]
 python = "^3.11"
 curl_cffi = {version = "0.6.0b9", allow-prereleases = true}
-python3-capsolver = "^0.9"
-better-proxy = "1.1.1"
+better-proxy = "^1.1"
 beautifulsoup4 = "^4"
 pydantic = ">=1"
 lxml = "^5"
 pyotp = "^2"
 yarl = "^1"
+aiohttp = "^3.9"
+tenacity = "^8"
+requests = "^2"
+loguru = "^0.7"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tweepy_self-1.6.3/README.md` & `tweepy_self-1.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -73,35 +73,37 @@
 Не каждое взаимодействие с Twitter достоверно определяет статус аккаунта.
 Например, простой запрос данных об аккаунте честно вернет данные, даже если ваш аккаунт заморожен.
 
 Для достоверной установки статуса аккаунта используйте метод `establish_status()`
 
 ### Примеры работы
 Запрос информации о пользователе:
+
 ```python
 # Запрос информации о текущем пользователе:
-me = await twitter_client.request_user_data()
+me = await twitter_client.request_user()
 print(f"[{account.short_auth_token}] {me}")
 print(f"Аккаунт создан: {me.created_at}")
 print(f"Following (подписан ты): {me.followings_count}")
 print(f"Followers (подписаны на тебя): {me.followers_count}")
 print(f"Прочая информация: {me.raw_data}")
 
 # Запрос информации об ином пользователе:
-elonmusk = await twitter.request_user_data("@elonmusk")
+elonmusk = await twitter.request_user("@elonmusk")
 print(elonmusk)
 ```
 
 Смена имени пользователя и пароля:
+
 ```python
 account = twitter.Account("auth_token", password="password")
 ...
 await twitter_client.change_username("new_username")
-await twitter_client.request_user_data()
-print(f"New username: {account.data.username}")
+await twitter_client.request_user()
+print(f"New username: {account.username}")
 
 await twitter_client.change_password("new_password")
 print(f"New password: {account.password}")
 print(f"New auth_token: {account.auth_token}")
 ```
 
 Смена данных профиля:
@@ -139,16 +141,17 @@
 
 bind_code = await twitter_client.oauth_2(**bind_data)
 # Передайте код авторизации (привязки) сервису.
 # Сервис также может потребовать state, если он динамический.
 ```
 
 Отправка сообщения:
+
 ```python
-bro = await twitter_client.request_user_data("@username")
+bro = await twitter_client.request_user("@username")
 await twitter_client.send_message(bro.id, "I love you!")
 ```
 
 Запрос входящих сообщений:
 ```python
 messages = await twitter_client.request_messages()
 for message in messages:
```

### Comparing `tweepy_self-1.6.3/twitter/__init__.py` & `tweepy_self-1.9.0/twitter/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,29 +2,39 @@
 Twitter API Wrapper
 ~~~~~~~~~~~~~~~~~~~
 
 A basic wrapper for the Twitter user API.
 """
 
 from .client import Client
-from .account import Account, AccountStatus, load_accounts_from_file, extract_accounts_to_file
-from .models import Tweet, UserData
+from .account import (
+    Account,
+    AccountStatus,
+    load_accounts_from_file,
+    extract_accounts_to_file,
+)
+from .models import Tweet, User, Media, Image
 from . import errors, utils
 
 __all__ = [
     "Client",
     "Account",
     "AccountStatus",
+    "Tweet",
+    "User",
+    "Media",
+    "Image",
     "utils",
     "errors",
     "load_accounts_from_file",
     "extract_accounts_to_file",
 ]
 
 
 import warnings
+
 # HACK: Ignore event loop warnings from curl_cffi
-warnings.filterwarnings('ignore', module='curl_cffi')
+warnings.filterwarnings("ignore", module="curl_cffi")
 
+from loguru import logger
 
-from python3_capsolver.core import config
-config.APP_ID = "6F895B2F-F454-44D1-8FE0-77ACAD3DBDC8"
+logger.disable("twitter")
```

### Comparing `tweepy_self-1.6.3/twitter/account.py` & `tweepy_self-1.9.0/twitter/account.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from pathlib import Path
 from typing import Sequence, Iterable
 
-from pydantic import BaseModel, Field
+from pydantic import Field
 import pyotp
 
 from .utils import hidden_value, load_lines, write_lines
 from .enums import AccountStatus
+from .models import User
 
 
-class Account(BaseModel):
+class Account(User):
     # fmt: off
     auth_token:  str | None = Field(default=None, pattern=r"^[a-f0-9]{40}$")
     ct0:         str | None = None
-    id:          int | None = None
-    name:        str | None = None
-    username:    str | None = None
     password:    str | None = None
     email:       str | None = None
     totp_secret: str | None = None
     backup_code: str | None = None
     status: AccountStatus = AccountStatus.UNKNOWN
     # fmt: on
 
@@ -34,20 +32,26 @@
     def hidden_totp_secret(self) -> str | None:
         return hidden_value(self.totp_secret) if self.totp_secret else None
 
     @property
     def hidden_backup_code(self) -> str | None:
         return hidden_value(self.backup_code) if self.backup_code else None
 
-    def __repr__(self):
-        return f"{self.__class__.__name__}(auth_token={self.hidden_auth_token}, username={self.username})"
-
     def __str__(self):
         return self.hidden_auth_token
 
+    def __repr__(self):
+        return f"{self.__class__.__name__}(id={self.id}, username={self.username}, auth_token={self.hidden_auth_token})"
+
+    def update(self, **data: dict):
+        update = self.dict()
+        update.update(data)
+        for k, v in self.validate(update).dict(exclude_defaults=True).items():
+            setattr(self, k, v)
+
     def get_totp_code(self) -> str | None:
         if not self.totp_secret:
             raise ValueError("No key2fa")
 
         return str(pyotp.TOTP(self.totp_secret).now())
```

### Comparing `tweepy_self-1.6.3/twitter/base/session.py` & `tweepy_self-1.9.0/twitter/base/session.py`

 * *Files identical despite different names*

### Comparing `tweepy_self-1.6.3/twitter/client.py` & `tweepy_self-1.9.0/twitter/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from typing import Any, Literal
+from typing import Any, Literal, Iterable
 from time import time
 import asyncio
 import base64
 import re
 
+from loguru import logger
 from curl_cffi import requests
 from yarl import URL
 
-from python3_capsolver.fun_captcha import FunCaptcha, FunCaptchaTypeEnm
+from ._capsolver.fun_captcha import FunCaptcha, FunCaptchaTypeEnm
 
 from .errors import (
     TwitterException,
     FailedToFindDuplicatePost,
     HTTPException,
     BadRequest,
     Unauthorized,
@@ -21,23 +22,28 @@
     ServerError,
     BadAccount,
     BadToken,
     Locked,
     ConsentLocked,
     Suspended,
 )
-from .utils import to_json, tweet_url as create_tweet_url
-from .base import BaseClient
+from .utils import to_json
+from .base import BaseHTTPClient
 from .account import Account, AccountStatus
-from .models import UserData, Tweet
-from .utils import remove_at_sign, parse_oauth_html, parse_unlock_html
+from .models import User, Tweet, Media
+from .utils import (
+    remove_at_sign,
+    parse_oauth_html,
+    parse_unlock_html,
+    tweets_data_from_instructions,
+)
 
 
-class Client(BaseClient):
-    _BEARER_TOKEN = "Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA"
+class Client(BaseHTTPClient):
+    _BEARER_TOKEN = "AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA"
     _DEFAULT_HEADERS = {
         "authority": "twitter.com",
         "origin": "https://twitter.com",
         "x-twitter-active-user": "yes",
         # 'x-twitter-auth-type': 'OAuth2Session',
         "x-twitter-client-language": "en",
     }
@@ -52,14 +58,15 @@
         "DeleteTweet": "VaenaVgh5q5ih7kvyVjgtg",
         "UserTweets": "V1ze5q3ijDS1VeLwLY0m7g",
         "TweetDetail": "VWFGPVAGkZMGRKGe3GFFnA",
         "ProfileSpotlightsQuery": "9zwVLJ48lmVUk8u_Gh9DmA",
         "Following": "t-BPOrMIduGUJWO_LxcvNQ",
         "Followers": "3yX7xr2hKjcZYnXt6cU6lQ",
         "UserByScreenName": "G3KGOASz96M-Qu0nwmGXNg",
+        "UsersByRestIds": "itEhGywpgX9b3GJCzOtSrA",
         "Viewer": "W62NnYgkgziw9bwyoVht0g",
     }
     _CAPTCHA_URL = "https://twitter.com/account/access"
     _CAPTCHA_SITE_KEY = "0152B4EB-D2DC-460A-89A1-629838B529C9"
 
     @classmethod
     def _action_to_url(cls, action: str) -> tuple[str, str]:
@@ -72,15 +79,15 @@
 
     def __init__(
         self,
         account: Account,
         *,
         wait_on_rate_limit: bool = True,
         capsolver_api_key: str = None,
-        max_unlock_attempts: int = 4,
+        max_unlock_attempts: int = 5,
         **session_kwargs,
     ):
         super().__init__(**session_kwargs)
         self.account = account
         self.wait_on_rate_limit = wait_on_rate_limit
         self.capsolver_api_key = capsolver_api_key
         self.max_unlock_attempts = max_unlock_attempts
@@ -93,37 +100,51 @@
         bearer: bool = True,
         **kwargs,
     ) -> tuple[requests.Response, Any]:
         cookies = kwargs["cookies"] = kwargs.get("cookies") or {}
         headers = kwargs["headers"] = kwargs.get("headers") or {}
 
         if bearer:
-            headers["authorization"] = self._BEARER_TOKEN
+            headers["authorization"] = f"Bearer {self._BEARER_TOKEN}"
 
         if auth:
             if not self.account.auth_token:
                 raise ValueError("No auth_token. Login before")
 
             cookies["auth_token"] = self.account.auth_token
             if self.account.ct0:
                 cookies["ct0"] = self.account.ct0
                 headers["x-csrf-token"] = self.account.ct0
 
+        # fmt: off
+        log_message = f"{self.account} Request {method} {url}"
+        if kwargs.get('data'): log_message += f"\nRequest data: {kwargs.get('data')}"
+        if kwargs.get('json'): log_message += f"\nRequest data: {kwargs.get('json')}"
+        logger.debug(log_message)
+        # fmt: on
+
         try:
             response = await self._session.request(method, url, **kwargs)
         except requests.errors.RequestsError as exc:
             if exc.code == 35:
                 msg = (
                     "The IP address may have been blocked by Twitter. Blocked countries: Russia. "
                     + str(exc)
                 )
                 raise requests.errors.RequestsError(msg, 35, exc.response)
             raise
 
         data = response.text
+        # fmt: off
+        log_message = (f"{self.account} Response {method} {url}"
+                       f"\nStatus code: {response.status_code}"
+                       f"\nResponse data: {data}")
+        logger.debug(log_message)
+        # fmt: on
+
         if response.headers["content-type"].startswith("application/json"):
             data = response.json()
 
         if response.status_code == 429:
             if self.wait_on_rate_limit:
                 reset_time = int(response.headers["x-rate-limit-reset"])
                 sleep_time = reset_time - int(time()) + 1
@@ -331,20 +352,20 @@
             )
             authenticity_token, redirect_url, redirect_after_login_url = (
                 parse_oauth_html(response.text)
             )
 
         return authenticity_token, redirect_url
 
-    async def request_username(self):
+    async def request_and_set_username(self):
         url = "https://twitter.com/i/api/1.1/account/settings.json"
         response, response_json = await self.request("POST", url)
         self.account.username = response_json["screen_name"]
 
-    async def _request_user_data(self, username: str) -> UserData:
+    async def _request_user(self, username: str) -> User:
         url, query_id = self._action_to_url("UserByScreenName")
         username = remove_at_sign(username)
         variables = {
             "screen_name": username,
             "withSafetyModeUserFields": True,
         }
         features = {
@@ -363,56 +384,64 @@
             "withAuxiliaryUserLabels": False,
         }
         params = {
             "variables": to_json(variables),
             "features": to_json(features),
             "fieldToggles": to_json(field_toggles),
         }
-        response, response_json = await self.request("GET", url, params=params)
-        user_data = UserData.from_raw_user_data(response_json["data"]["user"]["result"])
-
-        if self.account.username == user_data.username:
-            self.account.id = user_data.id
-            self.account.name = user_data.name
+        response, data = await self.request("GET", url, params=params)
+        return User.from_raw_data(data["data"]["user"]["result"])
 
-        return user_data
+    async def request_user(
+        self, *, username: str = None, user_id: int | str = None
+    ) -> User | Account:
+        if username and user_id:
+            raise ValueError("Specify username or user_id, not both.")
 
-    async def request_user_data(self, username: str = None) -> UserData:
-        if username:
-            return await self._request_user_data(username)
+        if user_id:
+            users = await self.request_users((user_id,))
+            user = users[user_id]
         else:
-            if not self.account.username:
-                await self.request_username()
-            return await self._request_user_data(self.account.username)
+            if not username:
+                if not self.account.username:
+                    await self.request_and_set_username()
+                username = self.account.username
+
+            user = await self._request_user(username)
+
+        if self.account.username == user.username:
+            self.account.update(**user.model_dump())
+            user = self.account
+
+        return user
 
     async def upload_image(
         self,
         image: bytes,
         attempts: int = 3,
         timeout: float | tuple[float, float] = 10,
-    ) -> int:
+    ) -> Media:
         """
         Upload image as bytes.
 
         Иногда при первой попытке загрузки изображения возвращает 408,
         после чего повторная попытка загрузки изображения проходит успешно
 
-        :return: Media ID
+        :return: Media
         """
         url = "https://upload.twitter.com/1.1/media/upload.json"
 
-        data = {"media_data": base64.b64encode(image)}
+        payload = {"media_data": base64.b64encode(image)}
 
         for attempt in range(attempts):
             try:
-                response, response_json = await self.request(
-                    "POST", url, data=data, timeout=timeout
+                response, data = await self.request(
+                    "POST", url, data=payload, timeout=timeout
                 )
-                media_id = response_json["media_id"]
-                return media_id
+                return Media.from_raw_data(data)
             except (HTTPException, requests.errors.RequestsError) as exc:
                 if (
                     attempt < attempts - 1
                     and (
                         isinstance(exc, requests.errors.RequestsError)
                         and exc.code == 28
                     )
@@ -421,17 +450,14 @@
                         and exc.response.status_code == 408
                     )
                 ):
                     continue
                 else:
                     raise
 
-        media_id = response_json["media_id"]
-        return media_id
-
     async def _follow_action(self, action: str, user_id: int | str) -> bool:
         url = f"https://twitter.com/i/api/1.1/friendships/{action}.json"
         params = {
             "include_profile_interstitial_type": "1",
             "include_blocking": "1",
             "include_blocked_by": "1",
             "include_followed_by": "1",
@@ -462,30 +488,68 @@
 
     async def _interact_with_tweet(self, action: str, tweet_id: int) -> dict:
         url, query_id = self._action_to_url(action)
         json_payload = {
             "variables": {"tweet_id": tweet_id, "dark_request": False},
             "queryId": query_id,
         }
-        response, response_json = await self.request("POST", url, json=json_payload)
-        return response_json
+        response, data = await self.request("POST", url, json=json_payload)
+        return data
+
+    async def _repost(self, tweet_id: int | str) -> Tweet:
+        data = await self._interact_with_tweet("CreateRetweet", tweet_id)
+        tweet_id = data["data"]["create_retweet"]["retweet_results"]["result"]["rest_id"]  # type: ignore
+        return await self.request_tweet(tweet_id)
+
+    async def _repost_or_search_duplicate(
+        self,
+        tweet_id: int,
+        *,
+        search_duplicate: bool = True,
+    ) -> Tweet:
+        try:
+            tweet = await self._repost(tweet_id)
+        except HTTPException as exc:
+            if (
+                search_duplicate
+                and 327
+                in exc.api_codes  # duplicate retweet (You have already retweeted this Tweet)
+            ):
+                tweets = await self.request_tweets(self.account.id)
+                duplicate_tweet = None
+                for tweet_ in tweets:  # type: Tweet
+                    if tweet_.retweeted_tweet and tweet_.retweeted_tweet.id == tweet_id:
+                        duplicate_tweet = tweet_
+
+                if not duplicate_tweet:
+                    raise FailedToFindDuplicatePost(
+                        f"Couldn't find a post duplicate in the next 20 posts"
+                    )
+
+                tweet = duplicate_tweet
+
+            else:
+                raise
+
+        return tweet
 
-    async def repost(self, tweet_id: int) -> int:
+    async def repost(
+        self,
+        tweet_id: int,
+        *,
+        search_duplicate: bool = True,
+    ) -> Tweet:
         """
         Repost (retweet)
 
-        :return: Tweet ID
+        :return: Tweet
         """
-        response_json = await self._interact_with_tweet("CreateRetweet", tweet_id)
-        retweet_id = int(
-            response_json["data"]["create_retweet"]["retweet_results"]["result"][
-                "rest_id"
-            ]
+        return await self._repost_or_search_duplicate(
+            tweet_id, search_duplicate=search_duplicate
         )
-        return retweet_id
 
     async def like(self, tweet_id: int) -> bool:
         response_json = await self._interact_with_tweet("FavoriteTweet", tweet_id)
         is_liked = response_json["data"]["favorite_tweet"] == "Done"
         return is_liked
 
     async def unlike(self, tweet_id: int) -> dict:
@@ -584,97 +648,85 @@
         self,
         text: str = None,
         *,
         media_id: int | str = None,
         tweet_id_to_reply: str | int = None,
         attachment_url: str = None,
         search_duplicate: bool = True,
-        with_tweet_url: bool = True,
     ) -> Tweet:
         try:
             tweet = await self._tweet(
                 text,
                 media_id=media_id,
                 tweet_id_to_reply=tweet_id_to_reply,
                 attachment_url=attachment_url,
             )
         except HTTPException as exc:
             if (
                 search_duplicate
                 and 187 in exc.api_codes  # duplicate tweet (Status is a duplicate)
             ):
-                tweets = await self.request_tweets(self.account.id)
+                tweets = await self.request_tweets()
                 duplicate_tweet = None
                 for tweet_ in tweets:
-                    if tweet_.full_text.startswith(text.strip()):
+                    if tweet_.text.startswith(text.strip()):
                         duplicate_tweet = tweet_
 
                 if not duplicate_tweet:
                     raise FailedToFindDuplicatePost(
                         f"Couldn't find a post duplicate in the next 20 posts"
                     )
                 tweet = duplicate_tweet
 
             else:
                 raise
 
-        if with_tweet_url:
-            if not self.account.username:
-                await self.request_user_data()
-            tweet.url = create_tweet_url(self.account.username, tweet.id)
-
         return tweet
 
     async def tweet(
         self,
         text: str,
         *,
         media_id: int | str = None,
         search_duplicate: bool = True,
-        with_tweet_url: bool = True,
     ) -> Tweet:
         return await self._tweet_or_search_duplicate(
             text,
             media_id=media_id,
             search_duplicate=search_duplicate,
-            with_tweet_url=with_tweet_url,
         )
 
     async def reply(
         self,
         tweet_id: str | int,
         text: str,
         *,
         media_id: int | str = None,
         search_duplicate: bool = True,
-        with_tweet_url: bool = True,
     ) -> Tweet:
         return await self._tweet_or_search_duplicate(
             text,
             media_id=media_id,
             tweet_id_to_reply=tweet_id,
             search_duplicate=search_duplicate,
-            with_tweet_url=with_tweet_url,
         )
 
     async def quote(
         self,
         tweet_url: str,
         text: str,
         *,
         media_id: int | str = None,
         search_duplicate: bool = True,
-        with_tweet_url: bool = True,
     ) -> Tweet:
         return await self._tweet_or_search_duplicate(
             text,
             media_id=media_id,
             attachment_url=tweet_url,
             search_duplicate=search_duplicate,
-            with_tweet_url=with_tweet_url,
         )
 
     async def vote(
         self, tweet_id: int | str, card_id: int | str, choice_number: int
     ) -> dict:
         """
         :return: Raw vote information
@@ -688,15 +740,15 @@
             "twitter:string:selected_choice": str(choice_number),
         }
         response, response_json = await self.request("POST", url, params=params)
         return response_json
 
     async def _request_users(
         self, action: str, user_id: int | str, count: int
-    ) -> list[UserData]:
+    ) -> list[User]:
         url, query_id = self._action_to_url(action)
         variables = {
             "userId": str(user_id),
             "count": count,
             "includePromotedContent": False,
         }
         features = {
@@ -733,48 +785,68 @@
                 "instructions"
             ][-1]["entries"]
             for entry in entries:
                 if entry["entryId"].startswith("user"):
                     user_data_dict = entry["content"]["itemContent"]["user_results"][
                         "result"
                     ]
-                    users.append(UserData.from_raw_user_data(user_data_dict))
+                    users.append(User.from_raw_data(user_data_dict))
         return users
 
     async def request_followers(
         self, user_id: int | str = None, count: int = 10
-    ) -> list[UserData]:
+    ) -> list[User]:
         """
         :param user_id: Текущий пользователь, если не передан ID иного пользователя.
         :param count: Количество подписчиков.
         """
         if user_id:
             return await self._request_users("Followers", user_id, count)
         else:
             if not self.account.id:
-                await self.request_user_data()
+                await self.request_user()
             return await self._request_users("Followers", self.account.id, count)
 
     async def request_followings(
         self, user_id: int | str = None, count: int = 10
-    ) -> list[UserData]:
+    ) -> list[User]:
         """
         :param user_id: Текущий пользователь, если не передан ID иного пользователя.
         :param count: Количество подписчиков.
         """
         if user_id:
             return await self._request_users("Following", user_id, count)
         else:
             if not self.account.id:
-                await self.request_user_data()
+                await self.request_user()
             return await self._request_users("Following", self.account.id, count)
 
-    async def _request_tweet_data(self, tweet_id: int) -> dict:
-        action = "TweetDetail"
-        url, query_id = self._action_to_url(action)
+    async def request_users(
+        self, user_ids: Iterable[str | int]
+    ) -> dict[int : User | Account]:
+        url, query_id = self._action_to_url("UsersByRestIds")
+        variables = {"userIds": list({str(user_id) for user_id in user_ids})}
+        features = {
+            "responsive_web_graphql_exclude_directive_enabled": True,
+            "responsive_web_graphql_skip_user_profile_image_extensions_enabled": False,
+            "responsive_web_graphql_timeline_navigation_enabled": True,
+            "verified_phone_label_enabled": False,
+        }
+        query = {"variables": variables, "features": features}
+        response, data = await self.request("GET", url, params=query)
+
+        users = {}
+        for user_data in data["data"]["users"]:
+            user_data = user_data["result"]
+            user = User.from_raw_data(user_data)
+            users[user.id] = user
+        return users
+
+    async def _request_tweet(self, tweet_id: int | str) -> Tweet:
+        url, query_id = self._action_to_url("TweetDetail")
         variables = {
             "focalTweetId": str(tweet_id),
             "with_rux_injections": False,
             "includePromotedContent": True,
             "withCommunity": True,
             "withQuickPromoteEligibilityTweetFields": True,
             "withBirdwatchNotes": True,
@@ -797,20 +869,79 @@
             "freedom_of_speech_not_reach_fetch_enabled": True,
             "standardized_nudges_misinfo": True,
             "tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled": True,
             "longform_notetweets_rich_text_read_enabled": True,
             "longform_notetweets_inline_media_enabled": True,
             "responsive_web_enhance_cards_enabled": False,
         }
-        params = {
+        query = {
             "variables": to_json(variables),
             "features": to_json(features),
         }
-        response, response_json = await self.request("GET", url, params=params)
-        return response_json
+        response, data = await self.request("GET", url, params=query)
+        instructions = data["data"]["threaded_conversation_with_injections_v2"]["instructions"]  # type: ignore
+        tweet_data = tweets_data_from_instructions(instructions)[0]
+        return Tweet.from_raw_data(tweet_data)
+
+    async def _request_tweets(self, user_id: int | str, count: int = 20) -> list[Tweet]:
+        url, query_id = self._action_to_url("UserTweets")
+        variables = {
+            "userId": str(user_id),
+            "count": count,
+            "includePromotedContent": True,
+            "withQuickPromoteEligibilityTweetFields": True,
+            "withVoice": True,
+            "withV2Timeline": True,
+        }
+        features = {
+            "responsive_web_graphql_exclude_directive_enabled": True,
+            "verified_phone_label_enabled": False,
+            "creator_subscriptions_tweet_preview_api_enabled": True,
+            "responsive_web_graphql_timeline_navigation_enabled": True,
+            "responsive_web_graphql_skip_user_profile_image_extensions_enabled": False,
+            "c9s_tweet_anatomy_moderator_badge_enabled": True,
+            "tweetypie_unmention_optimization_enabled": True,
+            "responsive_web_edit_tweet_api_enabled": True,
+            "graphql_is_translatable_rweb_tweet_is_translatable_enabled": True,
+            "view_counts_everywhere_api_enabled": True,
+            "longform_notetweets_consumption_enabled": True,
+            "responsive_web_twitter_article_tweet_consumption_enabled": False,
+            "tweet_awards_web_tipping_enabled": False,
+            "freedom_of_speech_not_reach_fetch_enabled": True,
+            "standardized_nudges_misinfo": True,
+            "tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled": True,
+            "rweb_video_timestamps_enabled": True,
+            "longform_notetweets_rich_text_read_enabled": True,
+            "longform_notetweets_inline_media_enabled": True,
+            "responsive_web_media_download_video_enabled": False,
+            "responsive_web_enhance_cards_enabled": False,
+        }
+        params = {"variables": to_json(variables), "features": to_json(features)}
+        response, data = await self.request("GET", url, params=params)
+
+        instructions = data["data"]["user"]["result"]["timeline_v2"]["timeline"][
+            "instructions"
+        ]
+        tweets_data = tweets_data_from_instructions(instructions)
+        return [Tweet.from_raw_data(tweet_data) for tweet_data in tweets_data]
+
+    async def request_tweet(self, tweet_id: int | str) -> Tweet:
+        return await self._request_tweet(tweet_id)
+
+    async def request_tweets(
+        self,
+        user_id: int | str = None,
+        count: int = 20,
+    ) -> list[Tweet]:
+        if not user_id:
+            if not self.account.id:
+                await self.request_user()
+            user_id = self.account.id
+
+        return await self._request_tweets(user_id, count)
 
     async def _update_profile_image(
         self, type: Literal["banner", "image"], media_id: str | int
     ) -> str:
         """
         :return: Image URL
         """
@@ -828,16 +959,16 @@
             "include_ext_has_nft_avatar": "1",
             "include_ext_is_blue_verified": "1",
             "include_ext_verified_type": "1",
             "include_ext_profile_image_shape": "1",
             "skip_status": "1",
             "return_user": "true",
         }
-        response, response_json = await self.request("POST", url, params=params)
-        image_url = response_json[f"profile_{type}_url"]
+        response, data = await self.request("POST", url, params=params)
+        image_url = data[f"profile_{type}_url"]
         return image_url
 
     async def update_profile_avatar(self, media_id: int | str) -> str:
         """
         :return: Image URL
         """
         return await self._update_profile_image("image", media_id)
@@ -846,40 +977,41 @@
         """
         :return: Image URL
         """
         return await self._update_profile_image("banner", media_id)
 
     async def change_username(self, username: str) -> bool:
         url = "https://twitter.com/i/api/1.1/account/settings.json"
-        data = {"screen_name": username}
-        response, response_json = await self.request("POST", url, data=data)
-        new_username = response_json["screen_name"]
-        is_changed = new_username == username
+        payload = {"screen_name": username}
+        response, data = await self.request("POST", url, data=payload)
+        new_username = data["screen_name"]
+        changed = new_username == username
         self.account.username = new_username
-        return is_changed
+        return changed
 
     async def change_password(self, password: str) -> bool:
         """
         После изменения пароля обновляется auth_token!
         """
         if not self.account.password:
             raise ValueError(f"Specify the current password before changing it")
 
         url = "https://twitter.com/i/api/i/account/change_password.json"
-        data = {
+        payload = {
             "current_password": self.account.password,
             "password": password,
             "password_confirmation": password,
         }
-        response, response_json = await self.request("POST", url, data=data)
-        is_changed = response_json["status"] == "ok"
+        response, data = await self.request("POST", url, data=payload)
+        changed = data["status"] == "ok"
+        # TODO Делать это автоматически в методе request
         auth_token = response.cookies.get("auth_token", domain=".twitter.com")
         self.account.auth_token = auth_token
         self.account.password = password
-        return is_changed
+        return changed
 
     async def update_profile(
         self,
         name: str = None,
         description: str = None,
         location: str = None,
         website: str = None,
@@ -887,41 +1019,38 @@
         """
         Locks an account!
         """
         if name is None and description is None:
             raise ValueError("Specify at least one param")
 
         url = "https://twitter.com/i/api/1.1/account/update_profile.json"
-        headers = {"content-type": "application/x-www-form-urlencoded"}
+        # headers = {"content-type": "application/x-www-form-urlencoded"}
         # Создаем словарь data, включая в него только те ключи, для которых значения не равны None
-        data = {
+        payload = {
             k: v
             for k, v in [
                 ("name", name),
                 ("description", description),
                 ("location", location),
                 ("url", website),
             ]
             if v is not None
         }
-        response, response_json = await self.request(
-            "POST", url, headers=headers, data=data
-        )
+        # response, response_json = await self.request("POST", url, headers=headers, data=payload)
+        response, data = await self.request("POST", url, data=payload)
         # Проверяем, что все переданные параметры соответствуют полученным
-        is_updated = all(
-            response_json.get(key) == value
-            for key, value in data.items()
-            if key != "url"
+        updated = all(
+            data.get(key) == value for key, value in payload.items() if key != "url"
         )
         if website:
-            is_updated &= URL(website) == URL(
-                response_json["entities"]["url"]["urls"][0]["expanded_url"]
+            updated &= URL(website) == URL(
+                data["entities"]["url"]["urls"][0]["expanded_url"]
             )
-        await self.request_user_data()
-        return is_updated
+        await self.request_user()
+        return updated
 
     async def establish_status(self):
         url = "https://twitter.com/i/api/1.1/account/update_profile.json"
         try:
             await self.request("POST", url)
         except BadAccount:
             pass
@@ -943,24 +1072,24 @@
             "birthdate_visibility": visibility,
             "birthdate_year_visibility": year_visibility,
         }
         response, response_json = await self.request(
             "POST", url, headers=headers, data=data
         )
         birthdate_data = response_json["extended_profile"]["birthdate"]
-        is_updated = all(
+        updated = all(
             (
                 birthdate_data["day"] == day,
                 birthdate_data["month"] == month,
                 birthdate_data["year"] == year,
                 birthdate_data["visibility"] == visibility,
                 birthdate_data["year_visibility"] == year_visibility,
             )
         )
-        return is_updated
+        return updated
 
     async def send_message(self, user_id: int | str, text: str) -> dict:
         """
         :return: Event data
         """
         url = "https://api.twitter.com/1.1/direct_messages/events/new.json"
         payload = {
@@ -968,17 +1097,17 @@
                 "type": "message_create",
                 "message_create": {
                     "target": {"recipient_id": user_id},
                     "message_data": {"text": text},
                 },
             }
         }
-        response, response_json = await self.request("POST", url, json=payload)
-        event_data = response_json["event"]
-        return event_data
+        response, data = await self.request("POST", url, json=payload)
+        event_data = data["event"]
+        return event_data  # TODO Возвращать модель, а не словарь
 
     async def request_messages(self) -> list[dict]:
         """
         :return: Messages data
         """
         url = "https://twitter.com/i/api/1.1/dm/inbox_initial_state.json"
         params = {
@@ -1019,64 +1148,15 @@
         }
         response, response_json = await self.request("GET", url, params=params)
         messages = [
             entry["message"]
             for entry in response_json["inbox_initial_state"]["entries"]
             if "message" in entry
         ]
-        return messages
-
-    async def request_tweets(self, user_id: str | int, count: int = 20) -> list[Tweet]:
-        url, query_id = self._action_to_url("UserTweets")
-        variables = {
-            "userId": str(user_id),
-            "count": count,
-            "includePromotedContent": True,
-            "withQuickPromoteEligibilityTweetFields": True,
-            "withVoice": True,
-            "withV2Timeline": True,
-        }
-        features = {
-            "responsive_web_graphql_exclude_directive_enabled": True,
-            "verified_phone_label_enabled": False,
-            "creator_subscriptions_tweet_preview_api_enabled": True,
-            "responsive_web_graphql_timeline_navigation_enabled": True,
-            "responsive_web_graphql_skip_user_profile_image_extensions_enabled": False,
-            "c9s_tweet_anatomy_moderator_badge_enabled": True,
-            "tweetypie_unmention_optimization_enabled": True,
-            "responsive_web_edit_tweet_api_enabled": True,
-            "graphql_is_translatable_rweb_tweet_is_translatable_enabled": True,
-            "view_counts_everywhere_api_enabled": True,
-            "longform_notetweets_consumption_enabled": True,
-            "responsive_web_twitter_article_tweet_consumption_enabled": False,
-            "tweet_awards_web_tipping_enabled": False,
-            "freedom_of_speech_not_reach_fetch_enabled": True,
-            "standardized_nudges_misinfo": True,
-            "tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled": True,
-            "rweb_video_timestamps_enabled": True,
-            "longform_notetweets_rich_text_read_enabled": True,
-            "longform_notetweets_inline_media_enabled": True,
-            "responsive_web_media_download_video_enabled": False,
-            "responsive_web_enhance_cards_enabled": False,
-        }
-        params = {"variables": to_json(variables), "features": to_json(features)}
-        response, response_json = await self.request("GET", url, params=params)
-
-        tweets = []
-        for instruction in response_json["data"]["user"]["result"]["timeline_v2"][
-            "timeline"
-        ]["instructions"]:
-            if instruction["type"] == "TimelineAddEntries":
-                for entry in instruction["entries"]:
-                    if entry["entryId"].startswith("tweet"):
-                        tweet_data = entry["content"]["itemContent"]["tweet_results"][
-                            "result"
-                        ]
-                        tweets.append(Tweet.from_raw_data(tweet_data))
-        return tweets
+        return messages  # TODO Возвращать модели, а не словари
 
     async def _confirm_unlock(
         self,
         authenticity_token: str,
         assignment_token: str,
         verification_string: str = None,
     ) -> tuple[requests.Response, str]:
@@ -1370,15 +1450,15 @@
             raise TwitterException(f"Failed to login: email verification!")
 
         if "LoginTwoFactorAuthChallenge" in subtask_ids:
             flow_token, subtasks = await self._login_two_factor_auth_challenge(
                 flow_token
             )
 
-        # TODO Возможно, стоит добавить отслеживание этих параметров прямо в request
+        # TODO Делать это автоматически в методе request
         self.account.auth_token = self._session.cookies["auth_token"]
         self.account.ct0 = self._session.cookies["ct0"]
 
         await self._finish_task(flow_token)
 
     async def login(self):
         if self.account.auth_token:
@@ -1393,15 +1473,15 @@
             raise ValueError("No password")
 
         await self._login()
         await self.establish_status()
 
     async def totp_is_enabled(self):
         if not self.account.id:
-            await self.request_user_data()
+            await self.request_user()
 
         url = f"https://twitter.com/i/api/1.1/strato/column/User/{self.account.id}/account-security/twoFactorAuthSettings2"
         response, data = await self.request("GET", url)
         return "Totp" in [
             method_data["twoFactorType"] for method_data in data["methods"]
         ]
 
@@ -1558,9 +1638,9 @@
         if not self.account.password:
             raise ValueError("Password is required for this action")
 
         if await self.totp_is_enabled():
             return
 
         # TODO Осторожно, костыль! Перед началом работы вызываем request_user_data, чтоб убедиться что нет других ошибок
-        await self.request_user_data()
+        await self.request_user()
         await self._enable_totp()
```

### Comparing `tweepy_self-1.6.3/twitter/errors.py` & `tweepy_self-1.9.0/twitter/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     "BadToken",
     "Locked",
     "ConsentLocked",
     "Suspended",
 ]
 
 
+# TODO Возвращать аккаунт в теле исключения
 class TwitterException(Exception):
     pass
 
 
 class FailedToFindDuplicatePost(TwitterException):
     pass
 
@@ -71,15 +72,15 @@
                 exception_message = (
                     f"(response status: {response.status_code}) Rate limit exceeded."
                     f" Set wait_on_rate_limit=True to ignore this exception."
                 )
             super().__init__(exception_message)
             return
 
-        self.api_errors = data.get("errors", [])
+        self.api_errors = data.get("errors", [data])
         self.detail = data.get("detail")
 
         for error in self.api_errors:
             if "code" in error:
                 self.api_codes.append(error["code"])
             if "message" in error:
                 self.api_messages.append(error["message"])
```

### Comparing `tweepy_self-1.6.3/twitter/utils/file.py` & `tweepy_self-1.9.0/twitter/utils/file.py`

 * *Files identical despite different names*

### Comparing `tweepy_self-1.6.3/twitter/utils/html.py` & `tweepy_self-1.9.0/twitter/utils/html.py`

 * *Files identical despite different names*

### Comparing `tweepy_self-1.6.3/PKG-INFO` & `tweepy_self-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: tweepy-self
-Version: 1.6.3
+Version: 1.9.0
 Summary: Twitter (selfbot) for Python!
 Home-page: https://github.com/alenkimov/tweepy-self
 Author: Alen
 Author-email: alen.kimov@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiohttp (>=3.9,<4.0)
 Requires-Dist: beautifulsoup4 (>=4,<5)
-Requires-Dist: better-proxy (==1.1.1)
+Requires-Dist: better-proxy (>=1.1,<2.0)
 Requires-Dist: curl_cffi (==0.6.0b9)
+Requires-Dist: loguru (>=0.7,<0.8)
 Requires-Dist: lxml (>=5,<6)
 Requires-Dist: pydantic (>=1)
 Requires-Dist: pyotp (>=2,<3)
-Requires-Dist: python3-capsolver (>=0.9,<0.10)
+Requires-Dist: requests (>=2,<3)
+Requires-Dist: tenacity (>=8,<9)
 Requires-Dist: yarl (>=1,<2)
 Project-URL: Repository, https://github.com/alenkimov/tweepy-self
+Project-URL: Source, https://github.com/alenkimov/tweepy-self
 Description-Content-Type: text/markdown
 
 # Tweepy-self
 [![Telegram channel](https://img.shields.io/endpoint?url=https://runkit.io/damiankrawczyk/telegram-badge/branches/master?url=https://t.me/cum_insider)](https://t.me/cum_insider)
 [![PyPI version info](https://img.shields.io/pypi/v/tweepy-self.svg)](https://pypi.python.org/pypi/tweepy-self)
 [![PyPI supported Python versions](https://img.shields.io/pypi/pyversions/tweepy-self.svg)](https://pypi.python.org/pypi/tweepy-self)
 [![PyPI downloads per month](https://img.shields.io/pypi/dm/tweepy-self.svg)](https://pypi.python.org/pypi/tweepy-self)
@@ -95,35 +99,37 @@
 Не каждое взаимодействие с Twitter достоверно определяет статус аккаунта.
 Например, простой запрос данных об аккаунте честно вернет данные, даже если ваш аккаунт заморожен.
 
 Для достоверной установки статуса аккаунта используйте метод `establish_status()`
 
 ### Примеры работы
 Запрос информации о пользователе:
+
 ```python
 # Запрос информации о текущем пользователе:
-me = await twitter_client.request_user_data()
+me = await twitter_client.request_user()
 print(f"[{account.short_auth_token}] {me}")
 print(f"Аккаунт создан: {me.created_at}")
 print(f"Following (подписан ты): {me.followings_count}")
 print(f"Followers (подписаны на тебя): {me.followers_count}")
 print(f"Прочая информация: {me.raw_data}")
 
 # Запрос информации об ином пользователе:
-elonmusk = await twitter.request_user_data("@elonmusk")
+elonmusk = await twitter.request_user("@elonmusk")
 print(elonmusk)
 ```
 
 Смена имени пользователя и пароля:
+
 ```python
 account = twitter.Account("auth_token", password="password")
 ...
 await twitter_client.change_username("new_username")
-await twitter_client.request_user_data()
-print(f"New username: {account.data.username}")
+await twitter_client.request_user()
+print(f"New username: {account.username}")
 
 await twitter_client.change_password("new_password")
 print(f"New password: {account.password}")
 print(f"New auth_token: {account.auth_token}")
 ```
 
 Смена данных профиля:
@@ -161,16 +167,17 @@
 
 bind_code = await twitter_client.oauth_2(**bind_data)
 # Передайте код авторизации (привязки) сервису.
 # Сервис также может потребовать state, если он динамический.
 ```
 
 Отправка сообщения:
+
 ```python
-bro = await twitter_client.request_user_data("@username")
+bro = await twitter_client.request_user("@username")
 await twitter_client.send_message(bro.id, "I love you!")
 ```
 
 Запрос входящих сообщений:
 ```python
 messages = await twitter_client.request_messages()
 for message in messages:
```

