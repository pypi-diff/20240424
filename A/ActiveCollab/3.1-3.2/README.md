# Comparing `tmp/activecollab-3.1.tar.gz` & `tmp/activecollab-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activecollab-3.1.tar", last modified: Fri Apr 19 05:52:10 2024, max compression
+gzip compressed data, was "activecollab-3.2.tar", last modified: Wed Apr 24 04:13:38 2024, max compression
```

## Comparing `activecollab-3.1.tar` & `activecollab-3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:52:10.768946 activecollab-3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:52:10.768946 activecollab-3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:52:10.768946 activecollab-3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-19 05:52:05.000000 activecollab-3.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-19 05:52:05.000000 activecollab-3.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:52:10.768946 activecollab-3.1/ActiveCollab/
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-19 05:52:05.000000 activecollab-3.1/ActiveCollab/ActiveCollab.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 05:52:05.000000 activecollab-3.1/ActiveCollab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:52:10.768946 activecollab-3.1/ActiveCollab/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-19 05:52:05.000000 activecollab-3.1/ActiveCollab/__pycache__/ActiveCollab.cpython-38.pyc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:52:10.768946 activecollab-3.1/ActiveCollab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-19 05:52:10.000000 activecollab-3.1/ActiveCollab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-19 05:52:10.000000 activecollab-3.1/ActiveCollab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 05:52:10.000000 activecollab-3.1/ActiveCollab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 05:52:10.000000 activecollab-3.1/ActiveCollab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 05:52:10.000000 activecollab-3.1/ActiveCollab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-19 05:52:05.000000 activecollab-3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-19 05:52:10.768946 activecollab-3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-19 05:52:05.000000 activecollab-3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-19 05:52:05.000000 activecollab-3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 05:52:10.768946 activecollab-3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-19 05:52:05.000000 activecollab-3.1/setup.py_bck
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:13:38.237677 activecollab-3.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:13:38.233677 activecollab-3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:13:38.233677 activecollab-3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-24 04:13:32.000000 activecollab-3.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 04:13:32.000000 activecollab-3.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:13:38.233677 activecollab-3.2/ActiveCollab/
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-24 04:13:32.000000 activecollab-3.2/ActiveCollab/ActiveCollab.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-24 04:13:32.000000 activecollab-3.2/ActiveCollab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:13:38.233677 activecollab-3.2/ActiveCollab/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-24 04:13:32.000000 activecollab-3.2/ActiveCollab/__pycache__/ActiveCollab.cpython-38.pyc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:13:38.233677 activecollab-3.2/ActiveCollab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-24 04:13:38.000000 activecollab-3.2/ActiveCollab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-24 04:13:38.000000 activecollab-3.2/ActiveCollab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 04:13:38.000000 activecollab-3.2/ActiveCollab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 04:13:38.000000 activecollab-3.2/ActiveCollab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 04:13:38.000000 activecollab-3.2/ActiveCollab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-24 04:13:32.000000 activecollab-3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-24 04:13:38.233677 activecollab-3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-24 04:13:32.000000 activecollab-3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-24 04:13:32.000000 activecollab-3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 04:13:38.237677 activecollab-3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-24 04:13:32.000000 activecollab-3.2/setup.py_bck
```

### Comparing `activecollab-3.1/.github/workflows/publish.yml` & `activecollab-3.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `activecollab-3.1/ActiveCollab/ActiveCollab.py` & `activecollab-3.2/ActiveCollab/ActiveCollab.py`

 * *Files 21% similar despite different names*

