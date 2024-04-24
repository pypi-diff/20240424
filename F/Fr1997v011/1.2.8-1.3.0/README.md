# Comparing `tmp/Fr1997v011-1.2.8.tar.gz` & `tmp/Fr1997v011-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.2.8.tar", last modified: Fri Apr 19 12:37:53 2024, max compression
+gzip compressed data, was "Fr1997v011-1.3.0.tar", last modified: Tue Apr 23 10:39:21 2024, max compression
```

## Comparing `Fr1997v011-1.2.8.tar` & `Fr1997v011-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 12:37:53.243040 Fr1997v011-1.2.8/
-drwxrwxrwx   0        0        0        0 2024-04-19 12:37:53.237040 Fr1997v011-1.2.8/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-04-19 12:37:53.000000 Fr1997v011-1.2.8/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-04-19 12:37:53.000000 Fr1997v011-1.2.8/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 12:37:53.000000 Fr1997v011-1.2.8/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-19 12:37:53.000000 Fr1997v011-1.2.8/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-04-19 12:37:53.000000 Fr1997v011-1.2.8/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.2.8/LICENSE
--rw-rw-rw-   0        0        0      182 2024-04-19 12:37:53.242040 Fr1997v011-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-04-19 12:37:52.000000 Fr1997v011-1.2.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 12:37:53.238040 Fr1997v011-1.2.8/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.2.8/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 12:37:53.240040 Fr1997v011-1.2.8/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2023-10-09 02:29:18.000000 Fr1997v011-1.2.8/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   145627 2024-04-19 12:37:49.000000 Fr1997v011-1.2.8/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-04-19 12:37:53.241040 Fr1997v011-1.2.8/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.2.8/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-19 12:37:53.243040 Fr1997v011-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-04-19 12:37:49.000000 Fr1997v011-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:39:21.243054 Fr1997v011-1.3.0/
+drwxrwxrwx   0        0        0        0 2024-04-23 10:39:21.229538 Fr1997v011-1.3.0/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-23 10:39:20.000000 Fr1997v011-1.3.0/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2024-04-23 10:39:21.000000 Fr1997v011-1.3.0/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 10:39:20.000000 Fr1997v011-1.3.0/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-23 10:39:20.000000 Fr1997v011-1.3.0/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-04-23 10:39:20.000000 Fr1997v011-1.3.0/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-04-23 10:39:21.242054 Fr1997v011-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-04-23 02:41:51.000000 Fr1997v011-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 10:39:21.231542 Fr1997v011-1.3.0/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.3.0/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:39:21.236542 Fr1997v011-1.3.0/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2023-10-09 02:29:18.000000 Fr1997v011-1.3.0/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   164931 2024-04-23 10:33:35.000000 Fr1997v011-1.3.0/fr1997_mode/mode_func/all_func.py
+-rw-rw-rw-   0        0        0    37242 2024-04-23 03:22:03.000000 Fr1997v011-1.3.0/fr1997_mode/mode_func/json_data_fastgpt.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:39:21.240054 Fr1997v011-1.3.0/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.3.0/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-23 10:39:21.243054 Fr1997v011-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-04-23 10:39:18.000000 Fr1997v011-1.3.0/setup.py
```

### Comparing `Fr1997v011-1.2.8/LICENSE` & `Fr1997v011-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.2.8/README.md` & `Fr1997v011-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```sh
 python setup.py sdist
 ```
 
 ### （本地）安装包
 
 ```sh
-pip install dist/Fr1997v011-1.2.8.tar.gz
+pip install dist/Fr1997v011-1.2.9.tar.gz
 ```
 
 ### 下载包
 
 ```sh
 pip install Fr1997v011
 ```
```

### Comparing `Fr1997v011-1.2.8/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.3.0/fr1997_mode/mode_func/all_func.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,40 +12,42 @@
 import ctypes
 import struct
 import base64
 import memcache  # pip install python-memcached
 from elasticsearch import Elasticsearch  # ES
 from concurrent.futures import ThreadPoolExecutor  # 线程次
 from pypinyin import pinyin, Style  # 汉字转拼音
