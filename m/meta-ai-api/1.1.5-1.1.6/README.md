# Comparing `tmp/meta_ai_api-1.1.5.tar.gz` & `tmp/meta_ai_api-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meta_ai_api-1.1.5.tar", last modified: Mon Apr 22 17:01:43 2024, max compression
+gzip compressed data, was "meta_ai_api-1.1.6.tar", last modified: Wed Apr 24 17:24:42 2024, max compression
```

## Comparing `meta_ai_api-1.1.5.tar` & `meta_ai_api-1.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:01:43.153195 meta_ai_api-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-04-22 17:01:43.153195 meta_ai_api-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-04-22 17:01:38.000000 meta_ai_api-1.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-22 17:01:38.000000 meta_ai_api-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-22 17:01:43.153195 meta_ai_api-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-22 17:01:38.000000 meta_ai_api-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:01:43.149195 meta_ai_api-1.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:01:43.149195 meta_ai_api-1.1.5/src/meta_ai_api/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-22 17:01:38.000000 meta_ai_api-1.1.5/src/meta_ai_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-22 17:01:38.000000 meta_ai_api-1.1.5/src/meta_ai_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13274 2024-04-22 17:01:38.000000 meta_ai_api-1.1.5/src/meta_ai_api/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     9883 2024-04-22 17:01:38.000000 meta_ai_api-1.1.5/src/meta_ai_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:01:43.153195 meta_ai_api-1.1.5/src/meta_ai_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-04-22 17:01:43.000000 meta_ai_api-1.1.5/src/meta_ai_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-22 17:01:43.000000 meta_ai_api-1.1.5/src/meta_ai_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 17:01:43.000000 meta_ai_api-1.1.5/src/meta_ai_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-22 17:01:43.000000 meta_ai_api-1.1.5/src/meta_ai_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 17:01:43.000000 meta_ai_api-1.1.5/src/meta_ai_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:24:42.700308 meta_ai_api-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    10160 2024-04-24 17:24:42.700308 meta_ai_api-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-04-24 17:24:38.000000 meta_ai_api-1.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-24 17:24:38.000000 meta_ai_api-1.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-24 17:24:42.700308 meta_ai_api-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-24 17:24:38.000000 meta_ai_api-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:24:42.696308 meta_ai_api-1.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:24:42.696308 meta_ai_api-1.1.6/src/meta_ai_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-24 17:24:38.000000 meta_ai_api-1.1.6/src/meta_ai_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-24 17:24:38.000000 meta_ai_api-1.1.6/src/meta_ai_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14256 2024-04-24 17:24:38.000000 meta_ai_api-1.1.6/src/meta_ai_api/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-04-24 17:24:38.000000 meta_ai_api-1.1.6/src/meta_ai_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:24:42.700308 meta_ai_api-1.1.6/src/meta_ai_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10160 2024-04-24 17:24:42.000000 meta_ai_api-1.1.6/src/meta_ai_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-24 17:24:42.000000 meta_ai_api-1.1.6/src/meta_ai_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 17:24:42.000000 meta_ai_api-1.1.6/src/meta_ai_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-24 17:24:42.000000 meta_ai_api-1.1.6/src/meta_ai_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 17:24:42.000000 meta_ai_api-1.1.6/src/meta_ai_api.egg-info/top_level.txt
```

### Comparing `meta_ai_api-1.1.5/PKG-INFO` & `meta_ai_api-1.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,7 @@
-Metadata-Version: 2.1
-Name: meta_ai_api
-Version: 1.1.5
-Summary: Meta AI API Wrapper to interact with the Meta AI API
-Home-page: https://github.com/tomchen/example_pypi_package
-Author: Roméo Phillips
-Author-email: phillipsromeo@gmail.com
-Project-URL: Documentation, https://github.com/Strvm/meta-ai-api
-Project-URL: Bug Reports, https://github.com/Strvm/meta-ai-api
-Project-URL: Source Code, https://github.com/Strvm/meta-ai-api
-Keywords: llm,ai,meta_ai_api
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Requires-Dist: requests
-Requires-Dist: requests-html
-Requires-Dist: lxml_html_clean
-Provides-Extra: dev
-Requires-Dist: check-manifest; extra == "dev"
-
 # MetaAI API Wrapper
 
 MetaAI is a Python library designed to interact with Meta's AI APIs that run in the backend of https://www.meta.ai/. It encapsulates the complexities of authentication and communication with the APIs, providing a straightforward interface for sending queries and receiving responses.
 
 With this you can easily prompt the AI with a message and get a response, directly from your Python code. **NO API KEY REQUIRED**
 
 **Meta AI is connected to the internet, so you will be able to get the latest real-time responses from the AI.** (powered by Bing)
