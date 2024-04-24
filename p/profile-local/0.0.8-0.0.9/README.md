# Comparing `tmp/profile-local-0.0.8.tar.gz` & `tmp/profile-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profile-local-0.0.8.tar", last modified: Mon Sep  4 07:02:20 2023, max compression
+gzip compressed data, was "profile-local-0.0.9.tar", last modified: Mon Sep  4 10:55:38 2023, max compression
```

## Comparing `profile-local-0.0.8.tar` & `profile-local-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 07:02:20.364982 profile-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (999)      469 2023-09-04 07:02:20.364982 profile-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1008 2023-09-04 07:01:47.000000 profile-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 07:02:20.360982 profile-local-0.0.8/profile_local/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-04 07:01:47.000000 profile-local-0.0.8/profile_local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 07:02:20.364982 profile-local-0.0.8/profile_local/src/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-04 07:01:47.000000 profile-local-0.0.8/profile_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      824 2023-09-04 07:01:47.000000 profile-local-0.0.8/profile_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (999)     5898 2023-09-04 07:01:47.000000 profile-local-0.0.8/profile_local/src/generic_profile_insert.py
--rw-r--r--   0 runner    (1001) docker     (999)     9604 2023-09-04 07:01:47.000000 profile-local-0.0.8/profile_local/src/profiles_local.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 07:02:20.360982 profile-local-0.0.8/profile_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)      469 2023-09-04 07:02:20.000000 profile-local-0.0.8/profile_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      348 2023-09-04 07:02:20.000000 profile-local-0.0.8/profile_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-04 07:02:20.000000 profile-local-0.0.8/profile_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       14 2023-09-04 07:02:20.000000 profile-local-0.0.8/profile_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)      499 2023-09-04 07:01:47.000000 profile-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-04 07:02:20.364982 profile-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)      753 2023-09-04 07:01:47.000000 profile-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 10:55:38.903556 profile-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (999)      469 2023-09-04 10:55:38.899556 profile-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     1008 2023-09-04 10:55:12.000000 profile-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 10:55:38.899556 profile-local-0.0.9/profile_local/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-04 10:55:12.000000 profile-local-0.0.9/profile_local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 10:55:38.899556 profile-local-0.0.9/profile_local/src/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-04 10:55:12.000000 profile-local-0.0.9/profile_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      824 2023-09-04 10:55:12.000000 profile-local-0.0.9/profile_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5794 2023-09-04 10:55:12.000000 profile-local-0.0.9/profile_local/src/generic_profile_insert.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8565 2023-09-04 10:55:12.000000 profile-local-0.0.9/profile_local/src/profiles_local.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 10:55:38.899556 profile-local-0.0.9/profile_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)      469 2023-09-04 10:55:38.000000 profile-local-0.0.9/profile_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      348 2023-09-04 10:55:38.000000 profile-local-0.0.9/profile_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-04 10:55:38.000000 profile-local-0.0.9/profile_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       14 2023-09-04 10:55:38.000000 profile-local-0.0.9/profile_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      499 2023-09-04 10:55:12.000000 profile-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-04 10:55:38.903556 profile-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)      753 2023-09-04 10:55:12.000000 profile-local-0.0.9/setup.py
```

### Comparing `profile-local-0.0.8/README.md` & `profile-local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `profile-local-0.0.8/profile_local/src/constants.py` & `profile-local-0.0.9/profile_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `profile-local-0.0.8/profile_local/src/generic_profile_insert.py` & `profile-local-0.0.9/profile_local/src/generic_profile_insert.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,23 +11,25 @@
 from person_local_python_package.src.person import Person
 from reaction_local.src.reaction import Reaction
 from profile_reaction_local.src.profile_reaction import ProfileReactions
 from operational_hours_local.src.operational_hours import OperationalHours
 from dotenv import load_dotenv
 
 load_dotenv()
-#from user_context.src.user_context import UserContext # noqa: E402
+from user_context.src.user_context import UserContext # noqa: E402
 from logger_local.Logger import Logger  # noqa: E402
 
 logger = Logger.create_logger(object=OBJECT_TO_INSERT_CODE)
 
