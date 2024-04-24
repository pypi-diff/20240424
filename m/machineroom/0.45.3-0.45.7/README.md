# Comparing `tmp/machineroom-0.45.3.tar.gz` & `tmp/machineroom-0.45.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machineroom-0.45.3.tar", last modified: Sun Apr 14 05:39:34 2024, max compression
+gzip compressed data, was "machineroom-0.45.7.tar", last modified: Wed Apr 24 18:48:57 2024, max compression
```

## Comparing `machineroom-0.45.3.tar` & `machineroom-0.45.7.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-14 05:39:34.728881 machineroom-0.45.3/
--rw-r--r--   0 root         (0) staff       (20)     2358 2024-02-29 11:53:06.000000 machineroom-0.45.3/.gitignore
--rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.45.3/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     4392 2024-04-14 05:39:34.728713 machineroom-0.45.3/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     3597 2024-02-29 11:21:25.000000 machineroom-0.45.3/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-14 05:39:34.719731 machineroom-0.45.3/cmdbin/
--rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.45.3/cmdbin/connect
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-14 05:39:34.725681 machineroom-0.45.3/machineroom/
--rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-14 05:39:34.000000 machineroom-0.45.3/machineroom/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     8132 2024-04-14 04:31:36.000000 machineroom-0.45.3/machineroom/const.py
--rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.45.3/machineroom/schema.json
--rw-r--r--   0 root         (0) staff       (20)    13510 2024-04-13 15:24:08.000000 machineroom-0.45.3/machineroom/sql.py
--rw-r--r--   0 root         (0) staff       (20)    25277 2024-04-14 04:31:36.000000 machineroom-0.45.3/machineroom/taskbase.py
--rw-r--r--   0 root         (0) staff       (20)    14368 2024-04-08 17:07:54.000000 machineroom-0.45.3/machineroom/util.py
--rw-r--r--   0 root         (0) staff       (20)     2759 2024-03-23 02:51:57.000000 machineroom-0.45.3/machineroom/worker.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-14 05:39:34.728188 machineroom-0.45.3/machineroom.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     4392 2024-04-14 05:39:34.000000 machineroom-0.45.3/machineroom.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      371 2024-04-14 05:39:34.000000 machineroom-0.45.3/machineroom.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-04-14 05:39:34.000000 machineroom-0.45.3/machineroom.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       12 2024-04-14 05:39:34.000000 machineroom-0.45.3/machineroom.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       79 2024-04-14 05:39:34.729421 machineroom-0.45.3/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     2569 2024-03-01 08:09:46.000000 machineroom-0.45.3/setup.py
--rw-r--r--   0 root         (0) staff       (20)     1532 2024-04-13 11:13:43.000000 machineroom-0.45.3/update
--rw-r--r--   0 root         (0) staff       (20)        7 2024-04-14 05:39:17.000000 machineroom-0.45.3/version
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 18:48:57.273468 machineroom-0.45.7/
+-rw-r--r--   0 root         (0) staff       (20)     2365 2024-04-24 18:48:26.000000 machineroom-0.45.7/.gitignore
+-rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.45.7/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     4714 2024-04-24 18:48:57.273200 machineroom-0.45.7/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3597 2024-02-29 11:21:25.000000 machineroom-0.45.7/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 18:48:57.263947 machineroom-0.45.7/cmdbin/
+-rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.45.7/cmdbin/connect
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 18:48:57.267684 machineroom-0.45.7/machineroom/
+-rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-24 18:48:56.000000 machineroom-0.45.7/machineroom/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     9410 2024-04-24 17:40:53.000000 machineroom-0.45.7/machineroom/const.py
+-rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.45.7/machineroom/schema.json
+-rw-r--r--   0 root         (0) staff       (20)    14669 2024-04-24 18:22:06.000000 machineroom-0.45.7/machineroom/sql.py
+-rw-r--r--   0 root         (0) staff       (20)    28485 2024-04-24 18:48:01.000000 machineroom-0.45.7/machineroom/taskbase.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 18:48:57.271628 machineroom-0.45.7/machineroom/tunnels/
+-rw-r--r--   0 root         (0) staff       (20)       23 2024-04-24 17:37:19.000000 machineroom-0.45.7/machineroom/tunnels/__init__.py
+-rwxr-xr-x   0 root         (0) staff       (20)     8069 2024-04-24 17:12:31.000000 machineroom-0.45.7/machineroom/tunnels/conn.py
+-rw-r--r--   0 root         (0) staff       (20)      468 2024-04-24 17:12:31.000000 machineroom-0.45.7/machineroom/tunnels/fork.py
+-rw-r--r--   0 root         (0) staff       (20)    15171 2024-04-24 18:22:06.000000 machineroom-0.45.7/machineroom/util.py
+-rw-r--r--   0 root         (0) staff       (20)     5230 2024-04-24 18:48:01.000000 machineroom-0.45.7/machineroom/worker.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 18:48:57.272556 machineroom-0.45.7/machineroom.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     4714 2024-04-24 18:48:57.000000 machineroom-0.45.7/machineroom.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      493 2024-04-24 18:48:57.000000 machineroom-0.45.7/machineroom.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-24 18:48:57.000000 machineroom-0.45.7/machineroom.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       28 2024-04-24 18:48:57.000000 machineroom-0.45.7/machineroom.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       12 2024-04-24 18:48:57.000000 machineroom-0.45.7/machineroom.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       79 2024-04-24 18:48:57.274063 machineroom-0.45.7/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     2620 2024-04-24 14:34:36.000000 machineroom-0.45.7/setup.py
+-rw-r--r--   0 root         (0) staff       (20)     1532 2024-04-15 07:27:18.000000 machineroom-0.45.7/update
+-rw-r--r--   0 root         (0) staff       (20)        7 2024-04-24 18:48:47.000000 machineroom-0.45.7/version
```

### Comparing `machineroom-0.45.3/.gitignore` & `machineroom-0.45.7/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -200,7 +200,8 @@
 .ropeproject
 
 # mkdocs documentation
 /site
 
 # mypy
 .mypy_cache/
