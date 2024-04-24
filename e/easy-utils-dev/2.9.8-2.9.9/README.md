# Comparing `tmp/easy_utils_dev-2.9.8.tar.gz` & `tmp/easy_utils_dev-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_utils_dev-2.9.8.tar", last modified: Wed Apr 17 23:02:28 2024, max compression
+gzip compressed data, was "easy_utils_dev-2.9.9.tar", last modified: Wed Apr 24 09:07:11 2024, max compression
```

## Comparing `easy_utils_dev-2.9.8.tar` & `easy_utils_dev-2.9.9.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 23:02:28.270007 easy_utils_dev-2.9.8/
--rw-rw-rw-   0        0        0      174 2024-04-17 23:02:28.265129 easy_utils_dev-2.9.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 23:02:28.227870 easy_utils_dev-2.9.8/easy_utils_dev/
--rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.9.8/easy_utils_dev/EasySsh.py
--rw-rw-rw-   0        0        0     2978 2024-04-15 06:57:41.000000 easy_utils_dev-2.9.8/easy_utils_dev/Events.py
--rw-rw-rw-   0        0        0      389 2024-04-07 14:14:30.000000 easy_utils_dev-2.9.8/easy_utils_dev/__init__.py
--rw-rw-rw-   0        0        0    19602 2024-04-17 23:02:12.000000 easy_utils_dev-2.9.8/easy_utils_dev/cplib.py
--rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.9.8/easy_utils_dev/custom_env.py
--rw-rw-rw-   0        0        0     8876 2024-04-17 15:54:24.000000 easy_utils_dev-2.9.8/easy_utils_dev/debugger.py
--rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.9.8/easy_utils_dev/encryptor.py
--rw-rw-rw-   0        0        0     7170 2024-04-05 20:43:02.000000 easy_utils_dev-2.9.8/easy_utils_dev/keycloakapi.py
--rw-rw-rw-   0        0        0     7942 2024-04-07 14:50:44.000000 easy_utils_dev-2.9.8/easy_utils_dev/lralib.py
--rw-rw-rw-   0        0        0    33411 2024-04-17 16:03:32.000000 easy_utils_dev-2.9.8/easy_utils_dev/ne1830PSS.py
--rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.9.8/easy_utils_dev/optics_utils.py
--rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.9.8/easy_utils_dev/simple_sqlite.py
--rw-rw-rw-   0        0        0     2176 2024-04-02 04:54:18.000000 easy_utils_dev-2.9.8/easy_utils_dev/uiserver.py
--rw-rw-rw-   0        0        0     3379 2024-04-17 21:11:29.000000 easy_utils_dev-2.9.8/easy_utils_dev/utils.py
--rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.9.8/easy_utils_dev/wsnoclib.py
--rw-rw-rw-   0        0        0     7984 2024-04-04 18:33:00.000000 easy_utils_dev-2.9.8/easy_utils_dev/wsselib.py
-drwxrwxrwx   0        0        0        0 2024-04-17 23:02:28.261219 easy_utils_dev-2.9.8/easy_utils_dev.egg-info/
--rw-rw-rw-   0        0        0      174 2024-04-17 23:02:28.000000 easy_utils_dev-2.9.8/easy_utils_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      633 2024-04-17 23:02:28.000000 easy_utils_dev-2.9.8/easy_utils_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 23:02:28.000000 easy_utils_dev-2.9.8/easy_utils_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-17 23:02:28.000000 easy_utils_dev-2.9.8/easy_utils_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-17 23:02:28.000000 easy_utils_dev-2.9.8/easy_utils_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 23:02:28.270007 easy_utils_dev-2.9.8/setup.cfg
--rw-rw-rw-   0        0        0      317 2024-04-17 23:02:23.000000 easy_utils_dev-2.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:07:11.432499 easy_utils_dev-2.9.9/
+-rw-rw-rw-   0        0        0      174 2024-04-24 09:07:11.424467 easy_utils_dev-2.9.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 09:07:11.348801 easy_utils_dev-2.9.9/easy_utils_dev/
+-rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.9.9/easy_utils_dev/EasySsh.py
+-rw-rw-rw-   0        0        0     2978 2024-04-15 06:57:41.000000 easy_utils_dev-2.9.9/easy_utils_dev/Events.py
+-rw-rw-rw-   0        0        0      419 2024-04-23 18:04:28.000000 easy_utils_dev-2.9.9/easy_utils_dev/__init__.py
+-rw-rw-rw-   0        0        0    19602 2024-04-22 03:43:01.000000 easy_utils_dev-2.9.9/easy_utils_dev/cplib.py
+-rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.9.9/easy_utils_dev/custom_env.py
+-rw-rw-rw-   0        0        0     8876 2024-04-17 15:54:24.000000 easy_utils_dev-2.9.9/easy_utils_dev/debugger.py
+-rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.9.9/easy_utils_dev/encryptor.py
+-rw-rw-rw-   0        0        0     7170 2024-04-05 20:43:02.000000 easy_utils_dev-2.9.9/easy_utils_dev/keycloakapi.py
+-rw-rw-rw-   0        0        0     7942 2024-04-07 14:50:44.000000 easy_utils_dev-2.9.9/easy_utils_dev/lralib.py
+-rw-rw-rw-   0        0        0    33411 2024-04-17 16:03:32.000000 easy_utils_dev-2.9.9/easy_utils_dev/ne1830PSS.py
+-rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.9.9/easy_utils_dev/optics_utils.py
+-rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.9.9/easy_utils_dev/simple_sqlite.py
+-rw-rw-rw-   0        0        0     2451 2024-04-24 08:17:39.000000 easy_utils_dev-2.9.9/easy_utils_dev/uiserver.py
+-rw-rw-rw-   0        0        0     3379 2024-04-17 21:11:29.000000 easy_utils_dev-2.9.9/easy_utils_dev/utils.py
+-rw-rw-rw-   0        0        0    12341 2024-04-24 09:02:45.000000 easy_utils_dev-2.9.9/easy_utils_dev/winserviceapi.py
+-rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.9.9/easy_utils_dev/wsnoclib.py
+-rw-rw-rw-   0        0        0     7984 2024-04-04 18:33:00.000000 easy_utils_dev-2.9.9/easy_utils_dev/wsselib.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:07:11.416657 easy_utils_dev-2.9.9/easy_utils_dev.egg-info/
+-rw-rw-rw-   0        0        0      174 2024-04-24 09:07:10.000000 easy_utils_dev-2.9.9/easy_utils_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      665 2024-04-24 09:07:11.000000 easy_utils_dev-2.9.9/easy_utils_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 09:07:10.000000 easy_utils_dev-2.9.9/easy_utils_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-24 09:07:10.000000 easy_utils_dev-2.9.9/easy_utils_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-24 09:07:10.000000 easy_utils_dev-2.9.9/easy_utils_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 09:07:11.433476 easy_utils_dev-2.9.9/setup.cfg
+-rw-rw-rw-   0        0        0      317 2024-04-24 09:07:07.000000 easy_utils_dev-2.9.9/setup.py
```

### Comparing `easy_utils_dev-2.9.8/easy_utils_dev/EasySsh.py` & `easy_utils_dev-2.9.9/easy_utils_dev/EasySsh.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.8/easy_utils_dev/Events.py` & `easy_utils_dev-2.9.9/easy_utils_dev/Events.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.8/easy_utils_dev/cplib.py` & `easy_utils_dev-2.9.9/easy_utils_dev/cplib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.8/easy_utils_dev/custom_env.py` & `easy_utils_dev-2.9.9/easy_utils_dev/custom_env.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.8/easy_utils_dev/debugger.py` & `easy_utils_dev-2.9.9/easy_utils_dev/debugger.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.8/easy_utils_dev/encryptor.py` & `easy_utils_dev-2.9.9/easy_utils_dev/encryptor.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.8/easy_utils_dev/keycloakapi.py` & `easy_utils_dev-2.9.9/easy_utils_dev/keycloakapi.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.8/easy_utils_dev/lralib.py` & `easy_utils_dev-2.9.9/easy_utils_dev/lralib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.8/easy_utils_dev/ne1830PSS.py` & `easy_utils_dev-2.9.9/easy_utils_dev/ne1830PSS.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.8/easy_utils_dev/optics_utils.py` & `easy_utils_dev-2.9.9/easy_utils_dev/optics_utils.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.8/easy_utils_dev/simple_sqlite.py` & `easy_utils_dev-2.9.9/easy_utils_dev/simple_sqlite.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.8/easy_utils_dev/uiserver.py` & `easy_utils_dev-2.9.9/easy_utils_dev/uiserver.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,22 +10,25 @@
 from easy_utils_dev.custom_env import cenv
 
 
 def getClassById( id ) :
     return cenv[id]
 
 class UISERVER :
