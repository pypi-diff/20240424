# Comparing `tmp/imgtool-2.0.0.tar.gz` & `tmp/imgtool-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgtool-2.0.0.tar", last modified: Mon Oct 23 23:53:11 2023, max compression
+gzip compressed data, was "imgtool-2.0.0rc1.tar", last modified: Fri Sep 29 14:19:27 2023, max compression
```

## Comparing `imgtool-2.0.0.tar` & `imgtool-2.0.0rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 23:53:11.372480 imgtool-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2023-10-23 23:53:11.372480 imgtool-2.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 23:53:11.368480 imgtool-2.0.0/imgtool/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2023-10-23 23:53:04.000000 imgtool-2.0.0/imgtool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2023-10-23 23:53:04.000000 imgtool-2.0.0/imgtool/boot_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    11063 2023-10-23 23:53:04.000000 imgtool-2.0.0/imgtool/dumpinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    27833 2023-10-23 23:53:04.000000 imgtool-2.0.0/imgtool/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 23:53:11.372480 imgtool-2.0.0/imgtool/keys/
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2023-10-23 23:53:04.000000 imgtool-2.0.0/imgtool/keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9492 2023-10-23 23:53:04.000000 imgtool-2.0.0/imgtool/keys/ecdsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2023-10-23 23:53:04.000000 imgtool-2.0.0/imgtool/keys/ecdsa_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2023-10-23 23:53:04.000000 imgtool-2.0.0/imgtool/keys/ed25519.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2023-10-23 23:53:04.000000 imgtool-2.0.0/imgtool/keys/ed25519_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2023-10-23 23:53:04.000000 imgtool-2.0.0/imgtool/keys/general.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2023-10-23 23:53:04.000000 imgtool-2.0.0/imgtool/keys/privatebytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2023-10-23 23:53:04.000000 imgtool-2.0.0/imgtool/keys/rsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2023-10-23 23:53:04.000000 imgtool-2.0.0/imgtool/keys/rsa_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2023-10-23 23:53:04.000000 imgtool-2.0.0/imgtool/keys/x25519.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21110 2023-10-23 23:53:04.000000 imgtool-2.0.0/imgtool/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2023-10-23 23:53:04.000000 imgtool-2.0.0/imgtool/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 23:53:11.372480 imgtool-2.0.0/imgtool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2023-10-23 23:53:11.000000 imgtool-2.0.0/imgtool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      559 2023-10-23 23:53:11.000000 imgtool-2.0.0/imgtool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-23 23:53:11.000000 imgtool-2.0.0/imgtool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-10-23 23:53:11.000000 imgtool-2.0.0/imgtool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-23 23:53:11.000000 imgtool-2.0.0/imgtool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-23 23:53:11.000000 imgtool-2.0.0/imgtool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-23 23:53:11.372480 imgtool-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      898 2023-10-23 23:53:04.000000 imgtool-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 14:19:27.054290 imgtool-2.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2023-09-29 14:19:27.054290 imgtool-2.0.0rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 14:19:27.050290 imgtool-2.0.0rc1/imgtool/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2023-09-29 14:19:21.000000 imgtool-2.0.0rc1/imgtool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2023-09-29 14:19:21.000000 imgtool-2.0.0rc1/imgtool/boot_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11063 2023-09-29 14:19:21.000000 imgtool-2.0.0rc1/imgtool/dumpinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27833 2023-09-29 14:19:21.000000 imgtool-2.0.0rc1/imgtool/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 14:19:27.054290 imgtool-2.0.0rc1/imgtool/keys/
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2023-09-29 14:19:21.000000 imgtool-2.0.0rc1/imgtool/keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9492 2023-09-29 14:19:21.000000 imgtool-2.0.0rc1/imgtool/keys/ecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2023-09-29 14:19:21.000000 imgtool-2.0.0rc1/imgtool/keys/ecdsa_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2023-09-29 14:19:21.000000 imgtool-2.0.0rc1/imgtool/keys/ed25519.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2023-09-29 14:19:21.000000 imgtool-2.0.0rc1/imgtool/keys/ed25519_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2023-09-29 14:19:21.000000 imgtool-2.0.0rc1/imgtool/keys/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2023-09-29 14:19:21.000000 imgtool-2.0.0rc1/imgtool/keys/privatebytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2023-09-29 14:19:21.000000 imgtool-2.0.0rc1/imgtool/keys/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2023-09-29 14:19:21.000000 imgtool-2.0.0rc1/imgtool/keys/rsa_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2023-09-29 14:19:21.000000 imgtool-2.0.0rc1/imgtool/keys/x25519.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21110 2023-09-29 14:19:21.000000 imgtool-2.0.0rc1/imgtool/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2023-09-29 14:19:21.000000 imgtool-2.0.0rc1/imgtool/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 14:19:27.054290 imgtool-2.0.0rc1/imgtool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2023-09-29 14:19:26.000000 imgtool-2.0.0rc1/imgtool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2023-09-29 14:19:27.000000 imgtool-2.0.0rc1/imgtool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-29 14:19:26.000000 imgtool-2.0.0rc1/imgtool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2023-09-29 14:19:26.000000 imgtool-2.0.0rc1/imgtool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-09-29 14:19:26.000000 imgtool-2.0.0rc1/imgtool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-09-29 14:19:26.000000 imgtool-2.0.0rc1/imgtool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-29 14:19:27.054290 imgtool-2.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2023-09-29 14:19:21.000000 imgtool-2.0.0rc1/setup.py
```

### Comparing `imgtool-2.0.0/imgtool/__init__.py` & `imgtool-2.0.0rc1/imgtool/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-imgtool_version = "2.0.0"
+imgtool_version = "2.0.0rc1"
```

### Comparing `imgtool-2.0.0/imgtool/boot_record.py` & `imgtool-2.0.0rc1/imgtool/boot_record.py`

 * *Files identical despite different names*

### Comparing `imgtool-2.0.0/imgtool/dumpinfo.py` & `imgtool-2.0.0rc1/imgtool/dumpinfo.py`

 * *Files identical despite different names*

### Comparing `imgtool-2.0.0/imgtool/image.py` & `imgtool-2.0.0rc1/imgtool/image.py`

 * *Files identical despite different names*

### Comparing `imgtool-2.0.0/imgtool/keys/__init__.py` & `imgtool-2.0.0rc1/imgtool/keys/__init__.py`

 * *Files identical despite different names*

### Comparing `imgtool-2.0.0/imgtool/keys/ecdsa.py` & `imgtool-2.0.0rc1/imgtool/keys/ecdsa.py`

 * *Files identical despite different names*

### Comparing `imgtool-2.0.0/imgtool/keys/ecdsa_test.py` & `imgtool-2.0.0rc1/imgtool/keys/ecdsa_test.py`

 * *Files identical despite different names*

### Comparing `imgtool-2.0.0/imgtool/keys/ed25519.py` & `imgtool-2.0.0rc1/imgtool/keys/ed25519.py`

 * *Files identical despite different names*

### Comparing `imgtool-2.0.0/imgtool/keys/ed25519_test.py` & `imgtool-2.0.0rc1/imgtool/keys/ed25519_test.py`

 * *Files identical despite different names*

### Comparing `imgtool-2.0.0/imgtool/keys/general.py` & `imgtool-2.0.0rc1/imgtool/keys/general.py`

 * *Files identical despite different names*

### Comparing `imgtool-2.0.0/imgtool/keys/privatebytes.py` & `imgtool-2.0.0rc1/imgtool/keys/privatebytes.py`

 * *Files identical despite different names*

### Comparing `imgtool-2.0.0/imgtool/keys/rsa.py` & `imgtool-2.0.0rc1/imgtool/keys/rsa.py`

 * *Files identical despite different names*

### Comparing `imgtool-2.0.0/imgtool/keys/rsa_test.py` & `imgtool-2.0.0rc1/imgtool/keys/rsa_test.py`

 * *Files identical despite different names*

### Comparing `imgtool-2.0.0/imgtool/keys/x25519.py` & `imgtool-2.0.0rc1/imgtool/keys/x25519.py`

 * *Files identical despite different names*

### Comparing `imgtool-2.0.0/imgtool/main.py` & `imgtool-2.0.0rc1/imgtool/main.py`

 * *Files identical despite different names*

### Comparing `imgtool-2.0.0/imgtool/version.py` & `imgtool-2.0.0rc1/imgtool/version.py`

 * *Files identical despite different names*

### Comparing `imgtool-2.0.0/imgtool.egg-info/SOURCES.txt` & `imgtool-2.0.0rc1/imgtool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imgtool-2.0.0/setup.py` & `imgtool-2.0.0rc1/setup.py`

 * *Files identical despite different names*

