# Comparing `tmp/datamana-0.0.8.tar.gz` & `tmp/datamana-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamana-0.0.8.tar", last modified: Sun Apr 21 08:41:46 2024, max compression
+gzip compressed data, was "datamana-0.0.9.tar", last modified: Wed Apr 24 14:56:01 2024, max compression
```

## Comparing `datamana-0.0.8.tar` & `datamana-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:41:46.795148 datamana-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-21 08:41:40.000000 datamana-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-21 08:41:40.000000 datamana-0.0.8/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 08:41:40.000000 datamana-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-21 08:41:40.000000 datamana-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-21 08:41:46.795148 datamana-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 08:41:40.000000 datamana-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:41:46.795148 datamana-0.0.8/csrc/
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-21 08:41:40.000000 datamana-0.0.8/csrc/mqueue.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-21 08:41:40.000000 datamana-0.0.8/csrc/python.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-21 08:41:40.000000 datamana-0.0.8/csrc/semaphore.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:41:46.795148 datamana-0.0.8/datamana/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 08:41:40.000000 datamana-0.0.8/datamana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 08:41:40.000000 datamana-0.0.8/datamana/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-21 08:41:40.000000 datamana-0.0.8/datamana/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:41:46.795148 datamana-0.0.8/datamana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-21 08:41:46.000000 datamana-0.0.8/datamana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-21 08:41:46.000000 datamana-0.0.8/datamana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 08:41:46.000000 datamana-0.0.8/datamana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 08:41:46.000000 datamana-0.0.8/datamana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 08:41:46.000000 datamana-0.0.8/datamana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-21 08:41:40.000000 datamana-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 08:41:46.795148 datamana-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-21 08:41:40.000000 datamana-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:56:01.555075 datamana-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-24 14:55:48.000000 datamana-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-24 14:55:48.000000 datamana-0.0.9/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-24 14:55:48.000000 datamana-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-24 14:55:48.000000 datamana-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-24 14:56:01.555075 datamana-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 14:55:48.000000 datamana-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:56:01.555075 datamana-0.0.9/csrc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-24 14:55:48.000000 datamana-0.0.9/csrc/mqueue.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-24 14:55:48.000000 datamana-0.0.9/csrc/python.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-24 14:55:48.000000 datamana-0.0.9/csrc/semaphore.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:56:01.555075 datamana-0.0.9/datamana/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 14:55:48.000000 datamana-0.0.9/datamana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 14:55:48.000000 datamana-0.0.9/datamana/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-24 14:55:48.000000 datamana-0.0.9/datamana/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:56:01.555075 datamana-0.0.9/datamana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-24 14:56:01.000000 datamana-0.0.9/datamana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-24 14:56:01.000000 datamana-0.0.9/datamana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:56:01.000000 datamana-0.0.9/datamana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 14:56:01.000000 datamana-0.0.9/datamana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 14:56:01.000000 datamana-0.0.9/datamana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-24 14:55:48.000000 datamana-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:56:01.555075 datamana-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-24 14:55:48.000000 datamana-0.0.9/setup.py
```

### Comparing `datamana-0.0.8/.gitignore` & `datamana-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `datamana-0.0.8/CMakeLists.txt` & `datamana-0.0.9/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `datamana-0.0.8/LICENSE` & `datamana-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `datamana-0.0.8/PKG-INFO` & `datamana-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamana
-Version: 0.0.8
+Version: 0.0.9
 Summary: Dataset Manager
 Author-email: Jiau Zhang <jiauzhang@163.com>
 Project-URL: Homepage, https://github.com/jiauzhang/datamana
 Keywords: Deep Learning,Dataset Manager,Artificial Intelligence
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamana-0.0.8/csrc/mqueue.hpp` & `datamana-0.0.9/csrc/mqueue.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -9,35 +9,47 @@
 struct MQueue {
     mqd_t mqd;
     struct mq_attr attr;
 
     MQueue() : mqd((mqd_t)-1) {}
 
     int py_mq_open(const char *name, int oflag, unsigned int mode) {
+        mode_t omask = umask(0);
         mqd = mq_open(name, oflag, (mode_t)mode, &attr);
-        if (mqd == (mqd_t)-1) {
-            return errno;
-        } else {
-            return 0;
-        }
+        umask(omask);
+        int ret = 0;
+        if (mqd == (mqd_t)-1)
+            ret = errno;
+        return ret;
     }
     int py_mq_unlink(const char *name) {
-        return mq_unlink(name);
+        int ret = mq_unlink(name);
+        if (ret == -1)
+            ret = errno;
+        return ret;
     }
     int py_mq_close() {
-        return mq_close(mqd);
+        int ret = mq_close(mqd);
+        if (ret == -1)
+            ret = errno;
+        return ret;
     }
     int py_mq_send(std::string &msg, unsigned int msg_prio) {
-        return mq_send(mqd, (const char *)msg.c_str(), msg.size(), msg_prio);
+        int ret = mq_send(mqd, (const char *)msg.c_str(), msg.size(), msg_prio);
+        if (ret == -1)
+            ret = errno;
+        return ret;
     }
-    std::string py_mq_receive() {
+    int py_mq_receive(std::string &msg) {
         unsigned int msg_prio;
-        std::string msg(32, '\0');
-        mq_receive(mqd, (char *)msg.c_str(), msg.size(), &msg_prio);
-        return msg;
+        msg.resize(attr.mq_msgsize);
+        int ret = mq_receive(mqd, (char *)msg.c_str(), msg.size(), &msg_prio);
+        if (ret == -1)
+            ret = errno;
+        return ret;
     }
 };
 
 void DEFINE_MQUEUE_MODULE(nb::module_ & (m)) {
     nb::class_<MQueue>(m, "MQueue")
         .def(nb::init<>())
         .def("open", &MQueue::py_mq_open)
```

### Comparing `datamana-0.0.8/csrc/semaphore.hpp` & `datamana-0.0.9/csrc/semaphore.hpp`

 * *Files identical despite different names*

### Comparing `datamana-0.0.8/datamana/torch.py` & `datamana-0.0.9/datamana/torch.py`

 * *Files identical despite different names*

### Comparing `datamana-0.0.8/datamana.egg-info/PKG-INFO` & `datamana-0.0.9/datamana.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamana
-Version: 0.0.8
+Version: 0.0.9
 Summary: Dataset Manager
 Author-email: Jiau Zhang <jiauzhang@163.com>
 Project-URL: Homepage, https://github.com/jiauzhang/datamana
 Keywords: Deep Learning,Dataset Manager,Artificial Intelligence
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamana-0.0.8/pyproject.toml` & `datamana-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "cmake >= 3.15",
     "nanobind >= 1.9.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datamana"
-version = "0.0.8"
+version = "0.0.9"
 description = "Dataset Manager"
 readme = "README.md"
 authors = [
     {name = "Jiau Zhang", email = "jiauzhang@163.com"},
 ]
 classifiers = [
     'Intended Audience :: Developers',
```

### Comparing `datamana-0.0.8/setup.py` & `datamana-0.0.9/setup.py`

 * *Files identical despite different names*

