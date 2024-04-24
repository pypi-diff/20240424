# Comparing `tmp/pyneople-0.2.4.tar.gz` & `tmp/pyneople-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneople-0.2.4.tar", last modified: Wed Apr 24 12:54:41 2024, max compression
+gzip compressed data, was "pyneople-0.2.5.tar", last modified: Wed Apr 24 14:18:18 2024, max compression
```

## Comparing `pyneople-0.2.4.tar` & `pyneople-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:54:41.292426 pyneople-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-24 12:54:30.000000 pyneople-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-24 12:54:41.292426 pyneople-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-24 12:54:30.000000 pyneople-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 12:54:30.000000 pyneople-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 12:54:41.292426 pyneople-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-24 12:54:30.000000 pyneople-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:54:41.288426 pyneople-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:54:41.288426 pyneople-0.2.4/src/pyneople/
--rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-04-24 12:54:30.000000 pyneople-0.2.4/src/pyneople/METADATA.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 12:54:30.000000 pyneople-0.2.4/src/pyneople/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33657 2024-04-24 12:54:30.000000 pyneople-0.2.4/src/pyneople/character.py
--rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-04-24 12:54:30.000000 pyneople-0.2.4/src/pyneople/database_connecter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-04-24 12:54:30.000000 pyneople-0.2.4/src/pyneople/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:54:41.292426 pyneople-0.2.4/src/pyneople.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-24 12:54:41.000000 pyneople-0.2.4/src/pyneople.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-24 12:54:41.000000 pyneople-0.2.4/src/pyneople.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:54:41.000000 pyneople-0.2.4/src/pyneople.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 12:54:41.000000 pyneople-0.2.4/src/pyneople.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:18.928583 pyneople-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-24 14:18:08.000000 pyneople-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-24 14:18:18.928583 pyneople-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-24 14:18:08.000000 pyneople-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 14:18:08.000000 pyneople-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:18:18.928583 pyneople-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-24 14:18:08.000000 pyneople-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:18.924583 pyneople-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:18.928583 pyneople-0.2.5/src/pyneople/
+-rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-04-24 14:18:08.000000 pyneople-0.2.5/src/pyneople/METADATA.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 14:18:08.000000 pyneople-0.2.5/src/pyneople/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34094 2024-04-24 14:18:08.000000 pyneople-0.2.5/src/pyneople/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-04-24 14:18:08.000000 pyneople-0.2.5/src/pyneople/database_connecter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-04-24 14:18:08.000000 pyneople-0.2.5/src/pyneople/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:18.928583 pyneople-0.2.5/src/pyneople.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-24 14:18:18.000000 pyneople-0.2.5/src/pyneople.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-24 14:18:18.000000 pyneople-0.2.5/src/pyneople.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:18:18.000000 pyneople-0.2.5/src/pyneople.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 14:18:18.000000 pyneople-0.2.5/src/pyneople.egg-info/top_level.txt
```

### Comparing `pyneople-0.2.4/LICENSE` & `pyneople-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.4/PKG-INFO` & `pyneople-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.2.4
+Version: 0.2.5
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/pyneople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/pyneople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneople-0.2.4/setup.py` & `pyneople-0.2.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyneople",
-    version="0.2.4",
+    version="0.2.5",
     author="ippo252525",
     author_email="ippo252525@gmail.com",
     description="Neople Open API wrapper for data analyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ippo252525/pyneople",
     project_urls={
```

### Comparing `pyneople-0.2.4/src/pyneople/METADATA.py` & `pyneople-0.2.5/src/pyneople/METADATA.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.4/src/pyneople/character.py` & `pyneople-0.2.5/src/pyneople/character.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,16 +52,15 @@
         # 한글 서버명을 영문 서버명으로 변환, 영문 서버명은 그대로 입력, 그 외의 입력은 에러 발생
         if arg_server_name in SERVER_NAME_2_ID.keys():
             arg_server_name = SERVER_NAME_2_ID[arg_server_name]
         elif arg_server_name in SERVER_NAME_2_ID.values():
             pass
         else:
             raise ValueError("서버 이름을 확인하시오")
-
-        
+        self._server_id = arg_server_name
         url = f"https://api.neople.co.kr/df/servers/{arg_server_name}/characters?characterName={urllib.parse.quote(arg_character_name)}&limit=1&apikey={self._api_key}"
         
         # parse_data에 매개변수로 사용 될 것을 생각해서 dict를 받을 수 있도록 정보 다듬어서 제공
         try:
             return get_request(url).get("rows")[0]
         except IndexError:
             return dict()
@@ -90,17 +89,17 @@
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 기본 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
                 arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
         """    
+        self._server_id = arg_server_id
         url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}?apikey={self._api_key}"
-
-        return get_request(url)        
+        return get_request(url)
     
     def parse_data(self, arg_data : dict, attribute_list : Iterable[str] = CHARACTER_INFORMATION_NAME.keys()):
         """
         데이터를 정리해서 하위 속성에 저장
             Args :
                 arg_data(dict) : Neople Open API 를 통해 받은 data
                 attribute_list(iterable of str) : 원하는 하위 속성 명
@@ -142,14 +141,15 @@
                 
                 arg_limit(int) : 한번 request할 때 수집 할 타임라인 데이터의 개수
                 
                 arg_code(int) : 수집하고 싶은 타임라인 코드 ex)201, 202 참조) https://developers.neople.co.kr/contents/guide/pages/all 
                 
                 arg_print_log(boolean) : 데이터 수집의 과정의 print 여부   
         """
+        self._server_id = arg_server_id
         timeline = []
         
         end_date = datetime.datetime.strptime(arg_end_date, '%Y-%m-%d %H:%M')
         start_date = end_date - datetime.timedelta(days=90)
         if start_date < datetime.datetime.strptime(arg_last_end_date, '%Y-%m-%d %H:%M'):
             start_date = datetime.datetime.strptime(arg_last_end_date, '%Y-%m-%d %H:%M')
         next = ""
@@ -203,18 +203,17 @@
         """
         캐릭터의 모험단명부터 명성 등 정보를 반환한다
             Args:
                 arg_server_id(str) :  서버 ID
                 
                 arg_character_id(str) : 캐릭터 ID
         """
-
+        self._server_id = arg_server_id
         url = f'https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/status?apikey={self._api_key}'
         return get_request(url)
-        
     def parse_data(self, arg_data : dict, attribute_list : Iterable[str] = STATUS_NAME.keys()):
         """
         데이터를 정리해서 하위 attribute에 저장
             Args :
                 arg_data(dict) : Neople Open API 를 통해 받은 data
                 attribute_list(iterable of str) : 원하는 하위 속성 명
         """
@@ -367,14 +366,15 @@
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 장착 장비 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
                 arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
         """        