@@ -121,14 +91,29 @@
          "link":"https://en.wikipedia.org/wiki/History_of_the_Golden_State_Warriors",
          "title":"History of the Golden State Warriors"
       }
    ]
 }
 ```
 
+**Using proxy**:
+
+```python
+from meta_ai_api import MetaAI
+
+proxy = {
+    'http': 'http://proxy_address:port',
+    'https': 'https://proxy_address:port'
+}
+
+ai = MetaAI(proxy=proxy)
+response = ai.prompt(message="How to find out which mushrooms are edible?")
+print(response)
+```
+
 **Streaming Response**:
 
 ```python
 from meta_ai_api import MetaAI
 
 ai = MetaAI()
 response = ai.prompt(message="What was the Warriors score last game?", stream=True)
@@ -197,7 +182,29 @@
          "type":"IMAGE",
          "prompt":"a tech CEO"
       }
    ]
 }
 ```
 ![Tech CEO](https://scontent-lax3-1.xx.fbcdn.net/o1/v/t0/f1/m247/3497663176351797954_3954783377_21-04-2024-14-17-47.jpeg?_nc_ht=scontent-lax3-1.xx.fbcdn.net&_nc_cat=110&ccb=9-4&oh=00_AfBp3bAfcuofqtI-z9D4bHw-GuGgCNPH_xhMM0PG_95S9Q&oe=66277AE9&_nc_sid=5b3566)
+
+# Copyright:
+This program is licensed under the GNU GPL v3. All code has been written by me, Strvm.
+
+# Copyright Notice:
+```
+Strvm/meta-ai-api: a reverse engineered API wrapper for MetaAI
+Copyright (C) 2023 ading2210
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+```
```

### Comparing `meta_ai_api-1.1.5/setup.py` & `meta_ai_api-1.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `meta_ai_api-1.1.5/src/meta_ai_api/main.py` & `meta_ai_api-1.1.6/src/meta_ai_api/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,35 +23,60 @@
 
 class MetaAI:
     """
     A class to interact with the Meta AI API to obtain and use access tokens for sending
     and receiving messages from the Meta AI Chat API.
     """
 
-    def __init__(self, fb_email: str = None, fb_password: str = None):
+    def __init__(self, fb_email: str = None, fb_password: str = None, proxy: dict = None):
         self.session = requests.Session()
         self.session.headers.update(
             {
                 "user-agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 "
                 "(KHTML, like Gecko) Chrome/122.0.0.0 Safari/537.36",
             }
         )
         self.access_token = None
         self.fb_email = fb_email
         self.fb_password = fb_password
+        self.proxy = proxy
+        if self.proxy and not self.check_proxy():
+            raise ConnectionError("Unable to connect to proxy. Please check your proxy settings.")
+
         self.is_authed = fb_password is not None and fb_email is not None
         self.cookies = self.get_cookies()
 
+    def check_proxy(self, test_url: str="https://api.ipify.org/?format=json") -> bool:
+        """
+        Checks the proxy connection by making a request to a test URL.
+        
+        Args:
+            test_url (str): A test site from which we check that the proxy is installed correctly.
+
+        Returns:
+            bool: True if the proxy is working, False otherwise.
+        """
+        try:
+            response = self.session.get(test_url, proxies=self.proxy, timeout=10)
+            if response.status_code == 200:
+                print(response.json())
+                self.session.proxies = self.proxy
+                return True
+            return False
+        except requests.RequestException:
+            return False
+
     def get_access_token(self) -> str:
         """
         Retrieves an access token using Meta's authentication API.
 
         Returns:
             str: A valid access token.
         """