-TEST_PERSON_ID = 50050341 #Temporary until Person class is ready
-#TODO: change "en" to UserContext.get_cuurent_language() when UserContext is ready
-#def generic_profile_insert(profle_json: str, lang_code: str = UserContext.get_cuurent_language()):
-def generic_profile_insert(profle_json: str, lang_code: str = "en"):
+TEST_PERSON_ID = 50050341  # Temporary until Person class is ready
+
+UserContext.login()
+user_context_obj = UserContext()
+
+def generic_profile_insert(profle_json: str, lang_code: str = user_context_obj.get_curent_lang_code()):
     GENERIC_INSERT_METHOD_NAME = "generic_insert"
     logger.start(GENERIC_INSERT_METHOD_NAME, object={"profle_json": profle_json})
     data: Dict[str, any] = None
     try:
         data = json.loads(profle_json)
     except json.JSONDecodeError as e:
         logger.exception(GENERIC_INSERT_METHOD_NAME, object={"exception": e})
@@ -58,18 +60,18 @@
         # Insert person to db
         person_entry: Dict[str, any] = entry['person']
         gender_obj = Gender()
         gender_id = gender_obj.get_gender_id_by_title(person_entry.get('gender', None))
         person_data: Dict[str, any] = {
             'number': person_entry.get('number', None),
             'last_coordinate': person_entry.get('last_coordinate', None),
-            
+
         }
         # Person class has errors
-        person_id = TEST_PERSON_ID    #temporary for test
+        person_id = TEST_PERSON_ID  # temporary for test
         '''
         person_obj = Person()
         person_id = Person.insert(
             person_data.get('number', None),
             gender_id,
             person_data.get('last_coordinate', None),
             person_data.get('location_id', None))
@@ -116,8 +118,8 @@
 
         # Insert operational hours to db
         if "operational_hours" in entry:
             operational_hours = OperationalHours.create_hours_array(entry["operational_hours"])
             operational_hours_obj = OperationalHours()
             operational_hours_obj.insert(profile_id, location_id, operational_hours)
 
-    logger.end(GENERIC_INSERT_METHOD_NAME)
+    logger.end(GENERIC_INSERT_METHOD_NAME)
```

### Comparing `profile-local-0.0.8/profile_local/src/profiles_local.py` & `profile-local-0.0.9/profile_local/src/profiles_local.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         'rip': rip,                                     #Optional
         'gender_id': gender_id,                         #Optional
         'stars': stars,
         'last_dialog_workflow_state_id': last_dialog_workflow_state_id
     },
     profile_id: int
     '''
+
     def insert(self, person_id: int, data: Dict[str, any]) -> int:
         INSERT_PROFILE_METHOD_NAME = "insert_profile"
         logger.start(INSERT_PROFILE_METHOD_NAME, object=data)
 
         query_insert_profile_table = "INSERT INTO profile_table(`number`, user_id, person_id, is_main," \
             " visibility_id, is_approved, profile_type_id, preferred_lang_code, experience_years_min," \
             " main_phone_id, rip, gender_id, stars, last_dialog_workflow_state_id)" \