+        self._server_id = arg_server_id
         url = f'https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/equipment?apikey={self._api_key}'
         return get_request(url)
 
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 attribute에 저장
             Args :
@@ -447,14 +447,15 @@
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 장착 아바타 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
                 arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
         """        
+        self._server_id = arg_server_id
         url = f'https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/avatar?apikey={self._api_key}'
         return get_request(url)
 
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 attribute에 저장
             Args :
@@ -484,14 +485,15 @@
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 장착 크리쳐 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
                 arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
         """
+        self._server_id = arg_server_id
         url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/creature?apikey={self._api_key}"
         return get_request(url)
     
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 attribute에 저장
             Args :
@@ -511,14 +513,15 @@
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 장착 휘장 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
                 arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
         """        
+        self._server_id = arg_server_id
         url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/flag?apikey={self._api_key}"
         return get_request(url)
     
     def parse_data(self, arg_data):
         """
         데이터를 정리해서 하위 attribute에 저장
             Args :
@@ -559,14 +562,15 @@
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 장착 탈리스만 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
                 arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
         """                
+        self._server_id = arg_server_id
         url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/talisman?apikey={self._api_key}"         
         return get_request(url)
     
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 attribute에 저장
             Args :
@@ -589,14 +593,15 @@
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 장비 특성 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
                 arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
         """                