-    def __init__(self ,id=getRandomKey(n=15),secretkey=generateToken(),address='localhost',port=5312,**kwargs) -> None:
+    def __init__(self ,id=getRandomKey(n=15),secretkey=generateToken(),address='localhost',port=5312 , https=False  ,**kwargs) -> None:
         self.id = id
         self.app = app = Flask(self.id)
         app.config['SECRET_KEY'] = secretkey
         CORS(app,resources={r"/*":{"origins":"*"}})
         self.address= address 
         self.port = port
-        self.httpProtocol = 'http'
+        if https :
+            self.httpProtocol = 'https'
+        else :
+            self.httpProtocol = 'http'
         self.socketio = SocketIO(app , cors_allowed_origins="*"  ,async_mode='threading' , engineio_logger=False , always_connect=True ,**kwargs )
         cenv[id] = self
         self.fullAddress = f"{self.httpProtocol}://{self.address}:{self.port}"
 
     def getInstance(self) :
         return self.getFlask() , self.getSocketio() , self.getWsgi()
     
@@ -37,27 +40,31 @@
     
     def getWsgi(self) :
         return self.wsgi_server
 
     def shutdownUi(self) :
         self.wsgi_server.shutdown()
 
-    def startUi(self) :
+    def startUi(self,daemon=True) :
 
         @self.app.route('/connection/test/internal' , methods=['GET'])
         def test_connection():
             return json.dumps({'status' : 200 , 'id' : self.id })