+test_*
```

### Comparing `machineroom-0.45.3/LICENSE` & `machineroom-0.45.7/LICENSE`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.3/PKG-INFO` & `machineroom-0.45.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: machineroom
-Version: 0.45.3
-Summary: A Python package to manage all my machines in the fingertip.
-Home-page: https://github.com/jjhesk/mymachineroom/
-Author: Jun-You Liu & Heskemo
-Author-email: meowmeow@gmail.com
-License: MIT
-Keywords: ssh machine room
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8,<4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Machine Room Management on my console
 
 Locate and manage all my machines on my console.
 
 ## Introduction
 
 Congratulations on utilizing technology to improve your machine room management! Having a machine room management app on your console, easily accessible at your fingertips, is a game-changer. It streamlines processes, increases efficiency, and allows you to stay on top of everything with ease. By taking advantage of this tool, you are not only simplifying your workload but also paving the way for future success. Keep up the great work and continue to embrace innovation in your everyday tasks. You've got this!
```

### Comparing `machineroom-0.45.3/cmdbin/connect` & `machineroom-0.45.7/cmdbin/connect`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.3/machineroom/__init__.py` & `machineroom-0.45.7/machineroom/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 logger5 = logging.getLogger("invoke")
 logger2.setLevel(logging.ERROR)
 logger1.setLevel(logging.ERROR)
 logger3.setLevel(logging.ERROR)
 logger4.setLevel(logging.ERROR)
 logger5.setLevel(logging.ERROR)
 
-__version__ = '0.45.3'
+__version__ = '0.45.7'
```

### Comparing `machineroom-0.45.3/machineroom/const.py` & `machineroom-0.45.7/machineroom/const.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from enum import Enum
+
+
 class PROJECT1:
     REMOTE_WS: str = "...remote_locator"
     WS_LOCAL: str = "...remote_locator"
     RAM_GB_REQUIREMENT: int = 4
     DISK_GB_REQUIREMENT: int = 100
     CONTAINER_NAME_IDS: list = []
 
@@ -13,23 +16,43 @@
 class COMMAND_PATH:
     BASH = "/usr/bin/bash"
     DOCKER_COMPOSE_VERSION: str = "2.24.6"
     DOCKER_COMPOSE = "/usr/local/bin/docker-compose"
     DOCKER = "/usr/bin/docker"
 
 
-class Config(COMMAND_PATH, PROJECT1, PROJECT2):
-    DATAPATH_BASE: str = "...._file....locator"
-    TEMP_FILE: str = "tmp.txt"
-    TEMP_JS: str = "tmp.js"
-    PUB_KEY: str = "/Users/xxxx/.ssh/id_rsa.pub"
-    LOCAL_KEY_HOLDER: str = "/Users/xxxx/.ssh"
-    MY_KEY_FEATURE: str = "xxx@xxxx"
-    HOME: str = "/root"
-    STAGE1 = ["cert", "docker", "docker-compose", "env"]
+class TunnelType(Enum):
+    NO_TUNNEL = 0
+    L2TP_IPSEC = 1
+    CISCO_IPSEC = 2
+    IKEV2 = 3
+    SSTP = 4
+    DAE = 5
+    IPVANISH = 6
+    PPTP = 7
+    WIREGUARD = 8
+
+    @classmethod
+    def Recongize(cls, what:str):
+        what = what.lower()
+        if "l2tp/ipsec" in what:
+            return cls.L2TP_IPSEC
+
+        elif "cisco/ipsec" in what:
+            return cls.CISCO_IPSEC
+
+        elif "ikv2" in what:
+            return cls.IKEV2
+
+        else:
+            return cls.NO_TUNNEL
+
+    @classmethod
+    def from_date(cls, date):
+        return cls(date.isoweekday())
 
 
 DETECT_PROCESS = 'ps aux | grep -sie "{COMMAND_NAME}" | grep -v "grep -sie"'
 HEALTH_CHK_DB = """docker run --rm -it --mount type=bind,source={PWD},destination=/data sstc/sqlite3 find . -maxdepth 1 -iname "*.db" -print0 -exec sqlite3 '{}' 'PRAGMA integrity_check;' ';'"""
 HEALTH_CHK_DB2 = """
 sudo apt update && sudo apt install sqlite3 -y
 sqlite3 --version
@@ -66,14 +89,23 @@
 stable"
 sudo apt-get update
 sudo apt-get install -y docker-ce
 sudo apt-get update
 sudo groupadd docker
 sudo usermod -aG docker $USER
 sudo systemctl enable docker"""
+DOCKER_V25_INSTALL = """
+docker --version | awk '{print $3}' | cut -d ',' -f1
+docker_version=$(docker --version | awk '{print $3}' | cut -d ',' -f1)
+if [ "$(echo -e "$docker_version 25" | sort -V | head -n1)" != "25" ]; then
+  echo "Updating Docker to version 25"
+  curl -fsSL https://get.docker.com | sh >/dev/null 2>&1
+fi
+echo "Docker version is now 25"
+"""
 PYTHON_CE = """sudo apt-get install -y \
 apt-transport-https \
 ca-certificates \
 curl \
 software-properties-common \
 python3"""
 INSTALL_DAED = """
@@ -82,14 +114,15 @@
 wget -P /tmp https://github.com/daeuniverse/daed/releases/latest/download/installer-daed-linux-$(arch).deb
 sudo dpkg -i /tmp/installer-daed-linux-$(arch).deb
 rm /tmp/installer-daed-linux-$(arch).deb
 sudo systemctl enable daed
 sudo systemctl start daed
 sudo systemctl status daed
 """
