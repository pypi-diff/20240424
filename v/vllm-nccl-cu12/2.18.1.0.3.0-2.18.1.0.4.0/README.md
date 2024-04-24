# Comparing `tmp/vllm_nccl_cu12-2.18.1.0.3.0.tar.gz` & `tmp/vllm_nccl_cu12-2.18.1.0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vllm_nccl_cu12-2.18.1.0.3.0.tar", last modified: Wed Apr 17 04:54:53 2024, max compression
+gzip compressed data, was "vllm_nccl_cu12-2.18.1.0.4.0.tar", last modified: Wed Apr 24 16:48:52 2024, max compression
```

## Comparing `vllm_nccl_cu12-2.18.1.0.3.0.tar` & `vllm_nccl_cu12-2.18.1.0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-17 04:54:53.250613 vllm_nccl_cu12-2.18.1.0.3.0/
--rw-r--r--   0 youkaichao   (501) staff       (20)    11357 2024-04-02 16:28:30.000000 vllm_nccl_cu12-2.18.1.0.3.0/LICENSE
--rw-r--r--   0 youkaichao   (501) staff       (20)       87 2024-04-17 04:54:53.250401 vllm_nccl_cu12-2.18.1.0.3.0/PKG-INFO
--rw-r--r--   0 youkaichao   (501) staff       (20)      164 2024-04-03 20:59:04.000000 vllm_nccl_cu12-2.18.1.0.3.0/README.md
--rw-r--r--   0 youkaichao   (501) staff       (20)       38 2024-04-17 04:54:53.250654 vllm_nccl_cu12-2.18.1.0.3.0/setup.cfg
--rw-r--r--   0 youkaichao   (501) staff       (20)     3417 2024-04-17 04:54:49.000000 vllm_nccl_cu12-2.18.1.0.3.0/setup.py
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-17 04:54:53.249767 vllm_nccl_cu12-2.18.1.0.3.0/vllm_nccl/
--rw-r--r--   0 youkaichao   (501) staff       (20)        0 2024-04-02 17:29:00.000000 vllm_nccl_cu12-2.18.1.0.3.0/vllm_nccl/__init__.py
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-17 04:54:53.250232 vllm_nccl_cu12-2.18.1.0.3.0/vllm_nccl_cu12.egg-info/
--rw-r--r--   0 youkaichao   (501) staff       (20)       87 2024-04-17 04:54:53.000000 vllm_nccl_cu12-2.18.1.0.3.0/vllm_nccl_cu12.egg-info/PKG-INFO
--rw-r--r--   0 youkaichao   (501) staff       (20)      200 2024-04-17 04:54:53.000000 vllm_nccl_cu12-2.18.1.0.3.0/vllm_nccl_cu12.egg-info/SOURCES.txt
--rw-r--r--   0 youkaichao   (501) staff       (20)        1 2024-04-17 04:54:53.000000 vllm_nccl_cu12-2.18.1.0.3.0/vllm_nccl_cu12.egg-info/dependency_links.txt
--rw-r--r--   0 youkaichao   (501) staff       (20)       10 2024-04-17 04:54:53.000000 vllm_nccl_cu12-2.18.1.0.3.0/vllm_nccl_cu12.egg-info/top_level.txt
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-24 16:48:52.291713 vllm_nccl_cu12-2.18.1.0.4.0/
+-rw-r--r--   0 youkaichao   (501) staff       (20)    11357 2024-04-02 16:28:30.000000 vllm_nccl_cu12-2.18.1.0.4.0/LICENSE
+-rw-r--r--   0 youkaichao   (501) staff       (20)       87 2024-04-24 16:48:52.291569 vllm_nccl_cu12-2.18.1.0.4.0/PKG-INFO
+-rw-r--r--   0 youkaichao   (501) staff       (20)      164 2024-04-03 20:59:04.000000 vllm_nccl_cu12-2.18.1.0.4.0/README.md
+-rw-r--r--   0 youkaichao   (501) staff       (20)       38 2024-04-24 16:48:52.291762 vllm_nccl_cu12-2.18.1.0.4.0/setup.cfg
+-rw-r--r--   0 youkaichao   (501) staff       (20)     3447 2024-04-24 16:48:48.000000 vllm_nccl_cu12-2.18.1.0.4.0/setup.py
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-24 16:48:52.290893 vllm_nccl_cu12-2.18.1.0.4.0/vllm_nccl/
+-rw-r--r--   0 youkaichao   (501) staff       (20)        0 2024-04-02 17:29:00.000000 vllm_nccl_cu12-2.18.1.0.4.0/vllm_nccl/__init__.py
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-24 16:48:52.291372 vllm_nccl_cu12-2.18.1.0.4.0/vllm_nccl_cu12.egg-info/
+-rw-r--r--   0 youkaichao   (501) staff       (20)       87 2024-04-24 16:48:52.000000 vllm_nccl_cu12-2.18.1.0.4.0/vllm_nccl_cu12.egg-info/PKG-INFO
+-rw-r--r--   0 youkaichao   (501) staff       (20)      200 2024-04-24 16:48:52.000000 vllm_nccl_cu12-2.18.1.0.4.0/vllm_nccl_cu12.egg-info/SOURCES.txt
+-rw-r--r--   0 youkaichao   (501) staff       (20)        1 2024-04-24 16:48:52.000000 vllm_nccl_cu12-2.18.1.0.4.0/vllm_nccl_cu12.egg-info/dependency_links.txt
+-rw-r--r--   0 youkaichao   (501) staff       (20)       10 2024-04-24 16:48:52.000000 vllm_nccl_cu12-2.18.1.0.4.0/vllm_nccl_cu12.egg-info/top_level.txt
```

### Comparing `vllm_nccl_cu12-2.18.1.0.3.0/LICENSE` & `vllm_nccl_cu12-2.18.1.0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vllm_nccl_cu12-2.18.1.0.3.0/setup.py` & `vllm_nccl_cu12-2.18.1.0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         for chunk in iter(lambda: f.read(4096), b""):  # Read file in 4KB chunks
             hash_md5.update(chunk)  # Update the hash with the chunk
     return hash_md5.hexdigest()  # Return the final hash as a hexadecimal string
 
 package_name = "vllm_nccl_cu12"
 cuda_name = package_name[-4:]
 nccl_version = "2.18.1"
-vllm_nccl_verion = "0.3.0"
+vllm_nccl_verion = "0.4.0"
 version = ".".join([nccl_version, vllm_nccl_verion])
 
 file_hash = {
     "cu11": "5129e4e7e671cc7ce072aaeea870bee8",
     "cu12": "296c4de7fbdb0f7fd8501fb63bd0cb40",
 }[cuda_name]
 
@@ -83,12 +83,14 @@
     if get_md5_hash(destination) != file_hash:
         print(f"md5 hash of downloaded file does not match expected hash, retrying")
         os.remove(destination)
     else:
         print(f"md5 hash of downloaded file matches expected hash")
         break
 
+os.chmod(destination, 0o777)
+
 setup(
     name=package_name,
     version=version,
     packages=["vllm_nccl"],
 )
```