+
         url = "https://www.meta.ai/api/graphql/"
         payload = {
             "lsd": self.cookies["lsd"],
             "fb_api_caller_class": "RelayModern",
             "fb_api_req_friendly_name": "useAbraAcceptTOSForTempUserMutation",
             "variables": {
                 "dob": "1999-01-01",
@@ -66,21 +91,23 @@
             "cookie": f'_js_datr={self.cookies["_js_datr"]}; '
             f'abra_csrf={self.cookies["abra_csrf"]}; datr={self.cookies["datr"]};',
             "sec-fetch-site": "same-origin",
             "x-fb-friendly-name": "useAbraAcceptTOSForTempUserMutation",
         }
 
         response = self.session.post(url, headers=headers, data=payload)
+
         try:
             auth_json = response.json()
         except json.JSONDecodeError:
             raise FacebookRegionBlocked(
                 "Unable to receive a valid response from Meta AI. This is likely due to your region being blocked. "
                 "Try manually accessing https://www.meta.ai/ to confirm."
             )
+
         access_token = auth_json["data"]["xab_abra_accept_terms_of_service"][
             "new_temp_user_auth"
         ]["access_token"]
         return access_token
 
     def prompt(
         self, message: str, stream: bool = False, attempts: int = 0
@@ -138,14 +165,15 @@
             "content-type": "application/x-www-form-urlencoded",
             "x-fb-friendly-name": "useAbraSendMessageMutation",
         }
         if self.is_authed:
             headers["cookie"] = f'abra_sess={self.cookies["abra_sess"]}'
             # Recreate the session to avoid cookie leakage when user is authenticated
             self.session = requests.Session()
+            self.session.proxies = self.proxy
 
         response = self.session.post(url, headers=headers, data=payload, stream=stream)
         if not stream:
             raw_response = response.text
             last_streamed_response = self.extract_last_response(raw_response)
             if not last_streamed_response:
                 return self.retry(message, stream=stream, attempts=attempts)
```

### Comparing `meta_ai_api-1.1.5/src/meta_ai_api/utils.py` & `meta_ai_api-1.1.6/src/meta_ai_api/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         .get("content", [])
     ):
         text += content["text"] + "\n"
     return text
 
 
 # Function to perform the login
-def get_fb_session(email, password):
+def get_fb_session(email, password, proxies=None):
     login_url = "https://mbasic.facebook.com/login/"
     headers = {
         "authority": "mbasic.facebook.com",
         "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
         "accept-language": "en-US,en;q=0.9",
         "sec-ch-ua": '"Chromium";v="122", "Not(A:Brand";v="24", "Google Chrome";v="122"',
         "sec-ch-ua-mobile": "?0",
@@ -94,15 +94,15 @@
         "sec-fetch-mode": "navigate",
         "sec-fetch-site": "none",
         "sec-fetch-user": "?1",
         "upgrade-insecure-requests": "1",
         "user-agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.0.0 Safari/537.36",
     }
     # Send the GET request
-    response = requests.get(login_url, headers=headers)
+    response = requests.get(login_url, headers=headers, proxies=proxies)
     soup = BeautifulSoup(response.text, "html.parser")
 
     # Parse necessary parameters from the login form
     lsd = soup.find("input", {"name": "lsd"})["value"]
     jazoest = soup.find("input", {"name": "jazoest"})["value"]
     li = soup.find("input", {"name": "li"})["value"]
     m_ts = soup.find("input", {"name": "m_ts"})["value"]
@@ -138,14 +138,15 @@
         "upgrade-insecure-requests": "1",
         "user-agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.0.0 Safari/537.36",
         "viewport-width": "1728",
     }
 
     # Send the POST request
     session = requests.session()