+INSTALL_WATCH_TOWER = "docker run -d --name watchtower -v /var/run/docker.sock:/var/run/docker.sock containrrr/watchtower"
 PORT_DETECTION = """
 # 检测并罗列未被占用的端口
 function list_recommended_ports {
     local start_port=8000 # 可以根据需要调整起始搜索端口
     local needed_ports=7
     local count=0
     local ports=()
@@ -103,25 +136,27 @@
     echo "推荐的端口如下："
     for port in "${ports[@]}"; do
         echo -e "\033[0;32m$port\033[0m"
     done
 }
 list_recommended_ports;"""
 DOCKER_STOP_REMOVE = """{COMMAND_DOCKER} rm $({COMMAND_DOCKER} stop $(sudo docker ps -a | grep "{CONTAINER_NAME}" | cut -d " " -f 1))"""
-DOCKER_LAUNCH_LINE = """{COMMAND_DOCKER} run -d --name {NODE_NAME} {VOLUME} {BIND_FILE} {NETWORK} --restart unless-stopped {IMAGE}{VERSION} {COMMAND}"""
+DOCKER_LAUNCH_LINE = """{COMMAND_DOCKER} run -d --name {NODE_NAME} {VOLUME} {BIND_FILE} {NETWORK} --restart unless-stopped {LOG_POLICY} {IMAGE}{VERSION} {COMMAND}"""
 DOCKER_STOP_ID = """{COMMAND_DOCKER} stop {CID}"""
 DOCKER_STOP_RM = """{COMMAND_DOCKER} rm {CID}"""
 DOCKER_STOP_CONTAIN_NAME = """{COMMAND_DOCKER} ps -a | grep '{CONTAINER_NAME}' | awk '{{print $1}}' | xargs {COMMAND_DOCKER} stop"""
 DOCKER_RM_NAME_BASED = """{COMMAND_DOCKER} ps -a | grep '{CONTAINER_NAME}' | awk '{{print $1}}' | xargs -r {COMMAND_DOCKER} rm -f"""
 DOCKER_RM_VOLUME = """{COMMAND_DOCKER} volume ls -qf dangling=true -f name={CONTAINER_NAME} | xargs -r {COMMAND_DOCKER} volume rm"""
 DOCKER_LOG_REVIEW = """COMMAND_DOCKER ps -a --filter "name=__CONTAINER_KEYWORD" --format "{{.ID}}" | shuf -n 1 | xargs docker logs --tail __RECENT_LINES"""
 DOCKER_GET_NETWORK_NAME = """COMMAND_DOCKER inspect -f '{{range $key, $value := .NetworkSettings.Networks}} {{$key}} {{end}}' CONTAINER_ID"""
 DOCKER_GET_CONTAINER_ID = """COMMAND_DOCKER inspect $(docker ps | grep "__IMAGE_NAME_OR_KEYWORD__" | awk '{print $1}') | grep '"Id":' | awk '{print $2}' | tr --delete '"' | tr --delete ','"""
 DOCKER_MOUNT_FILE = """--mount type=bind,source={SOURCE},target={TARGET}"""
 DOCKER_MOUNT_FILE_RO = """--mount type=bind,source={SOURCE},target={TARGET},readonly"""
+DOCKER_LOG_POLICY_10m_5f = "--log-opt max-size=10m --log-opt max-file=5"
+DOCKER_LOG_POLICY_5m_10f = "--log-opt max-size=5m --log-opt max-file=10"
 BACKUP_CACHE_FAST = """
 # Define the path to the file
 path_to_file="_CFP_"
 # Check if the file exists
 if [ -f "$path_to_file" ]; then
     # Go to the directory of the file
     cd "$(dirname "$path_to_file")" || exit
@@ -132,15 +167,15 @@
             if [ $? -eq 0 ]; then
                 break
             fi
         done
     echo "compress file success"
 fi"""
 DOCKER_COMPOSE_XCLASH = """
-version: '3.7'
+version: '3.8'
 services:
   proxy_service:
     image: dreamacro/clash
     container_name: clashmoe
     ports:
       - "17890:17890"
       - "17891:17891"
@@ -154,29 +189,29 @@
     privileged: true
     expose:
       - 7890
       - 7891
       - 17890
       - 9090
     networks:
-      - clsh_octopus_network
+      - octopus_dot
 
   proxy_control_service:
     image: adriansteward/galxewrok:X_CLASH_GALXE_HELPER_VER
     container_name: clash_checker
     restart: "on-failure"
     command: python clash_runtime.py
     networks:
-      - clsh_octopus_network
+      - octopus_dot
     depends_on:
       - proxy_service
     volumes:
       - ./config:/home/galxe/cache
 networks:
-  clsh_octopus_network:
+  octopus_dot:
 
 
 """
 CLASH_HELPER_RESOURCE = """{
   "clash_proxy": {
     "port": "7890",
     "secret": "___SECRET___",
@@ -184,15 +219,15 @@
     "selector": "___SELECTOR___",
     "test_endpoint": "__TEST_ENDPOINT__"
   }
 }
 """
 
 CLASH_SETUP_1 = """
-network_name="clsh_octopus_network"
+network_name="octopus_dot"
 docker network inspect "$network_name" >/dev/null 2>&1 || docker network create "$network_name"
 
 if [ -d "/home/clashperfectoctopus" ]; then
   cd /home/clashperfectoctopus
   git pull https://github.com/ONode/clashperfectoctopus.git
 else
   echo "Directory does not exist."
@@ -231,7 +266,20 @@
     exit;
 fi
 cd /home/clashperfectoctopus
 echo "start up the service"
 docker compose -f docker_proxy_compose.yml up -d
 
 """