+        self._server_id = arg_server_id
         url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/equipment-trait?apikey={self._api_key}"
         return get_request(url)
     
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 attribute에 저장
         강력한 일격과 명상의 레벨만 확인
@@ -629,16 +634,17 @@
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 스킬 스타일 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
                 arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
         """                
+        self._server_id = arg_server_id
         url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/skill/style?apikey={self._api_key}"
-        return get_request(url)                
+        return get_request(url)
 
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 attribute에 저장
         스킬 코드만 구현 완료 나머지 추후 개발
             Args :
                 arg_data(dict) : Neople Open API 를 통해 받은 data
@@ -690,14 +696,15 @@
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 버프 강화(장비, 아바타, 크리쳐) 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
                 arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
         """   
+        self._server_id = arg_server_id
         buff_info_dict = {}     
         buff_equipment_data = get_request(f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/skill/buff/equip/equipment?apikey={self._api_key}")
         buff_avatar_data = get_request(f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/skill/buff/equip/avatar?apikey={self._api_key}")
         buff_creature_data = get_request(f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/skill/buff/equip/creature?apikey={self._api_key}")
         buff_info_dict["equipment"] = buff_equipment_data
         buff_info_dict["avatar"] = buff_avatar_data
         buff_info_dict["creature"] = buff_creature_data
```

### Comparing `pyneople-0.2.4/src/pyneople/database_connecter.py` & `pyneople-0.2.5/src/pyneople/database_connecter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from .character import CharacterFame, CharacterSearch
-from .functions import get_request
+from .functions import get_request, ServerMaintenanceError, PyneopleError
 from multiprocessing import Process, Queue, Value
 from pymongo import MongoClient
 import time
 import psycopg2
 from psycopg2 import sql
 
 def store_data_to_mongodb(
         arg_mongo_client_instance : MongoClient,
         arg_database_name : str,
         arg_collection_name : str,
-        character_fame_instance_list : list[CharacterFame],
+        arg_api_key_list : list[str],
         arg_character_search_instance : CharacterSearch,
         arg_max_fame : int):
     # start_time = time.time()
     
     def task_get_request(id, character_fame_instance, args_queue, data_queue, completed_tasks_count, tasks_to_be_completed_count):
         while completed_tasks_count.value != tasks_to_be_completed_count:
             if not args_queue.empty():
                 args_dict = args_queue.get()
                 try:
                     data = character_fame_instance.get_data(**args_dict)
-                    print("task get request")
+                    print("task get request", end="\r")
                     data_queue.put(data)
+                except ServerMaintenanceError:
+                    raise Exception("서버 점검중")
                 except:
                     args_queue.put(args_dict)
 
     def task_store_data(id, args_queue, data_queue, mongo_collection, completed_tasks_count, tasks_to_be_completed_count):                
         
         while completed_tasks_count.value != tasks_to_be_completed_count:
             if not data_queue.empty():
@@ -37,32 +39,32 @@
                     arg_character_search_instance.parse_data(data[0], ['fame', 'job_id', 'job_grow_id', 'job_grow_name'])
                     max_fame = arg_character_search_instance.fame
                     arg_character_search_instance.parse_data(data[-1], ['fame', 'job_id', 'job_grow_id', 'job_grow_name'])
                     min_fame = arg_character_search_instance.fame
                     job_id = arg_character_search_instance.job_id
                     job_grow_id = arg_character_search_instance.job_grow_id
                     job_grow_name = arg_character_search_instance.job_grow_name
-                    print(f"max = {max_fame}, min = {min_fame}, 직업 = {job_grow_name}")
+                    print(f"max = {max_fame}, min = {min_fame}, 직업 = {job_grow_name}", end="\r")
                     if max_fame == min_fame:
                         min_fame = max_fame - 1
                     if min_fame <= 0:
                         completed_tasks_count.value += 1
-                        print(f"완료된 직업 개수 {completed_tasks_count.value}")
+                        print(f"완료된 직업 개수 {completed_tasks_count.value}", end="\r")
                         continue                        
                     args_dict = {
                         'arg_min_fame' : 0,
                         'arg_max_fame' : min_fame,
                         'arg_job_id' : job_id,
                         'arg_job_grow_id' : job_grow_id,
                         'arg_is_all_job_grow' : True
                     }
                     args_queue.put(args_dict)
                 else:
                     completed_tasks_count.value += 1
-                    print(f"완료된 직업 개수 {completed_tasks_count.value}")
+                    print(f"완료된 직업 개수 {completed_tasks_count.value}", end="\r")
                     continue                
 
     
     database = arg_mongo_client_instance[arg_database_name]
     collection = database[arg_collection_name]
     data = get_request(f"https://api.neople.co.kr/df/jobs?apikey={getattr(arg_character_search_instance, '_api_key')}")
     data = data['rows']
@@ -71,15 +73,16 @@
         for job_grow in job['rows']:
             job_id_list.append((job['jobId'], job_grow['jobGrowId'], job['jobName'], job_grow['jobGrowName']))
     tasks_to_be_completed_count = len(job_id_list)
     data_queue = Queue()
     args_queue = Queue()
     completed_tasks_count = Value("i", 0)          
     processes = []  
-    for character_fame_instance in character_fame_instance_list:
+    for api_key in arg_api_key_list:
+        character_fame_instance = CharacterFame(api_key)
         process = Process(target=task_get_request, args=(1, character_fame_instance, args_queue, data_queue, completed_tasks_count, tasks_to_be_completed_count))
         processes.append(process)
     process = Process(target=task_store_data, args=(2, args_queue, data_queue, collection, completed_tasks_count, tasks_to_be_completed_count))
     processes.append(process)
     for process in processes:
         process.start()
     
@@ -91,114 +94,112 @@
             'arg_job_id' : job_id,
             'arg_job_grow_id' : job_grow_id,
             'arg_is_all_job_grow' : True
         }
         args_queue.put(args_dict)        
 
     for process in processes:
-        process.join()                
-    # end_time = time.time()
-    # print(end_time - start_time)                    
+        process.join()           
                 
-                
-
-def execute(arg_connection, arg_sql : str):
-    '''
-    database에 connection 생성 후 sql문을 실행시키고 commit까지 완료 시키는 함수
-        Args:
-            arg_sql(str) : 실행되어야 하는 sql문
-    '''
+class PostgreSQLConnecter():
     
-    with arg_connection.cursor() as cursor:
-        cursor.execute(arg_sql)
-        arg_connection.commit()
-
-
-def fetch(arg_connection, arg_query : str):
-    '''
-    query문을 실행시켜 나오는 결과를 반환한다.
-        Args:
-            arg_query(str) : 실행되어야 하는 query문
-    '''
-
-    with arg_connection.cursor() as cursor:
-        cursor.execute(arg_query)
-        return cursor.fetchall()
-
-
-def create_table(arg_connection, arg_table_name : str, arg_columns : list, arg_drop : bool = False):
-    """
-    table을 만드는 함수
-        Args:
-            arg_table_name(str) : 생성하려는 table name
-            
-            arg_columns(list) : CREATE TABLE {table_name} (); 안에들어가는 문자열 list ex ["characterId VARCHAR(32) PRIMARY KEY", "serverId VARCHAR(32) NOT NULL"]
-            
-            arg_drop(bool) : {False : 이미 동일한 이름의 table이 있으면 에러발생(default), 
-                              True : 이미 동일한 이름의 table이 있으면 삭제하고 만든다}
-    """    
-    columns_str = ', '.join(arg_columns)
-    if arg_drop :
-        execute(arg_connection, f"DROP TABLE IF EXISTS {arg_table_name};")
-        execute(arg_connection, f"CREATE TABLE {arg_table_name} ({columns_str});")
-    else :
-        execute(arg_connection, f"CREATE TABLE {arg_table_name} ({columns_str});")
-
-
-def get_column_names(arg_connection, arg_table_name : str):
-    """
-    해당 table의 column 들의 이름을 list로 반환하는 함수
-        Args:
-            arg_table_name(str) : 확인하려는 table 이름
-    """
-    with arg_connection.cursor() as cursor:
-        cursor.execute(f"Select * FROM {arg_table_name} LIMIT 0")
-        column_names = [desc[0] for desc in cursor.description]
-        return column_names    
-
-
-def get_table_name_list(arg_connection):
-    '''
-    해당 데이터베이스의 table 이름의 list를 반환하는 함수
-    '''
-    data = fetch(arg_connection, 
-    """
-    SELECT
-        table_schema || '.' || table_name
-    FROM
-        information_schema.tables
-    WHERE
-        table_type = 'BASE TABLE'
-    AND
-        table_schema NOT IN ('pg_catalog', 'information_schema');
-    """
-    )            
-    table_name_list = [table_name[0].split(".")[1] for table_name in data]
-    return table_name_list
-
-
-def insert_into_table(arg_cursor , arg_table_name : str, arg_columns : list, arg_data : list, arg_ignore_duplication : bool = True):
-    """
-    table에 데이터를 삽입하는 함수
-        Args:
-            arg_cursor(cursor) : psycopg2 cursor 객체
-            arg_table_name(str) : 데이터를 삽입하려는 table name
-            arg_columns(list) : 데이터를 삽입하려는 column들의 list ex) ["characterId", "serverId", "jobName"]
-            arg_data(list) : ex [('f2baddf4a296490a4d463cb512a83789', 'anton', '총검사'),
-                                 ('87cbd3e834ae89c567a22a98bb2c9911', 'anton', '총검사')]
-                                 or
-                                 [('f2baddf4a296490a4d463cb512a83789', 'anton', '총검사')] <- data 1개여도 이런식으로 삽입
-            arg_ignore_duplication(bool) : {True : 중복되는게 있으면 해당 항목만 넘어가고 계속 저장해라, False : 중복되는게 있으면 에러를 발생시켜라}
-
-    주의사항 : 해당 함수는 connectiom.commit() 을 실행하지 않음
-    """
-    # 데이터를 삽입하기
-    # duplication_dict = {True : "ON CONFLICT DO NOTHING", False : ""}
-    
-    insert_query = sql.SQL("INSERT INTO {} ({}) VALUES {}").format(
-        sql.Identifier(arg_table_name),
-        sql.SQL(', ').join(map(sql.Identifier, arg_columns)),
-        sql.SQL(', ').join(map(sql.Literal, arg_data))
-        )
-    if arg_ignore_duplication:
-        insert_query += sql.SQL(" ON CONFLICT DO NOTHING") 
-    arg_cursor.execute(insert_query)                    
+    def __init__(self, arg_database_connection_dict : dict):
+        self.connection = psycopg2.connect(**arg_database_connection_dict)
+
+    def execute(self, arg_sql : str):
+        '''
+        sql문을 실행시키고 commit까지 완료 시키는 함수
+            Args:
+                arg_sql(str) : 실행되어야 하는 sql문
+        '''
+        
+        with self.connection.cursor() as cursor:
+            cursor.execute(arg_sql)
+            self.connection.commit()
+
+
+    def fetch(self, arg_query : str):
+        '''
+        query문을 실행시켜 나오는 결과를 반환한다.
+            Args:
+                arg_query(str) : 실행되어야 하는 query문
+        '''
+
+        with self.connection.cursor() as cursor:
+            cursor.execute(arg_query)
+            return cursor.fetchall()
+
+
+    def create_table(self, arg_table_name : str, arg_columns : list, arg_drop : bool = False):
+        """
+        table을 만드는 함수
+            Args:
+                arg_table_name(str) : 생성하려는 table name
+                
+                arg_columns(list) : CREATE TABLE {table_name} (); 안에들어가는 문자열 list ex ["characterId VARCHAR(32) PRIMARY KEY", "serverId VARCHAR(32) NOT NULL"]
+                
+                arg_drop(bool) : {False : 이미 동일한 이름의 table이 있으면 에러발생(default), 
+                                True : 이미 동일한 이름의 table이 있으면 삭제하고 만든다}
+        """    
+        columns_str = ', '.join(arg_columns)
+        if arg_drop :
+            self.execute(self, f"DROP TABLE IF EXISTS {arg_table_name};")
+            self.execute(self, f"CREATE TABLE {arg_table_name} ({columns_str});")
+        else :
+            self.execute(self, f"CREATE TABLE {arg_table_name} ({columns_str});")
+
+
+    def get_column_names(self, arg_table_name : str):
+        """
+        해당 table의 column 들의 이름을 list로 반환하는 함수
+            Args:
+                arg_table_name(str) : 확인하려는 table 이름
+        """
+        with self.connection.cursor() as cursor:
+            cursor.execute(f"Select * FROM {arg_table_name} LIMIT 0")
+            column_names = [desc[0] for desc in cursor.description]
+            return column_names    
+
+
+    def get_table_name_list(self):
+        '''
+        해당 데이터베이스의 table 이름의 list를 반환하는 함수
+        '''
+        data = self.fetch(self, 
+        """
+        SELECT
+            table_schema || '.' || table_name
+        FROM
+            information_schema.tables
+        WHERE
+            table_type = 'BASE TABLE'
+        AND
+            table_schema NOT IN ('pg_catalog', 'information_schema');
+        """
+        )            
+        table_name_list = [table_name[0].split(".")[1] for table_name in data]
+        return table_name_list
+
+
+    def insert_into_table(self, arg_cursor , arg_table_name : str, arg_columns : list, arg_data : list, arg_ignore_duplication : bool = True):
+        """
+        table에 데이터를 삽입하는 함수
+            Args:
+                arg_cursor(cursor) : psycopg2 cursor 객체
+                arg_table_name(str) : 데이터를 삽입하려는 table name
+                arg_columns(list) : 데이터를 삽입하려는 column들의 list ex) ["characterId", "serverId", "jobName"]
+                arg_data(list) : ex [('f2baddf4a296490a4d463cb512a83789', 'anton', '총검사'),
+                                    ('87cbd3e834ae89c567a22a98bb2c9911', 'anton', '총검사')]
+                                    or
+                                    [('f2baddf4a296490a4d463cb512a83789', 'anton', '총검사')] <- data 1개여도 이런식으로 삽입
+                arg_ignore_duplication(bool) : {True : 중복되는게 있으면 해당 항목만 넘어가고 계속 저장해라, False : 중복되는게 있으면 에러를 발생시켜라}
+
+        주의사항 : 해당 함수는 connectiom.commit() 을 실행하지 않음
+        """
+        insert_query = sql.SQL("INSERT INTO {} ({}) VALUES {}").format(
+            sql.Identifier(arg_table_name),
+            sql.SQL(', ').join(map(sql.Identifier, arg_columns)),
+            sql.SQL(', ').join(map(sql.Literal, arg_data))
+            )
+        if arg_ignore_duplication:
+            insert_query += sql.SQL(" ON CONFLICT DO NOTHING") 
+        arg_cursor.execute(insert_query)
```

### Comparing `pyneople-0.2.4/src/pyneople/functions.py` & `pyneople-0.2.5/src/pyneople/functions.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.4/src/pyneople.egg-info/PKG-INFO` & `pyneople-0.2.5/src/pyneople.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.2.4
+Version: 0.2.5
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/pyneople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/pyneople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