@@ -97,45 +98,39 @@
         'rip': rip,                                     #Optional
         'gender_id': gender_id,                         #Optional
         'stars': stars,
         'last_dialog_workflow_state_id': last_dialog_workflow_state_id
     }
     person_id: int                                      #Optional
     '''
-    def update(self, profile_id: int, data: Dict[str, any], person_id: int = None):
+
+    def update(self, profile_id: int, data: Dict[str, any]):
         UPDATE_PROFILE_METHOD_NAME = "update_profile"
         logger.start(UPDATE_PROFILE_METHOD_NAME, object={'profile_id': profile_id, 'data': data})
         query_update_profile_table: str = None
-        if person_id is not None:
-            query_update_profile_table = "UPDATE profile_table SET person_id = %s, user_id = %s, is_main = %s," \
-                " visibility_id = %s, is_approved = %s, profile_type_id = %s, preferred_lang_code = %s," \
-                " experience_years_min = %s, main_phone_id = %s, rip = %s, gender_id = %s, stars = %s," \
-                " last_dialog_workflow_state_id = %s WHERE profile_id = %s;"
-        else:
-            query_update_profile_table = "UPDATE profile_table SET user_id = %s, is_main = %s," \
-                " visibility_id = %s, is_approved = %s, profile_type_id = %s, preferred_lang_code = %s," \
-                " experience_years_min = %s, main_phone_id = %s, rip = %s, gender_id = %s, stars = %s," \
-                " last_dialog_workflow_state_id = %s WHERE profile_id = %s;"
+        query_update_profile_table = "UPDATE profile_table SET person_id = %s, user_id = %s, is_main = %s," \
+            " visibility_id = %s, is_approved = %s, profile_type_id = %s, preferred_lang_code = %s," \
+            " experience_years_min = %s, main_phone_id = %s, rip = %s, gender_id = %s, stars = %s," \
+            " last_dialog_workflow_state_id = %s WHERE profile_id = %s;"
         query_update_profile_ml_table = "UPDATE profile_ml_table SET lang_code = %s, `name` = %s, name_approved = %s WHERE profile_id = %s"
         data_to_update = (
+            data['person_id'],
             data['user_id'],
             data['is_main'],
             data['visibility_id'],
             data['is_approved'],
             data['profile_type_id'],
             data['preferred_lang_code'],
             data['experience_years_min'],
             data['main_phone_id'],
             data['rip'],
             data['gender_id'],
             data['stars'],
             data['last_dialog_workflow_state_id'],
             profile_id)
-        if person_id is not None:
-            data_to_update = (person_id,) + data_to_update
         self.cursor.execute(
             query_update_profile_table,
             (data_to_update))
         self.cursor.execute(
             query_update_profile_ml_table,
             (data['lang_code'],
              data['profile_name'],
@@ -167,26 +162,16 @@
             'is_approved': is_approved, 'profile_type_id': profile_type_id, 'preferred_lang_code': preferred_lang_code,
             'experience_years_min': experience_years_min, 'main_phone_id': main_phone_id, 'rip': rip,
             'gender_id': gender_id, 'stars': stars, 'last_dialog_workflow_state_id': last_dialog_workflow_state_id,
             'profile_ml_id': profile_ml_id, 'lang_code': lang_code, 'name': name, 'name_approved': name_approved}
         logger.end(READ_PROFILE_METHOD_NAME, object=read_result)
         return read_result
 
-    def delete_profile(self, profile_id: int):
+    def delete_by_profile_id(self, profile_id: int):
         DELETE_PROFILE_METHOD_NAME = "delete_profile"
         logger.start(DELETE_PROFILE_METHOD_NAME, object={'profile_id': profile_id})
 
         query_update = "UPDATE profile_table SET end_timestamp = NOW() WHERE profile_id = %s"
         self.cursor.execute(query_update, (profile_id, ))
 
         self.connector.commit()
         logger.end(DELETE_PROFILE_METHOD_NAME)
-
-    def get_last_profile_id_by_name(self, name: str) -> int:
-        GET_PROFILE_ID_METHOD_NAME = "get_profile_id_by_name"
-        logger.start(GET_PROFILE_ID_METHOD_NAME, object={'name': name})
-        query_get = "SELECT profile_id FROM profile_ml_view WHERE name = %s ORDER BY profile_ml_id DESC LIMIT 1"
-        self.cursor.execute(query_get, (name,))
-        profile_id, = self.cursor.fetchone()
-
-        logger.end(GET_PROFILE_ID_METHOD_NAME, object={'profile_id': profile_id})
-        return profile_id
```

### Comparing `profile-local-0.0.8/setup.py` & `profile-local-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
      name='profile-local',  
-     version='0.0.8',   #https://pypi.org/project/profile-local/
+     version='0.0.9',   #https://pypi.org/project/profile-local/
      author="Circles",
      author_email="info@circles.life",
      description="PyPI Package for Circles Profile Local Python",
      long_description="This is a package for sharing common profile functions used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/circles",
      packages=setuptools.find_packages(),
```