+
+
+class Config(COMMAND_PATH, PROJECT1, PROJECT2):
+    DATAPATH_BASE: str = "...._file....locator"
+    TEMP_FILE: str = "tmp.txt"
+    TEMP_JS: str = "tmp.js"
+    PUB_KEY: str = "/Users/xxxx/.ssh/id_rsa.pub"
+    LOCAL_KEY_HOLDER: str = "/Users/xxxx/.ssh"
+    MY_KEY_FEATURE: str = "xxx@xxxx"
+    HOME: str = "/root"
+    SYSTEM_TEMP: str = "/tmp"
+    STAGE1 = ["cert", "docker", "env"]
+    DOCKER_LOG_POLICY: str = DOCKER_LOG_POLICY_10m_5f
```

### Comparing `machineroom-0.45.3/machineroom/schema.json` & `machineroom-0.45.7/machineroom/schema.json`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.3/machineroom/sql.py` & `machineroom-0.45.7/machineroom/sql.py`

 * *Files 6% similar despite different names*

```diff
@@ -273,14 +273,20 @@
 
     def is_docker_yacht_installed(self):
         return self._is_what_installed("yacht_installed")
 
     def is_dae_installed(self):
         return self._is_what_installed("daed_installed")
 
+    def is_watchtower_installed(self):
+        return self._is_what_installed("watchtower_installed")
+
+    def watchtower_install(self):
+        self._update_what_installed("watchtower_installed")
+
     def is_xclash_installed(self):
         return self._is_what_installed("clash_installed")
 
     def is_docker_ce_installed(self):
         return self._is_what_installed("docker_installed")
 
     def is_python_installed(self):
@@ -339,17 +345,26 @@
     def show_all_serv(self) -> list:
         h = self.show_all_servers(self._tblembr)
         return h
 
     def set_server_id(self, server_id: str):
         self.server_id = server_id
 
-    def update_profile(self, profile_res: dict):
+    def update_tunel_profile(self, profile_name: str):
+        self.update_res_kv("tunnel_profile", profile_name)
+
+    def update_res_kv(self, k: str, val):
         da = self.get_member_res(self._tblembr, self.server_id)
-        da.update({"profile": profile_res})
+        da.update({k: val})
+        self._update_server_meta(self.server_id, da)
+
+    def delete_res_kv(self, k: str):
+        da = self.get_member_res(self._tblembr, self.server_id)
+        if k in da:
+            da.pop(k)
         self._update_server_meta(self.server_id, da)
 
     def get_home_path(self) -> str:
         da = self.get_member_res(self._tblembr, self.server_id)
         if "home_path" in da:
             return da["home_path"]
         else:
@@ -378,14 +393,29 @@
             # update when the new data is found. but the ID cannot be updated.
             p = {
                 "host": host,
                 "user": user,
                 "pass": password,
                 "port": port,
             }
+            return self.update_param(self.server_id, p)
+
+    def tipping_point_tunnel(self, profile_tunnel: str, user: str, id: str, host: str, password: str, port: int = 22):
+        if self.has_this_server() is False:
+            # first time registration
+            self._insert_server(host, id, password, user, port, {"tunnel_profile": profile_tunnel})
+        else:
+            self.update_res_kv("tunnel_profile", profile_tunnel)
+            # update when the new data is found. but the ID cannot be updated.
+            p = {
+                "host": host,
+                "user": user,
+                "pass": password,
+                "port": port,
+            }
             return self.update_param(self.server_id, p)
 
     def set_invalidate_token(self):
         d = self.get_member_res(self._tblembr, self.server_id)
         d.update({
             "expires_in": 0
         })
```

### Comparing `machineroom-0.45.3/machineroom/taskbase.py` & `machineroom-0.45.7/machineroom/taskbase.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os.path
 
 import pexpect
 from fabric import Connection, Config as FabricConfig, Result
 from machineroom.sql import ServerRoom
+from machineroom.tunnels import conn
 from machineroom.util import *
 
 
 def copy_id(c: Connection, file: str = Config.PUB_KEY):
     '''fab push 公钥 ssh-copy-id'''
     print("copy_id operation")
     c.put(file, "/tmp/id.pub")
@@ -155,15 +156,15 @@
     script_file = open(file_name)
     result = c.run(script_file.read())
     script_file.close()
     return result
 
 
 def exec_shell_global(c: Connection, _program_: str):
-    return exec_shell_program(c, Config.HOME, _program_)
+    return exec_shell_program(c, Config.SYSTEM_TEMP, _program_)
 
 
 def exec_shell_program(c: Connection, remote_path: str, _program_: str) -> Result:
     buffer_file = BufferFile()
     buffer_file.new_bash()
     buffer_file.add_cmd(_program_)
     c.put(buffer_file.path, remote_path)
@@ -268,14 +269,69 @@
 
 
 def docker_solve_conflict(c: Connection, hash: str):
     c.run(DOCKER_STOP_ID.format(CID=hash, COMMAND_DOCKER=Config.DOCKER), pty=True, timeout=100, warn=True, echo=True)
     c.run(DOCKER_STOP_RM.format(CID=hash, COMMAND_DOCKER=Config.DOCKER), pty=True, timeout=100, warn=True, echo=True)
 
 