-
+import socket
+import inspect
 import execjs  # pip install PyExecJS
 from urllib import parse  # 三位
 from urllib.parse import quote  # 两位
 from urllib.parse import urlparse, quote
 
 # 腾讯云cos  pip install -U cos-python-sdk-v5
 from qcloud_cos import CosConfig
 from qcloud_cos import CosS3Client
 
 """
-    pip install redis
-    pip install elasticsearch
-    pip install python-memcached
-    pip install PyExecJS
-    pip install -U cos-python-sdk-v5
-    pip install pypinyin
+    pip3 install redis
+    pip3 install pymysql
+    pip3 install elasticsearch
+    pip3 install python-memcached
+    pip3 install PyExecJS
+    pip3 install -U cos-python-sdk-v5
+    pip3 install pypinyin
 """
 
 """
     配置文件
         所有配置在这个地方读取 
         使用内存缓存机制 memcache
         没有读取到内存中的配置，这个包相当于不能用
     pip3 cache purge
-    pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple Fr1997v011==1.1.9
+    pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple Fr1997v011==1.2.8
 """
 
 
 # 存储内存数据
 def cache_set(key, data, save_time=None):
     mc = memcache.Client(['127.0.0.1:11211'], debug=True)
     if save_time:
@@ -628,17 +630,17 @@
             1004：修改人
             1005：自动编号
             13：电话号码
             22：地理位置
 
             -- 示例
             field_update = [
-                # {"field_name": '普通文本', "type": 1},  # 添加普通文本
-                # {"field_name": '数字-整数', "type": 2, "property": {"formatter": "0"}},  # 添加数字 整形
-                # {"field_name": '数字-浮点', "type": 2, "property": {"formatter": "0.00"}},  # 添加数字 浮点数
+                {"field_name": '普通文本', "type": 1},  # 添加普通文本
+                {"field_name": '数字-整数', "type": 2, "property": {"formatter": "0"}},  # 添加数字 整形
+                {"field_name": '数字-浮点', "type": 2, "property": {"formatter": "0.00"}},  # 添加数字 浮点数
                 {"field_name": '日期', "type": 5},  # 日期
             ]
             mode_feishu.create_table_fields_test(fapp_name, fapp_token, 'tblJyCmlB0Ly6yvr', field_update)
 
         """
         url = f'{mode_feishu.feishu_app_url}{app_token}/tables/{table_id}/fields'
         for i in field_update:
@@ -3556,14 +3558,96 @@
             data_dict['owner'] = owner
             data_dict['mp_tk'] = mp_tk
             data_dict['campaign_id'] = campaign_id
 
             data_list.append(data_dict)
         return data_list
 
+    # 本地地址
+    @classmethod
+    def loc_ip(cls):
+        hostname = socket.gethostname()
+        ip_list = []
+        # 获取IP地址信息
+        addr_infos = socket.getaddrinfo(hostname, None)
+        for addr in addr_infos:
+            ip_list.append(addr[4][0])
+        return ip_list
+
+    # 公网ip
+    @classmethod
+    def public_ip(cls):
+        return requests.get(r'https://jsonip.com').json()
+
+    # 错误推送
+    def err_log(self, func, p=4, err_times=3, sleep=30, err_msg="err!!!", save_mysql=0):
+        """
+        import inspect
+        func_info = inspect.getframeinfo(inspect.currentframe())
+        mode_pro.err_log(func_info, p=5, err_msg="这个错误啊!!!", err_times=1, sleep=10, save_mysql=1)
+
+            如果函数发生错误，需要发送推送信息
+                规则：
+                    1.两次推送的间要有休眠时间 sleep
+                    2.推送包含 错误等级p 错误信息 错误位置
+                    3.要有错误阈值err_times，错误n次后再推送
+
+            p等级 0-5 越小越紧急
+            - 0  服务器挂了
+            - 1  高度重视
+            - 2  中等错误
+            - 3  小错误
+            - 4  日常错误
+            - 5  except 抛出
+
+            err_times 错误次数 1-100000次
+        """
+
+        func_name = func.function
+        func_filename = func.filename
+        func_lineno = func.lineno
+
+        # 错误唯一标志
+        v = 'v11132sd'
+        key = f"err_log_{v}_{mode_pros.md5_base(f'{func_name}_{func_filename}_{func_lineno}')}"
+        key_send = f"err_send_{v}_{mode_pros.md5_base(f'{func_name}_{func_filename}_{func_lineno}')}"
+
+        def send(this_err_count):
+            mode_feishu.feishu_send_message(f"""err {p}
+        错误信息：{err_msg}
+        错误次数：{this_err_count}
+        错误函数：{func_name}
+        错误位置：{func_filename}
+        错误行数：{func_lineno}""")
+
+        err_cache = cache_get(key)
+        if err_cache:
+            err_count = err_cache['err_count'] + 1
+            cache_set(key, {'err_count': err_cache['err_count'] + 1})
+        else:
+            err_count = 1
+            cache_set(key, {'err_count': err_count})
+
+        if err_count >= err_times:
+            err_send_cache = cache_get(key_send)
+            if not err_send_cache:
+                send(err_count)
+                cache_set(key_send, 1, sleep)
+
+                # 存储mysql
+                mode_pro.mysql_db(method='iss', table='cd_err_log_python', save_data=[{
+                    'p': p,
+                    'err_msg': err_msg,
+                    'err_count': err_count,
+                    'func_name': func_name,
+                    'func_filename': func_filename,
+                    'func_lineno': func_lineno,
+                    'create_time': int(time.time()),
+                }])
+
 
 # cos
 class Cos:
 
     def __init__(self, **kwargs):
         # 选择服务器
         server_select = kwargs.get("server_select", 'jike')
@@ -3622,14 +3706,441 @@
                 Method='GET',
             )
             return download_url
         except Exception as E:
             print('Fr包err cnd获取路径失败', E)
 
 
+# FastGpt
+class FastGptAuto:
+
+    def __init__(self, **kwargs):
+        self.conn_tp = kwargs.get('conn_tp', 1)  # 2测试
+        self.avatar = "/icon/logo.svg"
+        self.base_url = 'https://aitest.dso100.com/api'
+        self.authorization = 'fastgpt-nE4z8uvJrrh5N1OvvdjDFG7Y055Rj9xVVXKeVSghM1cFAr1zXRUMdxm5v7a6pC'
+
+        self.user_text_table = 'cd_douyin_user_video_text'
+        self.es_user_text_table = 'douyin_user_video_text'
+        self.all_dataset_table = 'cd_fast_article_dataset'
+
+    # 通过后台生成的token https://aitest.dso100.com/account?currentTab=apikey
+    def get_header(self):
+        return {
+            'Authorization': f'Bearer {self.authorization}',
+            'user-agent': config_dict['base_ua'],
+        }
+
+    # 通过登录获取的token
+    def get_token_header(self, refresh=0):
+        key = 'fastgpt_token_v1'
+        token = cache_get(key)
+        if not token or refresh == 1:
+            url = f'{self.base_url}/support/user/account/loginByPassword'
+            data = {"username": "root", "password": "45d257ac8225ef3436843c66083736af23a24e7fd63a57f712e60e19c39248be"}
+            res = requests.post(url=url, json=data)
+            token = res.json()['data']['token']
+            cache_set(key, token, 3600)
+        return {
+            'cookie': f'token={token}',
+            'user-agent': config_dict['base_ua'],
+        }
+
+    # app list
+    def lit(self):
+        response = requests.get(f'{self.base_url}/core/app/list', headers=self.get_token_header())
+        print(response.json())
+
+    # 应用 创建
+    def app_create(self):
+        import json_data_fastgpt
+        member_id = 15315
+        response = requests.post(f'{self.base_url}/core/app/create', headers=self.get_token_header(),
+                                 json=json_data_fastgpt.json_app_create(member_id))
+        if response.status_code == 200:
+            data_data = response.json()
+            code = data_data['code']
+            if code == 200:
+                return data_data['data']
+
+    # 应用 修改 【知识库】 【提示词】
+    def app_update(self, app_id, dataset_id, cue_word):
+        import json_data_fastgpt
+        response = requests.post(f'{self.base_url}/core/app/update?appId={app_id}', headers=self.get_token_header(),
+                                 json=json_data_fastgpt.json_app_update(dataset_id, cue_word))
+        print(response.text)
+
+    # 知识库 创建
+    def dataset_create(self, dataset_name):
+        data = {
+            "parentId": None,
+            "type": "dataset",
+            "name": dataset_name,
+            "intro": '',
+            "avatar": self.avatar,
+            "vectorModel": "text-embedding-ada-002",
+            "agentModel": "gpt-3.5-turbo"
+        }
+        response = requests.post(f'{self.base_url}/core/dataset/create', headers=self.get_header(), json=data)
+        if response.status_code == 200:
+            data_data = response.json()
+            code = data_data['code']
+            if code == 200:
+                return data_data['data']
+
+    # 知识库 全部
+    def dataset_look_all(self):
+        t = 'fastgpt-4HuWTuvo4niPmg5myRqxRAJWrGwXzShJ1DSJyjRfUnjyULmK5Zp2iL3'
+        response = requests.get(f'{self.base_url}/core/dataset/list?parentId=', headers=self.get_header())
+        return response.json()
+
+    # 知识库 详情
+    def dataset_look_info(self, dataset_id):
+        response = requests.get(f'{self.base_url}/core/dataset/detail?id={dataset_id}', headers=self.get_header())
+        return response.json()
+
+    # 知识库 删除
+    def dataset_del(self, dataset_id):
+        response = requests.get(f'{self.base_url}/core/dataset/delete?id={dataset_id}', headers=self.get_header())
+        return response.json()
+
+    # 集合 创建
+    def collection_create(self, dataset_name, collection_name='测试'):
+        data = {
+            "datasetId": dataset_name,
+            "parentId": None,
+            "name": collection_name,
+            "type": "virtual",
+            "metadata": {
+                "test": 111
+            }
+        }
+        response = requests.post(f'{self.base_url}/core/dataset/collection/create', headers=self.get_header(),
+                                 json=data)
+        if response.status_code == 200:
+            data_data = response.json()
+            print(data_data)
+            code = data_data['code']
+            if code == 200:
+                return data_data['data']
+
+    # 知识库 集合 列表
+    def dataset_collection_list(self, dataset_id):
+        data = {
+            "pageNum": 1,
+            "pageSize": 100,
+            "datasetId": dataset_id,
+            "parentId": "",
+            "searchText": ""
+        }
+        response = requests.get(f'{self.base_url}/core/dataset/collection/list', headers=self.get_header(), json=data)
+        return response.json()
+
+    # 集合 纯文本集合
+    def collection_create_txt(self, dataset_name):
+        data = {
+            "text": "我喜欢踢足球",
+            "datasetId": dataset_name,
+            "parentId": None,
+            "name": "足球",
+
+            "trainingType": "qa",
+            "chunkSize": 8000,
+            "chunkSplitter": "",
+            "qaPrompt": "11",
+
+            "metadata": {}
+        }
+        response = requests.post(f'{self.base_url}/core/dataset/collection/create/text', headers=self.get_header(),
+                                 json=data)
+        if response.status_code == 200:
+            data_data = response.json()
+            print(data_data)
+            code = data_data['code']
+            if code == 200:
+                return data_data['data']
+
+    # 集合 添加数据
+    def collection_push_data(self, collection_id, push_data):
+        """
+            [
+                {
+                    "q": "文本文本文本文本文本",
+                    "a": ""
+                },
+            ]
+        """
+        # 每次添加50个
+        err = 0
+        split_push_data = mode_data.list_avg_split(push_data, 50)
+        for each_push_data in split_push_data:
+            time.sleep(1)
+            data = {
+                "collectionId": collection_id,
+                "trainingMode": "chunk",
+                "prompt": "",
+                "billId": "",
+                "data": each_push_data
+            }
+            try:
+                response = requests.post(f'{self.base_url}/core/dataset/data/pushData', headers=self.get_header(),
+                                         json=data)
+                if response.status_code == 200:
+                    data_data = response.json()
+                    code = data_data['code']
+                    if code != 200:
+                        err = 1
+                else:
+                    err = 1
+            except:
+                err = 1
+
+        return err
+
+    # 时间转换
+    def time_frame_stamp(self, time_frame, create_time):
+        """
+            [time_frame,create_time]
+        """
+        if time_frame == '6个月':
+            return create_time - 86400 * 31 * 6  # 六个月前时间戳
+        elif time_frame == '1年':
+            return create_time - 86400 * 366  # 1年前前时间戳
+        elif time_frame == '全部':
+            return 0  # 全部时间戳
+        else:
+            return create_time - 86400 * 31 * 3  # 三个月前时间戳
+
+    # 上传
+    def up(self):
+
+        import requests
+
+        # 定义目标 URL
+        url = 'https://aitest.dso100.com/api/common/file/upload'
+
+        # 定义请求头
+        headers = {
+            'accept': 'application/json, text/plain, */*',
+            'accept-language': 'zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6',
+            'content-type': 'multipart/form-data; boundary=----WebKitFormBoundarys9RAEXfISllHiC8p',
+            'cookie': 'Hm_lvt_a65de9750f8989adcf4af692ae366a3f=1712413671,1713143431,1713332672,1713422297; token=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI2NjIwYjQzYzNmOTAxYjQyZmNlN2NjNjEiLCJ0ZWFtSWQiOiI2NjIwYjQzYzNmOTAxYjQyZmNlN2NjNjQiLCJ0bWJJZCI6IjY2MjBiNDNjM2Y5MDFiNDJmY2U3Y2M2NiIsImV4cCI6MTcxNDIwMTA4MCwiaWF0IjoxNzEzNTk2MjgwfQ.hq0BaQhwtGyy1uLBOTZxUdC_k3Q7XMkTTTcGLrEHqao; Hm_lpvt_a65de9750f8989adcf4af692ae366a3f=1713601305',
+            'origin': 'https://aitest.dso100.com',
+            'referer': 'https://aitest.dso100.com/dataset/detail?datasetId=662381dd3f901b42fce7f8d6&parentId=&currentTab=import&source=csvTable',
+            'sec-ch-ua': '"Microsoft Edge";v="123", "Not:A-Brand";v="8", "Chromium";v="123"',
+            'sec-ch-ua-mobile': '?0',
+            'sec-ch-ua-platform': '"Windows"',
+            'sec-fetch-dest': 'empty',
+            'sec-fetch-mode': 'cors',
+            'sec-fetch-site': 'same-origin',
+            'token': 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI2NjIwYjQzYzNmOTAxYjQyZmNlN2NjNjEiLCJ0ZWFtSWQiOiI2NjIwYjQzYzNmOTAxYjQyZmNlN2NjNjQiLCJ0bWJJZCI6IjY2MjBiNDNjM2Y5MDFiNDJmY2U3Y2M2NiIsImV4cCI6MTcxNDIwMTA4MCwiaWF0IjoxNzEzNTk2MjgwfQ.hq0BaQhwtGyy1uLBOTZxUdC_k3Q7XMkTTTcGLrEHqao',
+            'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36 Edg/123.0.0.0',
+        }
+
+        # 定义文件路径
+        file_path = 'test_data.csv'
+
+        # 以二进制读取文件内容
+        with open(file_path, 'rb') as file:
+            # 构建文件对象
+            files = {'file': file}
+
+            # # 定义表单数据
+            # data = {
+            #     'metadata': {},
+            #     'bucketName': 'dataset',
+            # }
+
+            # 发送 POST 请求，同时上传文件和表单数据
+            response = requests.post(url, headers=headers, files=files)
+
+        print(response.text)
+
+    def te(self):
+
+        # # 定义目标 URL
+        # url = f'{self.base_url}/core/dataset/collection/create/file'
+        #
+        # # 定义文件路径
+        # file_path = 'C:/Users/30844\Documents\project_all\python_project\mofan\gy_pyhton_project/all_project/ai_fastgpt/fastgpt_mode.py'
+        #
+        # # 定义表单数据
+        # data = {"datasetId": "662377893f901b42fce7f115", "parentId": None, "trainingType": "chunk", "chunkSize": 512,
+        #         "chunkSplitter": "", "qaPrompt": "", "metadata": {}}
+        #
+        # # 以二进制读取文件内容
+        # with open(file_path, 'rb') as file:
+        #     # 构建文件对象
+        #     files = {'file': file}
+        #
+        #     # 发送 POST 请求，同时上传文件和表单数据
+        #     response = requests.post(url, headers=self.get_header(), files=files, json=data)
+        #
+        # # 检查响应状态码
+        # print(response.text)
+
+        url = 'https://aitest.dso100.com/api/core/dataset/collection/create/csvTable'
+        data = {
+            "parentId": "",
+            "trainingType": "chunk",
+            "datasetId": "662381dd3f901b42fce7f8d6",
+            "chunkSize": 700,
+            "chunkSplitter": "",
+            "qaPrompt": "<Context></Context> 标记中是一段文本，学习和分析它，并整理学习成果：\n- 提出问题并给出每个问题的答案。\n- 答案需详细完整，尽可能保留原文描述。\n- 答案可以包含普通文字、链接、代码、表格、公示、媒体链接等 Markdown 元素。\n- 最多提出 30 个问题。\n",
+            "name": "聚法帮法律咨询_2024-04-20 14_04_23.csv",
+            "fileId": "662380773f901b42fce7f6e7"
+        }
+        response = requests.post(url, headers=self.get_header(), json=data)
+        print(response.text)
+
+    def api_1(self):
+        headers = {
+            'Authorization': 'Bearer fastgpt-Qas3mebW6La0aYczKyoFWMPMM36oG7OMZVMZnq9cnMwfU2Y79FcQ4s',
+            'Content-Type': 'application/json',
+        }
+
+        data = {
+            "chatId": "662394053f901b42fce8005a",
+            "stream": False,
+            "detail": False,
+            "messages": [
+                {
+                    "content": "导演是谁",
+                    "role": "user"
+                }
+            ]
+        }
+        response = requests.post('https://aitest.dso100.com/api/v1/chat/completions', headers=headers, json=data)
+        print(response.text)
+
+        # headers = {
+        #     'Authorization': 'Bearer fastgpt-MdBia1If20J3gKnrHHzHOnNUg4a53FQU8dGEure6QaVK8gJXa5d9VB2Dy',
+        #     'Content-Type': 'application/json',
+        # }
+        #
+        # data = {
+        #     "chatId": "6620b4b13f901b42fce7ccc1",
+        #     "stream": False,
+        #     "detail": False,
+        #     "messages": [
+        #         {
+        #             "content": "导演是谁",
+        #             "role": "user"
+        #         }
+        #     ]
+        # }
+        # response = requests.get('https://aitest.dso100.com/api/core/app/list', headers=headers)
+        # print(response.text)
+
+    # 整合 创建知识库—>
+    def func_create_dataset(self, dataset_name, push_data, save_info):
+        # 根据用户创建知识库
+        dataset_id = self.dataset_create(dataset_name)
+
+        # 增加数据集
+        collection_id = self.collection_create(dataset_id, '抖音文案')
+
+        # 添加数据
+        err = self.collection_push_data(collection_id, push_data)
+        if err:
+            fi = inspect.getframeinfo(inspect.currentframe())
+            mode_pro.err_log(fi, p=5, err_msg=f"创建知识库err，{dataset_name}", err_times=1, sleep=10, save_mysql=1)
+        else:
+            print("创建知识库成功")
+
+            # 标记
+            mode_pro.mysql_db(method='up', table=self.user_text_table, conn_tp=self.conn_tp, save_data=[{
+                'to_dataset': 1,
+                'id': save_info[0],
+            }])
+
+            # 新增知识库
+            mode_pro.mysql_db(method='iss', table=self.all_dataset_table, conn_tp=self.conn_tp, save_data=[{
+                'platform': 'douyin',
+                'user_id': save_info[1],
+                'sec_uid': save_info[2],
+                'nickname': save_info[3],
+                'time_frame_video_count': save_info[6],
+                'time_frame': save_info[5],
+                'text_create_time': save_info[4],
+                'is_upload': 0,
+                'create_time': int(time.time()),
+                'dataset_name': dataset_name,
+                'dataset_id': dataset_id,
+                'collection_id': collection_id,
+            }])
+
+    # 计划任务 达人文案库 -> 知识库
+    def user_text_to_dataset(self):
+        sql = (f'SELECT id,user_id,sec_uid,nickname,create_time,time_frame,time_frame_video_count'
+               f' FROM {self.user_text_table} WHERE to_dataset = 0 and `state` = 1 limit 1')  # to_dataset=0|1
+        all_data = mode_pro.mysql_db(method='s', table=self.user_text_table, sql=sql, conn_tp=self.conn_tp)
+        for i in all_data:
+            print(i)
+            id_id = i[0]
+            user_id = i[1]
+            sec_uid = i[2]
+            nickname = i[3]
+            create_time = i[4]
+            time_frame = i[5]
+            time_frame_video_count = i[6]
+
+            tf_stamp = self.time_frame_stamp(time_frame, create_time)
+            # 时间范围 视频
+            query = {
+                "bool": {
+                    "must": [
+                        {"match": {"sec_uid": sec_uid}},
+                        {"match": {"aweme_type": 0}},
+                        {"range": {"create_time": {"gte": tf_stamp}}},
+                        {"range": {"create_time": {"lte": create_time}}},
+                    ]
+                }
+            }
+            source = ['video_text']
+            data_data = mode_pro.es_search_new_20231215(table=self.es_user_text_table, query=query, _source=source,
+                                                        size=3000)
+
+            push_data = []  # 要添加知识库的文案
+            for v in data_data:
+                print(v)
+                data_info = v['_source']
+                push_data.append({
+                    "q": data_info.get('video_text', ''),
+                    "a": ""
+                })
+
+            # 创建知识库
+            self.func_create_dataset(dataset_name=nickname, push_data=push_data, save_info=i)
+
+    # 计划任务 判断知识库文案装填成功
+    def dataset_is_upload(self):
+        save_data = []
+        sql = f'SELECT id,dataset_id,collection_id FROM {self.all_dataset_table} where is_upload = 0'
+        all_data = mode_pro.mysql_db(method='s', table=self.all_dataset_table, sql=sql, conn_tp=self.conn_tp)
+        for i in all_data:
+            print(i)
+            id_id = i[0]
+            dataset_id = i[1]
+            collection_id = i[2]
+            data_info = self.dataset_collection_list(dataset_id)
+            c_list = data_info['data']['data']
+            for ci in c_list:
+                if ci['_id'] == collection_id:
+                    if ci['trainingAmount'] == 0:
+                        save_data.append({
+                            'is_upload': 1,
+                            'id': id_id
+                        })
+                        continue
+
+        if save_data:
+            mode_pro.mysql_db(method='up', table=self.all_dataset_table, conn_tp=self.conn_tp, save_data=save_data)
+
+
 # myself 高阳本人信息
 class MyGy:
 
     def __init__(self, **kwargs):
         self.fr1997_config_dict = cache_get("fr1997_config_dict")
 
     # 获取信息
@@ -3647,44 +4158,13 @@
 mode_text = TextJike()  # 文本处理
 mode_data = DataJike()  # 数据处理
 mode_spider = SpiderJike()  # 数据请求
 mode_django = DjangoJike()  # django配置
 mode_douyin = DouyinJike()  # douyin配置
 mode_pros = ModeStatic()  # 其它函数
 mode_cos = Cos()  # cos
+mode_fastgpt = FastGptAuto()  # fastgpt
 mode_fr_cos = Cos(server_select='personal')  # cos 高阳
 mode_myself = MyGy()
 
 mode_pro = ModeFunc()  # main
 
-# fapp_name = 'jike_app'
-# fapp_token = 'ZOO2bktVDa1OOSsRGvCcJkXLn0b'
-# ftable_id = 'tblCevQUyQAvY4nv'
-# fview_id = 'vewe2KRJqs'
-# fields = mode_feishu.create_new_table(fapp_name, fapp_token, '群响-每日统计')
-
-
-# mode_feishu.create_table_and_fields(fapp_name, fapp_token, '群响-每日统计', dct=1)
-
-# fields_create = [
-#     {"field_name": '日期', "type": 5},  # 日期
-#     {"field_name": '手机', "type": 1},  # 添加普通文本
-#     {"field_name": '添加时间', "type": 5, "property": {"date_formatter": "yyyy/MM/dd HH:mm", "auto_fill": False}},  # 日期
-#     {"field_name": '备注', "type": 1},  # 添加普通文本
-#     {"field_name": '微信姓名', "type": 1},  # 添加普通文本
-#     {"field_name": '添加者', "type": 1},  # 添加普通文本
-#     {"field_name": '通过状态', "type": 1},  # 添加普通文本
-#     {"field_name": '加好友备注', "type": 1},  # 添加普通文本
-# ]
-# mode_feishu.create_table_and_fields(fapp_name, fapp_token, '群响-用户列表', dct=1, fields_create=fields_create)
-
-# add_data = [
-#     {
-#         "日期": int(time.time()) * 1000,
-#         "加好友次数": 1,
-#     }, {
-#         "日期": int(time.time()) * 1000,
-#         "加好友次数": 2,
-#     }
-# ]
-#
-# mode_feishu.add_more_view(fapp_name, fapp_token, 'tbloDwXrLC4Jz0be', add_data)
```