+    session.proxies = proxies
 
     result = session.post(post_url, headers=headers, data=data)
     if "sb" not in session.cookies:
         raise FacebookInvalidCredentialsException(
             "Was not able to login to Facebook. Please check your credentials. "
             "You may also have been rate limited. Try to connect to Facebook manually."
         )
@@ -179,15 +180,15 @@
         "pragma": "no-cache",
         "referer": "https://www.meta.ai/",
         "sec-fetch-mode": "cors",
         "sec-fetch-site": "same-origin",
         "user-agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.0.0 Safari/537.36",
     }
 
-    response = requests.request("POST", url, headers=headers, data=payload)
+    response = requests.request("POST", url, headers=headers, data=payload, proxies=proxies)
 
     state = extract_value(response.text, start_str='"state":"', end_str='"')
 
     url = f"https://www.facebook.com/oidc/?app_id=1358015658191005&scope=openid%20linking&response_type=code&redirect_uri=https%3A%2F%2Fwww.meta.ai%2Fauth%2F&no_universal_links=1&deoia=1&state={state}"
     payload = {}
     headers = {
         "authority": "www.facebook.com",
@@ -199,14 +200,15 @@
         "sec-fetch-mode": "navigate",
         "sec-fetch-site": "cross-site",
         "sec-fetch-user": "?1",
         "upgrade-insecure-requests": "1",
         "user-agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.0.0 Safari/537.36",
     }
     session = requests.session()
+    session.proxies = proxies
     response = session.get(url, headers=headers, data=payload, allow_redirects=False)
 
     next_url = response.headers["Location"]
 
     url = next_url
 
     payload = {}
```

### Comparing `meta_ai_api-1.1.5/src/meta_ai_api.egg-info/PKG-INFO` & `meta_ai_api-1.1.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_ai_api
-Version: 1.1.5
+Version: 1.1.6
 Summary: Meta AI API Wrapper to interact with the Meta AI API
 Home-page: https://github.com/tomchen/example_pypi_package
 Author: Roméo Phillips
 Author-email: phillipsromeo@gmail.com
 Project-URL: Documentation, https://github.com/Strvm/meta-ai-api
 Project-URL: Bug Reports, https://github.com/Strvm/meta-ai-api
 Project-URL: Source Code, https://github.com/Strvm/meta-ai-api
@@ -121,14 +121,29 @@
          "link":"https://en.wikipedia.org/wiki/History_of_the_Golden_State_Warriors",
          "title":"History of the Golden State Warriors"
       }
    ]
 }
 ```
 
+**Using proxy**:
+
+```python
+from meta_ai_api import MetaAI
+
+proxy = {
+    'http': 'http://proxy_address:port',
+    'https': 'https://proxy_address:port'
+}
+
+ai = MetaAI(proxy=proxy)
+response = ai.prompt(message="How to find out which mushrooms are edible?")
+print(response)
+```
+
 **Streaming Response**:
 
 ```python
 from meta_ai_api import MetaAI
 
 ai = MetaAI()
 response = ai.prompt(message="What was the Warriors score last game?", stream=True)
@@ -197,7 +212,29 @@
          "type":"IMAGE",
          "prompt":"a tech CEO"
       }
    ]
 }
 ```
 ![Tech CEO](https://scontent-lax3-1.xx.fbcdn.net/o1/v/t0/f1/m247/3497663176351797954_3954783377_21-04-2024-14-17-47.jpeg?_nc_ht=scontent-lax3-1.xx.fbcdn.net&_nc_cat=110&ccb=9-4&oh=00_AfBp3bAfcuofqtI-z9D4bHw-GuGgCNPH_xhMM0PG_95S9Q&oe=66277AE9&_nc_sid=5b3566)
+
+# Copyright:
+This program is licensed under the GNU GPL v3. All code has been written by me, Strvm.
+
+# Copyright Notice:
+```
+Strvm/meta-ai-api: a reverse engineered API wrapper for MetaAI
+Copyright (C) 2023 ading2210
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+```
```