+def docker_get_container_ids_by_keyword(c: Connection, keyword: str) -> list:
+    command = '__DOCKER__ ps -aqf "name=^______"'.replace('______', keyword).replace('__DOCKER__', Config.DOCKER)
+    r = c.run(command, pty=True, timeout=1900, hide=True, warn=True, echo=False)
+    reblock = r.stdout.replace("\r", "")
+    ids = reblock.split('\n')
+    container__ids = []
+    for container__id in ids:
+        if container__id != '':
+            container__ids.append(container__id)
+    container__ids = list(set(container__ids))
+    return container__ids
+
+
+def docker_read_console_result():
+    io = open(os.path.join(Config.DATAPATH_BASE, 'command_prompt_tmp'), 'r')
+    content = io.read()
+    io.close()
+    return json.loads(content)
+
+
+def docker_save_console_result(r):
+    content = r.stdout
+    io = open(os.path.join(Config.DATAPATH_BASE, 'command_prompt_tmp'), 'w')
+    io.write(content)
+    io.close()
+
+
+def docker_inspect_file(c: Connection, container_id: str):
+    command = f'docker inspect {container_id}'
+    r = c.run(command, pty=True, timeout=1900, hide=True, warn=True, echo=False)
+    docker_save_console_result(r)
+    return docker_read_console_result()
+
+
+def docker_restart_containers(c: Connection, contain_ids, result_line=None):
+    if isinstance(contain_ids, list):
+        for id in contain_ids:
+            rv = c.run(
+                f"{Config.DOCKER} restart {id}",
+                pty=True, timeout=1900, warn=True, echo=True
+            )
+            if callable(result_line):
+                line = str(rv.stdout.strip().replace("\n", "")).lower()
+                result_line(line, id)
+
+    if isinstance(contain_ids, str):
+        rv = c.run(
+            f"{Config.DOCKER} restart {contain_ids}",
+            pty=True, timeout=1900, warn=True, echo=True
+        )
+        if callable(result_line):
+            line = str(rv.stdout.strip().replace("\n", "")).lower()
+            result_line(line, contain_ids)
+
+
 def docker_launch(c: Connection, vol: Union[str, list[str]], container_name: str, image: str, ver: str, command: str,
                   network: str = "", bind_file: Union[str, list[str]] = "") -> Result:
     _vol = ""
     if isinstance(vol, str):
         _vol = f" -v {vol}"
     if isinstance(vol, list):
         _vol = " -v " + " -v ".join(vol)
@@ -314,26 +370,32 @@
         COMMAND_DOCKER=Config.DOCKER,
         VOLUME=_vol,
         NETWORK=_net,
         NODE_NAME=container_name,
         IMAGE=image,
         VERSION=_ver,
         COMMAND=command,
-        BIND_FILE=_bindf
+        BIND_FILE=_bindf,
+        LOG_POLICY=Config.DOCKER_LOG_POLICY
     ), pty=True, timeout=4900, warn=True, echo=True)
 
 
 def stop_container_by_name(c: Connection, container_name: str):
     cmd_line_go = DOCKER_STOP_CONTAIN_NAME.format(
         COMMAND_DOCKER=Config.DOCKER,
         CONTAINER_NAME=container_name
     )
     return c.run(cmd_line_go, pty=True, timeout=1900, warn=True, echo=True)
 
 
+def docker_stop_by_prefix(c: Connection, word: str):
+    service = """docker stop $(docker ps | grep "KEY_WORD" | cut -d " " -f1)""".replace('KEY_WORD', word)
+    c.run(service, pty=True, timeout=1900, warn=True, echo=True)
+
+
 def rm_container_by_name(c: Connection, container_name: str):
     cmd_line_go = DOCKER_RM_NAME_BASED.format(
         COMMAND_DOCKER=Config.DOCKER,
         CONTAINER_NAME=container_name
     )
     return c.run(cmd_line_go, pty=True, timeout=1900, warn=True, echo=True)
 
@@ -441,20 +503,29 @@
     return c.run(RUN_YACHT.format(LISTEN_PORT=port), pty=True, timeout=300, warn=True)
 
 
 def install_dae_proxy(c: Connection):
     return c.run(INSTALL_DAED, pty=True, timeout=900, warn=True)
 
 
+def install_watch_tower(c: Connection):
+    return c.run(INSTALL_WATCH_TOWER, pty=True, timeout=2900, warn=True)
+
+
 def install_python(c: Connection):
     return c.run(PYTHON_CE, warn=True)
 
 
 def install_docker_ce(c: Connection):
-    exec_shell_global(c, DOCKER_CE_INSTALL)
+    exec_shell_global(c, DOCKER_V25_INSTALL)
+    return True
+
+
+def install_docker_25(c: Connection):
+    exec_shell_global(c, DOCKER_V25_INSTALL)
     return True
 
 
 def install_docker_compose(c: Connection):
     exec_shell_global(c, DOCKER_COMPOSE.format(
         DOCKER_COMPOSE_VERSION=Config.DOCKER_COMPOSE_VERSION
     ))
@@ -462,45 +533,39 @@
 
 def docker_launch_solution(c: Connection, node_name: str, pass_file: str):
     print("use container name", node_name)
     _command_line = f"python main_exe.py {pass_file}"
     sentence = docker_launch(
         c=c,
         container_name=node_name,
-        vol=[
-            "/home/galxeionetapplication/cache:/home/galxe/cache",
-            "/home/clash_docker/config/proxy_config.json:/home/galxe/cache/proxy_config.json"
-        ],
+        vol="/home/galxeionetapplication/cache:/home/galxe/cache",
         image="adriansteward/galxewrok",
         ver="",
         command=_command_line
     )
     (issue, hash) = docker_is_container_conflict(sentence)
     if issue:
         docker_solve_conflict(c, hash)
         docker_launch_solution(c, node_name, pass_file)
 
 
 def docker_get_network_name_by_container_id(c: Connection, container_id: str) -> str:
     content = DOCKER_GET_NETWORK_NAME.replace("COMMAND_DOCKER", Config.DOCKER).replace("CONTAINER_ID", container_id)
     r = c.run(content, timeout=90, warn=True, hide=True)
     if r.ok:
-        line = str(r.stdout.strip().replace("\n", ""))
-        return line
+        return str(r.stdout.strip().replace("\n", ""))
     return ""
 
 
 def docker_get_container_id_by_keyword(c: Connection, keyword: str) -> str:
     content = DOCKER_GET_CONTAINER_ID.replace("COMMAND_DOCKER", Config.DOCKER).replace("__IMAGE_NAME_OR_KEYWORD__",
                                                                                        keyword)
-    r = c.run(content, timeout=90)
+    r = c.run(content, timeout=90, warn=True, hide=True)
     if r.ok:
-        line = str(r.stdout.strip().replace("\n", ""))
-        print(line)
-        return line
+        return str(r.stdout.strip().replace("\n", ""))
     return ""
 
 
 def install_clash_network(
         c: Connection,
         network_config_file: str,
         helper_version: str,
@@ -541,29 +606,45 @@
 
 
 class DeploymentBotFoundation:
     # the text file servers that recorded the authentications and some basic information
     srv: Servers
     # the local db connection of servers
     db: ServerRoom
+    start_server_from: int
+    stop_server_at: int
+    start_server_in_list: list[int]
 
     def __init__(self, server_room: str):
         # the server room file, usually "xxxx_server_room.txt", located under cache folder.
         self.srv = Servers(server_room)
+        self.start_server_from = 0
+        self.stop_server_at = self.srv.serv_count - 1
+        self.start_server_in_list = []
         self.srv.detect_servers()
 
     def _config(self) -> FabricConfig:
         return FabricConfig({
             'run': {
                 'watchers': [
                     DummyWatcher(),
                 ],
             },
         })
 
+    def run_tunnel_detection(self):
+        if self.srv.tunnel_type == TunnelType.NO_TUNNEL:
+            return
+        conn.use_macos_vpn_on(self.srv.profile_name)
+
+    def run_tunnel_detection_off(self):
+        if self.srv.tunnel_type == TunnelType.NO_TUNNEL:
+            return
+        conn.use_macos_vpn_off(self.srv.profile_name)
+
     def _est_connection(self) -> Connection:
         if self.db.has_this_server() is False:
             return Connection(host=self.srv.current_host, port=22, user=self.srv.current_user, connect_kwargs={
                 "password": self.srv.current_pass,
                 # "key_filename": ['/Users/..../.ssh/id_rsa']
             }, config=self._config())
         elif self.db.is_cert_installed() is False:
@@ -599,19 +680,26 @@
         elif isinstance(e, ConnectionResetError):
             self.connection_err(e, fail_exit)
             return False
         else:
             self.connection_err(e, fail_exit)
             return True
 
+    def stage_0(self):
+        if self.srv.tunnel_type == TunnelType.NO_TUNNEL:
+            self.db.tipping_point(
+                self.srv.current_user, self.srv.current_id,
+                self.srv.current_host, self.srv.current_pass
+            )
+        else:
+            self.db.tipping_point_tunnel(
+                self.srv.profile_name, self.srv.current_user, self.srv.current_id,
+                self.srv.current_host, self.srv.current_pass)
+
     def stage_1(self, c: Connection):
-        self.db.tipping_point(
-            self.srv.current_user, self.srv.current_id,
-            self.srv.current_host, self.srv.current_pass
-        )
         for key in Config.STAGE1:
             self._stage_loop(c, key)
 
     def load_system_paths(self, c: Connection):
         r = c.run("which bash", warn=True, pty=True)
         if str(r.stdout.strip()) != "":
             Config.BASH = str(r.stdout.strip())
@@ -643,23 +731,16 @@
         if task == "docker":
             if self.db.is_docker_ce_installed() is False:
                 if detect_program(c, "docker") is False:
                     install_docker_ce(c)
                     self.db.docker_ce_install()
                 else:
                     print("DOCKER is installed")
-
-        if task == "docker-compose":
-            if self.db.is_docker_compose_installed() is False:
-                if detect_program(c, "docker-compose") is False:
-                    install_docker_compose(c)
-                    self.db.docker_compose_install()
-                else:
-                    print("DOCKER COMPOSE is installed")
-                    check_no_permission(c)
+            else:
+                install_docker_ce(c)
 
         if task == "python":
             if self.db.is_python_installed() is False:
                 if detect_program(c, "python3") is False:
                     print("python3 needs to install")
                     install_python(c)
                     self.db.python3_install()
@@ -667,14 +748,21 @@
         if task == "daed":
             if self.db.is_dae_installed() is False:
                 if detect_program(c, "daed") is False:
                     print("daed will be installed")
                     install_dae_proxy(c)
                     self.db.dae_install()
 
+        if task == "watchtower":
+            if self.db.is_watchtower_installed() is False:
+                if check_docker_ps_specific(c, "containrrr/watchtower") is False:
+                    print("watchtower will be installed - the automatic updates of the docker container")
+                    install_watch_tower(c)
+                    self.db.watchtower_install()
+
         if task == "clash":
             if self.db.is_xclash_installed() is False:
                 if check_docker_ps_specific(c, "dreamacro/clash") is False:
                     print("dreamacro.clash will be installed")
                     if self.install_xclash(1) is True:
                         self.db.docker_clash_install()
             else:
```

### Comparing `machineroom-0.45.3/machineroom/util.py` & `machineroom-0.45.7/machineroom/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -387,39 +387,57 @@
     ...
 
 
 class NodeCountIsNotInPlan(Exception):
     ...
 
 
+class FoundVPNTunnel(Exception):
+    ...
+
+
 class Servers:
     _meta_file: str
     current_id: str
     current_host: str
     current_user: str
     current_pass: str
     _srv_index: int
     _meta_file: int
+    _tunnel_type: TunnelType
+    profile_name: str
+    _on_detect: bool
 
     def __init__(self, file: str):
         self._meta_file = file
         self.serv_count = 20
+        self._tunnel_type = TunnelType.NO_TUNNEL
+        self.profile_name = ""
         self._srv_index = 0
+        self._on_detect = True
 
     @property
     def path_file(self) -> str:
         return os.path.join(Config.DATAPATH_BASE, self._meta_file)
 
     @property
     def at_server(self) -> int:
         return self._srv_index
 
+    @property
+    def tunnel_type(self) -> TunnelType:
+        return self._tunnel_type
+
     def detect_servers(self):
         self.serv_count = read_file_total_lines(self.path_file)
-        self.read_serv_at(0)
+        try:
+            self.read_serv_at(0)
+            self._on_detect = False
+        except FoundVPNTunnel:
+            self.serv_count -= 1
 
     def read_serv_at(self, index: int) -> dict:
         n = index % self.serv_count
         line = read_file_at_line(self.path_file, n)
         if "----" in line:
             line = line.split("----")
         elif "---" in line:
@@ -430,29 +448,37 @@
             line = line.split("————")
         elif "——" in line:
             line = line.split("——")
         if isinstance(line, str):
             raise ServerAuthInfoErr()
 
         self._srv_index = n
+        if index == 0 and "#" in line[0]:
+            VPN_TUNNEL = line[1]
+            print(f"Detected tunnel for machine group {line[0]} using {VPN_TUNNEL}")
+            self._tunnel_type = TunnelType.Recongize(VPN_TUNNEL)
+            self.profile_name = line[0].replace("#", "")
+            raise FoundVPNTunnel()
+
         tmp = {
             "id": line[0],
             "ip": line[1],
             "user": line[2],
             "pass": line[3]
         }
         self.current_id = line[0]
         self.current_host = line[1]
         self.current_user = line[2]
         self.current_pass = line[3]
-        print(f"## ☎️ Now enter network ID#{n}: {line[0]} {line[1]}")
+        if self._on_detect is False:
+            print(f"## ☎️ Now enter network ID#{n}: {line[0]} {line[1]}")
         return tmp
 
-    def use_next_node(self) -> dict:
-        self._srv_index = self._srv_index + 1
+    def use_next_node(self, x: int = 1) -> dict:
+        self._srv_index = self._srv_index + x
         return self.read_serv_at(self._srv_index)
 
 
 class InfrastructurePlannerFoundation:
     # total running nodes on this KVM
     nodes: int
     # the total steps is always 1+
```

### Comparing `machineroom-0.45.3/machineroom.egg-info/PKG-INFO` & `machineroom-0.45.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.45.3
+Version: 0.45.7
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
@@ -14,109 +14,145 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: SQLiteAsJSON
+Requires-Dist: fabric
+Requires-Dist: pexpect
 
-# Machine Room Management on my console
+Machine Room Management on my console
+=====================================
 
 Locate and manage all my machines on my console.
 
-## Introduction
+Introduction
+------------
 
-Congratulations on utilizing technology to improve your machine room management! Having a machine room management app on your console, easily accessible at your fingertips, is a game-changer. It streamlines processes, increases efficiency, and allows you to stay on top of everything with ease. By taking advantage of this tool, you are not only simplifying your workload but also paving the way for future success. Keep up the great work and continue to embrace innovation in your everyday tasks. You've got this!
+Congratulations on utilizing technology to improve your machine room
+management! Having a machine room management app on your console, easily
+accessible at your fingertips, is a game-changer. It streamlines
+processes, increases efficiency, and allows you to stay on top of
+everything with ease. By taking advantage of this tool, you are not only
+simplifying your workload but also paving the way for future success.
+Keep up the great work and continue to embrace innovation in your
+everyday tasks. You’ve got this!
+
+Why
+---
+
+1. Improved efficiency: By having all machines located and managed on
+   one console, you can easily track and monitor their performance,
+   making it easier to identify and address issues quickly. This can
+   help to prevent downtime and keep your operations running smoothly.
+
+2. Centralized control: Having all machines on one console allows for
+   centralized control and management, making it easier to implement
+   changes, updates, or maintenance tasks across all machines
+   simultaneously.
+
+3. Increased visibility: With all machines located on one console, you
+   have greater visibility into the status and performance of each
+   machine, allowing you to make more informed decisions and better plan
+   for maintenance and upgrades.
+
+4. Enhanced security: Centralized management of all machines can help to
+   improve security by providing better oversight of access controls,
+   security settings, and compliance with policies and regulations.
+
+5. Cost savings: Managing all machines on one console can help to reduce
+   operational costs by streamlining processes, improving efficiency,
+   and reducing the need for manual intervention.
+
+6. Scalability: As your operations grow, having all machines on one
+   console makes it easier to scale up and add new machines, without the
+   need for additional management tools or resources.
+
+7. Improved collaboration: Centralized management of all machines can
+   facilitate better collaboration among team members, as everyone can
+   access the same data, reports, and tools from one console.
 
-## Why
+Installation
+------------
 
-1. Improved efficiency: By having all machines located and managed on one console, you can easily track and monitor their performance, making it easier to identify and address issues quickly. This can help to prevent downtime and keep your operations running smoothly.
+There are no requirements for this tool.
 
-2. Centralized control: Having all machines on one console allows for centralized control and management, making it easier to implement changes, updates, or maintenance tasks across all machines simultaneously.
+::
 
-3. Increased visibility: With all machines located on one console, you have greater visibility into the status and performance of each machine, allowing you to make more informed decisions and better plan for maintenance and upgrades.
+   pip3 install machineroom
 
-4. Enhanced security: Centralized management of all machines can help to improve security by providing better oversight of access controls, security settings, and compliance with policies and regulations.
+or if you want to get the upgrade
 
-5. Cost savings: Managing all machines on one console can help to reduce operational costs by streamlining processes, improving efficiency, and reducing the need for manual intervention.
+::
 
-6. Scalability: As your operations grow, having all machines on one console makes it easier to scale up and add new machines, without the need for additional management tools or resources.
+   sudo pip3 install machineroom --upgrade
 
-7. Improved collaboration: Centralized management of all machines can facilitate better collaboration among team members, as everyone can access the same data, reports, and tools from one console.
+Create bin file for easy execution
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+on macosx
 
-## Installation
+::
 
-There are no requirements for this tool.
+   #!/Library/Frameworks/Python.framework/Versions/3.11/bin/python3.11
+   # -*- coding: utf-8 -*-
 
-```
-pip3 install machineroom
-```
 
-or if you want to get the upgrade
-
-```
-sudo pip3 install machineroom --upgrade
-```
+   # setup your desired configuration path in the local machine
+   import machineroom.const.Config
+   Config.DATAPATH_BASE = "...."
+   Config.PUB_KEY = "...."
 
-### Create bin file for easy execution
-on macosx
-```
-#!/Library/Frameworks/Python.framework/Versions/3.11/bin/python3.11
-# -*- coding: utf-8 -*-
 
+   from machineroom.worker import internal_work
 
-# setup your desired configuration path in the local machine
-import machineroom.const.Config
-Config.DATAPATH_BASE = "...."
-Config.PUB_KEY = "...."
+   if __name__ == '__main__':
+       internal_work()
 
+The configurations are available as below
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-from machineroom.worker import internal_work
+::
 
-if __name__ == '__main__':
-    internal_work()
+   DATAPATH_BASE = "...._file....locator"
+   TEMP_FILE = "tmp.txt"
+   TEMP_JS = "tmp.js"
+   REMOTE_WS = "...remote_locator"
+   RAM_GB_REQUIREMENT = 4
+   PUB_KEY = "/Users/xxxx/.ssh/id_rsa.pub"
+   LOCAL_KEY_HOLDER = "/Users/xxxx/.ssh"
+   MY_KEY_FEATURE = "xxxx@xxxxx"
+   REMOTE_HOME = "/root"
+   DOCKER_COMPOSE_VERSION = "2.24.6"
 
+Usage
+-----
 
-```
-### The configurations are available as below
+::
 
-```
-DATAPATH_BASE = "...._file....locator"
-TEMP_FILE = "tmp.txt"
-TEMP_JS = "tmp.js"
-REMOTE_WS = "...remote_locator"
-RAM_GB_REQUIREMENT = 4
-PUB_KEY = "/Users/xxxx/.ssh/id_rsa.pub"
-LOCAL_KEY_HOLDER = "/Users/xxxx/.ssh"
-MY_KEY_FEATURE = "xxxx@xxxxx"
-REMOTE_HOME = "/root"
-DOCKER_COMPOSE_VERSION = "2.24.6"
-```
+   usage: connect [-h] [server id]
 
-## Usage
+   optional arguments:
+     -h, --help            Show this help message and exit
+     -ls,                  Show a list of the existing servers in my list
+     -scan,                Scan the existing server in the access list for health check
+     -import, --from       the import list of the server file within the given format
 
-```
-usage: connect [-h] [server id]
+Example
+~~~~~~~
 
-optional arguments:
-  -h, --help            Show this help message and exit
-  -ls,                  Show a list of the existing servers in my list
-  -scan,                Scan the existing server in the access list for health check
-  -import, --from       the import list of the server file within the given format
-```
+::
 
-### Example
+   connect serverabc
 
-```
-connect serverabc
-```
 connect the console to the existing machine in ssh
 
-```
-connect ls
-```
+::
 
+   connect ls
 
-### License
+License
+~~~~~~~
 
 MIT License (2022), Jun-You Liu, Heskemo BTC
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `machineroom-0.45.3/setup.py` & `machineroom-0.45.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,19 +17,20 @@
 
 import codecs
 import os
 import platform
 
 from setuptools import find_packages
 from setuptools import setup
+import pypandoc
 
 
 def find_version() -> str:
     f = codecs.open('version', 'r', 'utf-8-sig')
-    new_ver = f.readline().strip()
+    new_ver = f.readline().strip().replace("\n", "")
     f.close()
     edit_at_line(new_ver)
     return new_ver
 
 
 def edit_at_line(version: str):
     file = 'machineroom/__init__.py'
@@ -45,46 +46,45 @@
             o += 1
     if len(lines) > 0:
         with open(file, "w") as f:
             f.write("".join(lines))
             f.close()
 
 
-with open('README.md', 'r') as f:
-    long_description = f.read()
-
 _dir = os.path.dirname(__file__)
 py_version = platform.python_version()
 
 setup(
     name='machineroom',
     packages=find_packages(),
     description='A Python package to manage all my machines in the fingertip.',
-    long_description=long_description,
+    long_description=pypandoc.convert_file(os.path.join('README.md'), 'rst'),
     long_description_content_type='text/markdown',
     include_package_data=False,
     package_data={'': ['*.json']},
     author='Jun-You Liu & Heskemo',
     author_email='meowmeow@gmail.com',
     url='https://github.com/jjhesk/mymachineroom/',
     version=find_version(),
     license='MIT',
     keywords='ssh machine room',
-    install_requires=[],
+    install_requires=[
+        'SQLiteAsJSON', 'fabric', 'pexpect',
+    ],
     # py_modules=['bin/connect'],
     python_requires='>=3.8,<4',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Topic :: Software Development :: Code Generators',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ],
     entry_points={
         'console_scripts': [
-            #      'connect = mymachine.cmdbin:cli',
+            # 'connect = mymachine.cmdbin:cli',
         ],
     },
 )
```

### Comparing `machineroom-0.45.3/update` & `machineroom-0.45.7/update`

 * *Files identical despite different names*