```diff
@@ -30,48 +30,74 @@
         headers = {"Content-Type": "application/json" ,
                    "X-Angie-AuthApiToken": self.token}
 
         response = requests.get(url , headers=headers)
 
         if response.status_code == 200:
             projects = []
-            project = {}
             projects_data = response.json()
 
         if response.status_code != 200:
-            print('Error while fetching projects')
+            print(f'Error while fetching projects {response.status_code}')
             sys.exit()
 
         for i in projects_data:
+            project = {}
             project['id'] = i['id']
             project['name'] = i['name']
             project['members'] = i['members']
             projects.append(project)
         return projects
+    def list_project_tasklist(self,project_id):
+        """
+        :return: list of all projects you have with their project number
+        """
+        url = f'{self.host_url}/api/v1/projects/{project_id}/task-lists'
+        headers = {"Content-Type": "application/json" ,
+                   "X-Angie-AuthApiToken": self.token}
+
+        response = requests.get(url , headers=headers)
+
+        if response.status_code == 200:
+            projects_tasklist = []
+            projects_data = response.json()
+
+        if response.status_code != 200:
+            print(f'Error while fetching project {response.status_code}')
+            sys.exit()
+
+        for i in projects_data:
+            projects_tasklist_data = {}
+            projects_tasklist_data['id'] = i['id']
+            projects_tasklist_data['name'] = i['name']
+            projects_tasklist.append(projects_tasklist_data)
+            print(projects_tasklist)
+        return projects_tasklist
 
     def list_users(self):
         """
         :return: list of all users
         """
         url = f'{self.host_url}/api/v1/users'
         headers = {"Content-Type": "application/json" ,
                    "X-Angie-AuthApiToken": self.token}
 
         response = requests.get(url , headers=headers)
 
         if response.status_code == 200:
             users = []
-            user = {}
             users_data = response.json()
+            print(users_data)
 
         if response.status_code != 200:
             print('Error while fetching users')
             sys.exit()
 
         for i in users_data:
+            user = {}
             user['id'] = i['id']
             user['name'] = i['first_name']
             user['email'] = i['email']
             users.append(user)
         return users
 
     def project_detail(self , project_id):
```

### Comparing `activecollab-3.1/ActiveCollab.egg-info/PKG-INFO` & `activecollab-3.2/ActiveCollab.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ActiveCollab
-Version: 3.1
+Version: 3.2
 Summary: A python library working with activeCollab
 Author-email: Ankushtpss <ankushkumartpss@gmail.com>
 Project-URL: Homepage, https://github.com/Ankushtpss/ActiveCollab
 Project-URL: Bug Tracker, https://github.com/Ankushtpss/ActiveCollab/issues
 Keywords: Active Collab,ActiveCollab,Active Collab SDK,active collab
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -45,14 +45,19 @@
 ```
 
 ### List all projects
 ```python
 ac.list_projects()  # List out all project assigned to logged in user
 ```
 
+### List all task-list of a project
+```python
+ac.list_project_tasklist(project_id)  # List out all task-list of a project
+```
+
 ### List all users
 ```python
 ac.list_users()  # List out all users in your organization with id, name and email
 ```
 
 ### List Users in a Project
 ```python
```

### Comparing `activecollab-3.1/LICENSE` & `activecollab-3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `activecollab-3.1/PKG-INFO` & `activecollab-3.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ActiveCollab
-Version: 3.1
+Version: 3.2
 Summary: A python library working with activeCollab
 Author-email: Ankushtpss <ankushkumartpss@gmail.com>
 Project-URL: Homepage, https://github.com/Ankushtpss/ActiveCollab
 Project-URL: Bug Tracker, https://github.com/Ankushtpss/ActiveCollab/issues
 Keywords: Active Collab,ActiveCollab,Active Collab SDK,active collab
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -45,14 +45,19 @@
 ```
 
 ### List all projects
 ```python
 ac.list_projects()  # List out all project assigned to logged in user
 ```
 
+### List all task-list of a project
+```python
+ac.list_project_tasklist(project_id)  # List out all task-list of a project
+```
+
 ### List all users
 ```python
 ac.list_users()  # List out all users in your organization with id, name and email
 ```
 
 ### List Users in a Project
 ```python
```

### Comparing `activecollab-3.1/README.md` & `activecollab-3.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,19 @@
 ```
 
 ### List all projects
 ```python
 ac.list_projects()  # List out all project assigned to logged in user
 ```
 
+### List all task-list of a project
+```python
+ac.list_project_tasklist(project_id)  # List out all task-list of a project
+```
+
 ### List all users
 ```python
 ac.list_users()  # List out all users in your organization with id, name and email
 ```
 
 ### List Users in a Project
 ```python
```

### Comparing `activecollab-3.1/pyproject.toml` & `activecollab-3.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ]
 
 dependencies = [
     "requests",
     "sys",
 ]
 
-version = "3.1"
+version = "3.2"
 
 [tool.setuptools_scm]
 
 [project.urls]
 "Homepage" = "https://github.com/Ankushtpss/ActiveCollab"
 "Bug Tracker" = "https://github.com/Ankushtpss/ActiveCollab/issues"
```

### Comparing `activecollab-3.1/setup.py_bck` & `activecollab-3.2/setup.py_bck`

 * *Files identical despite different names*