-
+        if self.httpProtocol == 'http' :
+            con = None
+        elif self.httpProtocol == 'https' :
+            con='adhoc'
         self.wsgi_server = wsgi_server = ThreadedWSGIServer(
             host = self.address ,
+            ssl_context=con,
             port = self.port,
             app = self.app )
         
         def _start() :
             print(f"web-socket: {self.fullAddress}")
             log = logging.getLogger('werkzeug')
             log.setLevel(logging.ERROR)
             wsgi_server.serve_forever()   
         
         self.flaskprocess = Thread(target=_start)
-        self.flaskprocess.daemon = True
+        self.flaskprocess.daemon = daemon
         self.flaskprocess.start()
```

### Comparing `easy_utils_dev-2.9.8/easy_utils_dev/utils.py` & `easy_utils_dev-2.9.9/easy_utils_dev/utils.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.8/easy_utils_dev/wsnoclib.py` & `easy_utils_dev-2.9.9/easy_utils_dev/wsnoclib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.8/easy_utils_dev/wsselib.py` & `easy_utils_dev-2.9.9/easy_utils_dev/wsselib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9.8/easy_utils_dev.egg-info/SOURCES.txt` & `easy_utils_dev-2.9.9/easy_utils_dev.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 easy_utils_dev/keycloakapi.py
 easy_utils_dev/lralib.py
 easy_utils_dev/ne1830PSS.py
 easy_utils_dev/optics_utils.py
 easy_utils_dev/simple_sqlite.py
 easy_utils_dev/uiserver.py
 easy_utils_dev/utils.py
+easy_utils_dev/winserviceapi.py
 easy_utils_dev/wsnoclib.py
 easy_utils_dev/wsselib.py
 easy_utils_dev.egg-info/PKG-INFO
 easy_utils_dev.egg-info/SOURCES.txt
 easy_utils_dev.egg-info/dependency_links.txt
 easy_utils_dev.egg-info/requires.txt
 easy_utils_dev.egg-info/top_level.txt
```

