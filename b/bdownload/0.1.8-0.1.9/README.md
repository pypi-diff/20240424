# Comparing `tmp/bdownload-0.1.8.tar.gz` & `tmp/bdownload-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\bdownload-0.1.8.tar", last modified: Tue Apr  2 15:20:41 2024, max compression
+gzip compressed data, was "dist\bdownload-0.1.9.tar", last modified: Wed Apr 24 16:28:01 2024, max compression
```

## Comparing `bdownload-0.1.8.tar` & `bdownload-0.1.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 15:20:41.000000 bdownload-0.1.8/
--rw-rw-rw-   0        0        0     1035 2024-03-08 08:14:53.000000 bdownload-0.1.8/.readthedocs.yaml
--rw-rw-rw-   0        0        0      702 2024-03-16 15:16:23.000000 bdownload-0.1.8/.travis.yml
-drwxrwxrwx   0        0        0        0 2024-04-02 15:20:41.000000 bdownload-0.1.8/docs/
--rwxrwxrwx   0        0        0      756 2021-11-10 14:24:48.000000 bdownload-0.1.8/docs/make.bat
--rw-rw-rw-   0        0        0      584 2021-11-10 14:24:48.000000 bdownload-0.1.8/docs/Makefile
-drwxrwxrwx   0        0        0        0 2024-04-02 15:20:41.000000 bdownload-0.1.8/docs/source/
--rw-rw-rw-   0        0        0      449 2024-03-15 02:56:16.000000 bdownload-0.1.8/docs/source/bdownload.rst
--rw-rw-rw-   0        0        0      231 2022-02-23 10:08:54.000000 bdownload-0.1.8/docs/source/cli.rst
--rw-rw-rw-   0        0        0     6494 2024-03-08 06:08:09.000000 bdownload-0.1.8/docs/source/conf.py
--rw-rw-rw-   0        0        0     7283 2024-03-15 02:56:16.000000 bdownload-0.1.8/docs/source/index.rst
--rw-rw-rw-   0        0        0      314 2024-03-08 08:14:53.000000 bdownload-0.1.8/docs/source/requirements.txt
--rw-rw-rw-   0        0        0      267 2022-02-23 10:23:42.000000 bdownload-0.1.8/docs/source/test_bdownloader.rst
--rw-rw-rw-   0        0        0      359 2022-02-23 10:23:42.000000 bdownload-0.1.8/docs/source/test_multisource_download.rst
--rw-rw-rw-   0        0        0      178 2024-03-15 02:56:16.000000 bdownload-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0    20720 2024-04-02 15:20:41.000000 bdownload-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    19026 2024-04-02 10:26:45.000000 bdownload-0.1.8/README.md
--rw-rw-rw-   0        0        0      464 2024-03-08 08:14:53.000000 bdownload-0.1.8/requirements.txt
--rw-rw-rw-   0        0        0       58 2024-04-02 15:20:41.000000 bdownload-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     2710 2024-03-16 15:18:02.000000 bdownload-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:20:41.000000 bdownload-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2024-04-02 15:20:41.000000 bdownload-0.1.8/src/bdownload/
--rw-rw-rw-   0        0        0    18170 2024-03-31 08:11:00.000000 bdownload-0.1.8/src/bdownload/cli.py
--rw-rw-rw-   0        0        0    96037 2024-04-02 10:26:45.000000 bdownload-0.1.8/src/bdownload/download.py
--rw-rw-rw-   0        0        0     6157 2024-03-15 02:56:16.000000 bdownload-0.1.8/src/bdownload/utils.py
--rw-rw-rw-   0        0        0        5 2024-04-02 15:10:01.000000 bdownload-0.1.8/src/bdownload/VERSION
--rw-rw-rw-   0        0        0      364 2022-03-05 07:28:46.000000 bdownload-0.1.8/src/bdownload/__init__.py
--rw-rw-rw-   0        0        0      351 2024-03-15 02:56:16.000000 bdownload-0.1.8/src/bdownload/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:20:41.000000 bdownload-0.1.8/tests/
--rw-rw-rw-   0        0        0     4248 2021-11-19 11:24:44.000000 bdownload-0.1.8/tests/test_bdownloader.py
--rw-rw-rw-   0        0        0     1521 2024-03-17 06:34:08.000000 bdownload-0.1.8/tests/test_cli.py
--rw-rw-rw-   0        0        0     3331 2024-03-17 10:05:27.000000 bdownload-0.1.8/tests/test_multisource_download.py
--rw-rw-rw-   0        0        0        0 2021-11-10 14:24:48.000000 bdownload-0.1.8/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:20:41.000000 bdownload-0.1.8/third_parties/
-drwxrwxrwx   0        0        0        0 2024-04-02 15:20:41.000000 bdownload-0.1.8/third_parties/setupext_janitor/
--rw-rw-rw-   0        0        0     7272 2021-11-10 14:24:48.000000 bdownload-0.1.8/third_parties/setupext_janitor/janitor.py
--rw-rw-rw-   0        0        0     5228 2021-11-10 14:24:48.000000 bdownload-0.1.8/third_parties/setupext_janitor/README.rst
--rw-rw-rw-   0        0        0      167 2024-03-16 15:11:35.000000 bdownload-0.1.8/tox.ini
+drwxrwxrwx   0        0        0        0 2024-04-24 16:28:01.000000 bdownload-0.1.9/
+-rw-rw-rw-   0        0        0     1035 2024-03-08 08:14:53.000000 bdownload-0.1.9/.readthedocs.yaml
+-rw-rw-rw-   0        0        0      702 2024-03-16 15:16:23.000000 bdownload-0.1.9/.travis.yml
+drwxrwxrwx   0        0        0        0 2024-04-24 16:28:01.000000 bdownload-0.1.9/docs/
+-rwxrwxrwx   0        0        0      756 2021-11-10 14:24:48.000000 bdownload-0.1.9/docs/make.bat
+-rw-rw-rw-   0        0        0      584 2021-11-10 14:24:48.000000 bdownload-0.1.9/docs/Makefile
+drwxrwxrwx   0        0        0        0 2024-04-24 16:28:01.000000 bdownload-0.1.9/docs/source/
+-rw-rw-rw-   0        0        0      449 2024-03-15 02:56:16.000000 bdownload-0.1.9/docs/source/bdownload.rst
+-rw-rw-rw-   0        0        0      231 2022-02-23 10:08:54.000000 bdownload-0.1.9/docs/source/cli.rst
+-rw-rw-rw-   0        0        0     6494 2024-03-08 06:08:09.000000 bdownload-0.1.9/docs/source/conf.py
+-rw-rw-rw-   0        0        0     8440 2024-04-24 14:26:25.000000 bdownload-0.1.9/docs/source/index.rst
+-rw-rw-rw-   0        0        0      314 2024-03-08 08:14:53.000000 bdownload-0.1.9/docs/source/requirements.txt
+-rw-rw-rw-   0        0        0      267 2022-02-23 10:23:42.000000 bdownload-0.1.9/docs/source/test_bdownloader.rst
+-rw-rw-rw-   0        0        0      359 2022-02-23 10:23:42.000000 bdownload-0.1.9/docs/source/test_multisource_download.rst
+-rw-rw-rw-   0        0        0      178 2024-03-15 02:56:16.000000 bdownload-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    27144 2024-04-24 16:28:01.000000 bdownload-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    21510 2024-04-24 15:43:12.000000 bdownload-0.1.9/README.md
+-rw-rw-rw-   0        0        0      464 2024-03-08 08:14:53.000000 bdownload-0.1.9/requirements.txt
+-rw-rw-rw-   0        0        0       58 2024-04-24 16:28:01.000000 bdownload-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     2710 2024-03-16 15:18:02.000000 bdownload-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:28:01.000000 bdownload-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 16:28:01.000000 bdownload-0.1.9/src/bdownload/
+-rw-rw-rw-   0        0        0    21262 2024-04-17 05:19:12.000000 bdownload-0.1.9/src/bdownload/cli.py
+-rw-rw-rw-   0        0        0   101744 2024-04-24 15:43:12.000000 bdownload-0.1.9/src/bdownload/download.py
+-rw-rw-rw-   0        0        0     6157 2024-03-15 02:56:16.000000 bdownload-0.1.9/src/bdownload/utils.py
+-rw-rw-rw-   0        0        0        5 2024-04-24 16:06:20.000000 bdownload-0.1.9/src/bdownload/VERSION
+-rw-rw-rw-   0        0        0      364 2022-03-05 07:28:46.000000 bdownload-0.1.9/src/bdownload/__init__.py
+-rw-rw-rw-   0        0        0      351 2024-03-15 02:56:16.000000 bdownload-0.1.9/src/bdownload/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:28:01.000000 bdownload-0.1.9/tests/
+-rw-rw-rw-   0        0        0     4248 2021-11-19 11:24:44.000000 bdownload-0.1.9/tests/test_bdownloader.py
+-rw-rw-rw-   0        0        0     1521 2024-03-17 06:34:08.000000 bdownload-0.1.9/tests/test_cli.py
+-rw-rw-rw-   0        0        0     3331 2024-03-17 10:05:27.000000 bdownload-0.1.9/tests/test_multisource_download.py
+-rw-rw-rw-   0        0        0        0 2021-11-10 14:24:48.000000 bdownload-0.1.9/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:28:01.000000 bdownload-0.1.9/third_parties/
+drwxrwxrwx   0        0        0        0 2024-04-24 16:28:01.000000 bdownload-0.1.9/third_parties/setupext_janitor/
+-rw-rw-rw-   0        0        0     7272 2021-11-10 14:24:48.000000 bdownload-0.1.9/third_parties/setupext_janitor/janitor.py
+-rw-rw-rw-   0        0        0     5228 2021-11-10 14:24:48.000000 bdownload-0.1.9/third_parties/setupext_janitor/README.rst
+-rw-rw-rw-   0        0        0      167 2024-03-16 15:11:35.000000 bdownload-0.1.9/tox.ini
```

### Comparing `bdownload-0.1.8/.readthedocs.yaml` & `bdownload-0.1.9/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bdownload-0.1.8/.travis.yml` & `bdownload-0.1.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `bdownload-0.1.8/docs/make.bat` & `bdownload-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bdownload-0.1.8/docs/Makefile` & `bdownload-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bdownload-0.1.8/docs/source/conf.py` & `bdownload-0.1.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bdownload-0.1.8/docs/source/index.rst` & `bdownload-0.1.9/docs/source/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -49,23 +49,23 @@
 -------------------------------
 Synopsis
 ^^^^^^^^
 .. code-block:: shell
 
     bdownload      url | -L URLS [URLS ...]
                    [-O OUTPUT | -o OUTPUT [OUTPUT ...]] [-D DIR]
-                   [-p PROXY] [-n MAX_WORKERS] [-k MIN_SPLIT_SIZE]
-                   [-s CHUNK_SIZE] [-e COOKIE] [--user-agent USER_AGENT]
-                   [--referrer REFERRER]
+                   [-p PROXY] [-n MAX_WORKERS] [-j MAX_PARALLEL_DOWNLOADS]
+                   [-J WORKERS_PER_DOWNLOAD] [-k MIN_SPLIT_SIZE] [-s CHUNK_SIZE]
+                   [-e COOKIE] [--user-agent USER_AGENT] [--referrer REFERRER]
                    [--check-certificate {True,true,TRUE,False,false,FALSE}]
                    [--ca-certificate CA_CERTIFICATE]
                    [--certificate CERTIFICATE] [--private-key PRIVATE_KEY]
                    [-P {mill,bar,none}] [--num-pools NUM_POOLS]
                    [--pool-size POOL_SIZE] [-l {debug,info,warning,error,critical}]
-                   [-c | --no-continue]
+                   [-c | --no-continue] [-H HEADER] [-u USER_PASS] [--netrc-file NETRC_FILE]
                    [-h]
 
 Description
 ^^^^^^^^^^^
 
 ``url``
 
@@ -93,32 +93,40 @@
 
 ``-D DIR, --dir DIR``
 
     directory in which to save the downloaded files [default: directory in which this App is running]
 
 ``-p PROXY, --proxy PROXY``
 
-    proxy either in the form of "http://[user:pass@]host:port" or "socks5://[user:pass@]host:port"
+    proxy either in the form of "`http://[user:pass@]host:port`" or "`socks5://[user:pass@]host:port`"
 
 ``-n MAX_WORKERS, --max-workers MAX_WORKERS``
 
     number of worker threads [default: 20]
 
+``-j MAX_PARALLEL_DOWNLOADS, --max-parallel-downloads MAX_PARALLEL_DOWNLOADS``
+
+    number of files downloading concurrently [default: 5]
+
+``-J WORKERS_PER_DOWNLOAD, --workers-per-download WORKERS_PER_DOWNLOAD``
+
+    number of worker threads for every file downloading job [default: 4]
+
 ``-k MIN_SPLIT_SIZE, --min-split-size MIN_SPLIT_SIZE``
 
     file split size in bytes, "1048576, 1024K or 2M" for example [default: 1M]
 
 ``-s CHUNK_SIZE, --chunk-size CHUNK_SIZE``
 
     every request range size in bytes, "10240, 10K or 1M" for example [default: 100K]
 
 ``-e COOKIE, --cookie COOKIE``
 
     cookies either in the form of a string (maybe whitespace- and/or semicolon- separated)
-    like "cookie_key=cookie_value cookie_key2=cookie_value2; cookie_key3=cookie_value3", or a file,
+    like "`cookie_key=cookie_value cookie_key2=cookie_value2; cookie_key3=cookie_value3`", or a file,
     e.g. named "cookies.txt", in the Netscape cookie file format. NB the option ``-D DIR`` does not apply to the cookie file
 
 ``--user-agent USER_AGENT``
 
     custom user agent
 
 ``--referrer REFERRER``
@@ -165,35 +173,51 @@
 
     resume from the partially downloaded files. This is the default behavior
 
 ``--no-continue``
 
     do not resume from last interruption, i.e. start the download from beginning
 
+``-H HEADER, --header HEADER``
+
+    extra HTTP header, standard or custom, which can be repeated several times, e.g.
+    '`-H "User-Agent: John Doe" -H "X-BD-Key: One Thousand And One Nights"`'.The headers take precedence over the ones
+    specified by other parameters if conflict happens
+
+``-u USER_PASS, --user-pass USER_PASS``
+
+    default HTTP Authentication for ALL the downloads in "`user:password`" format. Warning: don't use this option
+    if not all of the downloads need the authentication to avoid leaking credential, use the ``--netrc-file`` option instead
+
+``--netrc-file NETRC_FILE``
+
+    a .netrc-like file for HTTP authentication, from which the 'default' entry, if present, takes precedence over the
+    ``--user-pass`` option
+
 ``-h, --help``
 
     show help message and exit
 
 Examples
 ^^^^^^^^
     ``$ bdownload https://www.afilelink.com/afile.tar.gz``
 
     ``$ bdownload -O /abspath/to/afile.tar.gz https://www.afilelink.com/afile.tar.gz``
 
     ``$ bdownload -O /abspath/to/a/dir/ https://www.afilelink.com/afile.tar.gz``
 
-    ``$ bdownload -O /abspath/to/afile.tar.gz https://www.afilelink.com/afile.tar.gz\thttps://nianpei.bpfatran.com/afile.tar.gz``
+    ``$ bdownload -O /abspath/to/afile.tar.gz "https://www.afilelink.com/afile.tar.gz\thttps://nianpei.bpfatran.com/afile.tar.gz"``
 
     ``$ bdownload -D path/to/working_dir/ -O relpath/to/working_dir/alias_afile.tar.gz https://www.afilelink.com/afile.tar.gz``
 
     ``$ bdownload -D path/to/working/dir https://www.afilelink.com/afile.tar.gz``
 
-    ``$ bdownload -o /abspath/to/file1.zip ~/file2.tgz -L http://foo.cc/file1.zip http://bar.cc/file2.tgz\thttp://bar2.cc/file2.tgz``
+    ``$ bdownload -o /abspath/to/file1.zip ~/file2.tgz -L "http://foo.cc/file1.zip" "http://bar.cc/file2.tgz\thttp://bar2.cc/file2.tgz"``
 
-    ``$ bdownload -D path/to/working/dir -L http://foo.cc/file1.zip http://bar.cc/file2.tgz\thttp://bar2.cc/file2.tgz``
+    ``$ bdownload -D path/to/working/dir -L "http://foo.cc/file1.zip" "http://bar.cc/file2.tgz\thttp://bar2.cc/file2.tgz"``
 
 .. _API indices:
 
 API indices
 ===========
 .. toctree::
    :maxdepth: 2
```

### Comparing `bdownload-0.1.8/PKG-INFO` & `bdownload-0.1.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,502 @@
 Metadata-Version: 2.1
 Name: bdownload
-Version: 0.1.8
+Version: 0.1.9
 Summary: A multi-threaded and multi-source aria2-like batch file downloading library for Python
 Home-page: https://github.com/Jesseatgao/bdownload
 Author: Jesse Gao
 Author-email: changxigao@gmail.com
 License: MIT License
+Description: ## bdownload
+        [![Latest Version](https://img.shields.io/pypi/v/bdownload.svg)](https://pypi.org/project/bdownload/)
+        [![Build Status](https://travis-ci.com/Jesseatgao/bdownload.svg?branch=master)](https://travis-ci.com/Jesseatgao/bdownload)
+        [![Supported Versions](https://img.shields.io/pypi/pyversions/bdownload.svg)](https://pypi.org/project/bdownload)
+        
+        A multi-threaded and multi-source aria2-like batch file downloading library for Python 2.7 and 3.6+
+        
+        > **:bulb:**\
+        > See also [https://bdownload.readthedocs.io](https://bdownload.readthedocs.io) for API reference.
+        
+        ### Installation
+        
+        * via PyPI
+        
+            `pip install bdownload`
+        
+        * from within source directory locally
+        
+            `pip install .`
+            
+            Note that you should `git clone` or download the source tarball (and unpack it of course) from the repository first 
+        
+        > **:bulb:**\
+        > For Python2.7: since the version of 2022.5.18, `certifi` has dropped the support for Python2.x. To upgrade to the latest CA
+        > certificates bundle, simply run:
+        > 
+        > `$ bdownload-upd-cacert-py2`
+        
+        ### Usage: as a Python package
+        
+        #### Importing
+        
+            `from bdownload import BDownloader, BDownloaderException`
+        
+                    or
+        
+            `import bdownload`
+        
+        #### Signatures
+        
+        `
+        class bdownload.BDownloader(max_workers=None, max_parallel_downloads=5, workers_per_download=4, min_split_size=1024*1024,
+                                    chunk_size=1024*100, proxy=None, cookies=None, user_agent=None, logger=None, progress='mill',
+                                    num_pools=20, pool_maxsize=20, request_timeout=None, request_retries=None, status_forcelist=None,
+                                    resumption_retries=None, continuation=True, referrer=None, check_certificate=True, ca_certificate=None,
+                                    certificate=None, auth=None, netrc=None, headers=None)
+        `
+        
+            Create and initialize a `BDownloader` object for executing download jobs.
+          
+          * The `max_workers` parameter specifies the number of the parallel downloading threads, whose default value is 
+            determined by _#num_of_processor * 5_ if set to `None`.
+        
+          * `max_parallel_downloads` limits the number of files downloading concurrently. It has a default value of 5.
+        
+          * `workers_per_download` sets the maximum number of worker threads for every file downloading job, which defaults to 4.
+          
+          * `min_split_size` denotes the size in bytes of file pieces split to be downloaded in parallel, which defaults to 
+            1024*1024 bytes (i.e. 1MB).
+          
+          * The `chunk_size` parameter specifies the chunk size in bytes of every http range request, which will take a default 
+            value of 1024*100 (i.e. 100KB) if not provided.
+          
+          * `proxy` supports both HTTP and SOCKS proxies in the form of _http://[user:pass@]host:port_ and 
+            _socks5://[user:pass@]host:port_, respectively.
+          
+          * If `cookies` needs to be set, it must either take the form of _cookie_key=cookie_value_, with multiple pairs separated
+            by whitespace and/or semicolon if applicable, e.g. '_key1=val1 key2=val2;key3=val3_', be packed into a `dict`, or 
+            be an instance of `CookieJar`, i.e. `cookielib.CookieJar` for Python27, `http.cookiejar.CookieJar` for Python3.x or 
+            `RequestsCookieJar` from `requests`.
+            
+            Note that the `ValueError` exception will be raised when the `cookies` is of the `str` type and not in the valid format.
+          
+          * When `user_agent` is not given, it will default to '_bdownload/VERSION_', with _VERSION_ being replaced by the 
+            package's version number.
+          
+          * The `logger` parameter specifies an event logger. If `logger` is not `None`, it must be an object of class 
+            `logging.Logger` or of its customized subclass.  Otherwise, it will use a default module-level logger returned by 
+            `logging.getLogger(__name__)`.
+          
+          * `progress` determines the style of the progress bar displayed while downloading files. Possible values are `'mill'`,
+            `'bar'` and `'none'`. `'mill'` is the default. To disable this feature, e.g. while scripting or multi-instanced, 
+            set it to `'none'`.
+          
+          * The `num_pools` parameter has the same meaning as `num_pools` in `urllib3.PoolManager` and will eventually be passed
+            to it. Specifically, `num_pools` specifies the number of connection pools to cache.
+          
+          * `pool_maxsize` will be passed to the underlying `requests.adapters.HTTPAdapter`. It specifies the maximum number of 
+            connections to save that can be reused in the urllib3 connection pool.
+        
+          * The `request_timeout` parameter specifies the timeouts for the internal `requests` session. The timeout value(s) 
+            as a float or `(connect, read)` tuple is intended for both the `connect` and the `read` timeouts, respectively.
+            If set to `None`, it will take a default value of `(3.05, 6)`.
+            
+          * `request_retries` specifies the maximum number of retry attempts allowed on exceptions and interested status codes
+            (i.e. `status_forcelist`) for the builtin Retry logic of `urllib3`. It will default to `download.URLLIB3_BUILTIN_RETRIES_ON_EXCEPTION`
+            if not given.
+            
+            NB: There are two retry mechanisms that jointly determine the total retries of a request. One is the above-mentioned
+            Retry logic that is built into `urllib3`, and the other is the extended high-level retry factor that is meant to 
+            complement the builtin retry mechanism. The total retries is bounded by the following formula:
+            `request_retries` * (_requests_extended_retries_factor_ + 1), where _requests_extended_retries_factor_ can be modified
+            through the module level function `bdownload.set_requests_retries_factor()`, and is initialized to 
+            `download.REQUESTS_EXTENDED_RETRIES_FACTOR` by default; Usually you don't want to change it.
+            
+          * `status_forcelist` specifies a set of HTTP status codes that a retry should be enforced on. The default set of status
+            codes shall be `download.URLLIB3_RETRY_STATUS_CODES` if not given.
+            
+          * The `resumption_retries` parameter specifies the maximum allowable number of retries on error at resuming the interrupted
+            download while streaming the request content. The default value of it is `download.REQUESTS_RETRIES_ON_STREAM_EXCEPTION` 
+            when not provided.
+            
+          * The `continuation` parameter specifies whether, if possible, to resume the partially downloaded files before, e.g. 
+            when the downloads had been terminated by the user by pressing `Ctrl-C`. When not present, it will default to `True`.
+          
+          * `referrer` specifies an HTTP request header `Referer` that applies to all downloads. If set to `'*'`, the request URL
+            shall be used as the referrer per download.
+        
+          * The `check_certificate` parameter specifies whether to verify the server's TLS certificate or not. It defaults to `True`.
+        
+          * `ca_certificate` specifies a path to the preferred CA bundle file (.pem) or directory with certificates in PEM format
+            of trusted CAs. If set to a path to a directory, the directory must have been processed using the `c_rehash` utility
+            supplied with OpenSSL, according to `requests`. NB the cert files in the directory each only contain one CA certificate.
+        
+          * `certificate` specifies a client certificate. It has the same meaning as that of `cert` in `requests.request()`.
+        
+          * The `auth` parameter sets a (user, pass) tuple or Auth handler to enable Basic/Digest/Custom HTTP Authentication. 
+            It will be passed down to the underlying :class:`requests.Session` instance as the default authentication.
+            
+            > **:warning:**\
+              The `auth` will be applied to all the downloads for HTTP Authentication. Don't use this parameter, if not all of the
+              downloads need the authentication, to avoid leaking credential. Instead, use the `netrc` parameter for fine-grained
+              control over HTTP Authentication.
+        
+          * `netrc` specifies a dictionary of ``'machine': (login, password)`` (or ``'machine': requests.auth.AuthBase``)
+            for HTTP Authentication, similar to the .netrc file format in spirit.
+        
+          * `headers` specifies extra HTTP headers, standard or custom, for use in all of the requests made by the session. 
+            The headers take precedence over the ones specified by other parameters, e.g. `user_agent`, if conflict happens.
+        
+        `
+        BDownloader.downloads(path_urls)
+        `
+        
+            Submit multiple downloading jobs at a time.
+          
+          * `path_urls` accepts a list of tuples of the form (_path_, _url_), where _path_ should be a pathname, probably prefixed
+            with absolute or relative paths, and _url_ should be a URL string, which may consist of multiple TAB-separated URLs 
+            pointing to the same file. A valid `path_urls`, for example, could be [('_/opt/files/bar.tar.bz2_', '_https://foo.cc/bar.tar.bz2_'),
+            ('_./sanguoshuowen.pdf_', '_https://bar.cc/sanguoshuowen.pdf\thttps://foo.cc/sanguoshuowen.pdf_'), 
+            ('_/**to**/**be**/created/_', '_https://flash.jiefang.rmy/lc-cl/gaozhuang/chelsia/rockspeaker.tar.gz_'), ('_/path/to/**existing**-dir_',
+            '_https://ghosthat.bar/foo/puretonecone81.xz\thttps://tpot.horn/foo/puretonecone81.xz\thttps://hawkhill.bar/foo/puretonecone81.xz_')].
+            
+            Note that `BDownloaderException` will be raised if the downloads were interrupted, e.g. by calling
+            `BDownloader.cancel()` in a `SIGINT` signal handler, in the process of submitting the download requests.
+        
+            > **:warning:**\
+              The method is not thread-safe, which means it should not be called at the same time in multiple threads
+              with one instance.
+            > 
+            > When multi-instanced (e.g. one instance per thread), the file paths specified in one instance should not overlap 
+              those in another to avoid potential race conditions. File loss may occur, for example, if a failed download task 
+              in one instance tries to delete a directory that is being accessed by some download tasks in other instances.
+              However, this limitation doesn't apply to the file paths specified in a same instance.
+        
+        `
+        BDownloader.download(path, url)
+        `
+        
+            Submit a single downloading job.
+          
+          * Similar to `BDownloader.downloads()`, in fact it is just a special case of which, with [(`path`, `url`)] composed of
+            the specified parameters as the input.
+            
+            Note that `BDownloaderException` will be raised if the download was interrupted, e.g. by calling
+            `BDownloader.cancel()` in a `SIGINT` signal handler, in the process of submitting the download request.
+            
+            > **:warning:**\
+              The limitation on the method and the `path_name` parameter herein is the same as in `BDownloader.downloads()`.
+        
+        `
+        BDownloader.wait_for_all()
+        `
+        
+            Wait for all the downloading jobs to complete. Returns a 2-tuple of lists (_succeeded_, _failed_).
+            The first list _succeeded_ contains the originally passed (_path_, _url_)s that completed successfully, while
+            the second list _failed_ contains the raised and cancelled ones.
+        
+        `
+        BDownloader.results()
+        `
+        
+            Get both the succeeded and failed downloads when all done or interrupted by user. Return a 2-tuple of list
+            same as that returned by `BDownloader.wait_for_all()`.
+        
+        `
+        BDownloader.result()
+        `
+        
+            Return the final download status. 0 for success, and -1 failure.
+        
+        `
+        BDownloader.close()
+        `
+        
+            Shut down and perform the cleanup.
+        
+        `
+        BDownloader.cancel(keyboard_interrupt=True)
+        `
+        
+            Cancel all the download jobs.
+        
+          * `keyboard_interrupt` specifies whether the user hit the interrupt key (e.g. Ctrl-C).
+        
+        `
+        bdownload.set_requests_retries_factor(retries)
+        `
+        
+            Set the retries factor that complements and extends the builtin retry mechanism of `urllib3`.
+        
+          * The `retries` parameter specifies the maximum number of retries when a decorated method of `requests` raised an 
+            exception or returned any bad status code. It should take a value of at least `1`, or else nothing changes.
+        
+        #### Examples
+        
+        * [`movie-downloader`'s third-party programs downloader](https://github.com/Jesseatgao/movie-downloader/blob/32b775c89f273d0b34af6c713e9a9362039b805c/mdl/third_parties/__init__.py#L175)
+        
+        * [`bdownload`'s command-line utility](https://github.com/Jesseatgao/bdownload/blob/master/src/bdownload/cli.py)
+        
+        * [`bdownload`'s CACERT-updating utility](https://github.com/Jesseatgao/bdownload/blob/master/src/bdownload/utils.py)
+        
+        * Single file downloading
+        
+        ```python
+        
+        import unittest
+        import tempfile
+        import os
+        import hashlib
+        
+        from bdownload import BDownloader
+        
+        
+        class TestBDownloader(unittest.TestCase):
+            def setUp(self):
+                self.tmp_dir = tempfile.TemporaryDirectory()
+        
+            def tearDown(self):
+                self.tmp_dir.cleanup()
+        
+            def test_bdownloader_download(self):
+                file_path = os.path.join(self.tmp_dir.name, "aria2-x86_64-win.zip")
+                file_url = "https://github.com/Jesseatgao/aria2-patched-static-build/releases/download/1.35.0-win-linux/aria2-x86_64-win.zip"
+                file_sha1_exp = "16835c5329450de7a172412b09464d36c549b493"
+        
+                with BDownloader(max_workers=20, progress='mill') as downloader:
+                    downloader.download(file_path, file_url)
+                    downloader.wait_for_all()
+        
+                hashf = hashlib.sha1()
+                with open(file_path, mode='rb') as f:
+                    hashf.update(f.read())
+                file_sha1 = hashf.hexdigest()
+        
+                self.assertEqual(file_sha1_exp, file_sha1)
+        
+        
+        if __name__ == '__main__':
+            unittest.main()
+        
+        ```
+        
+        * Batch file downloading
+        
+        ```python
+        
+        import unittest
+        import tempfile
+        import os
+        import hashlib
+        
+        from bdownload import BDownloader
+        
+        
+        class TestBDownloader(unittest.TestCase):
+            def setUp(self):
+                self.tmp_dir = tempfile.TemporaryDirectory()
+        
+            def tearDown(self):
+                self.tmp_dir.cleanup()
+        
+            def test_bdownloader_downloads(self):
+                files = [
+                    {
+                        "file": os.path.join(self.tmp_dir.name, "aria2-x86_64-linux.tar.xz"),
+                        "url": "https://github.com/Jesseatgao/aria2-patched-static-build/releases/download/1.35.0-win-linux/aria2-x86_64-linux.tar.xz",
+                        "sha1": "d02dfdab7517e78a257f4403e502f1acc2a795e4"
+                    },
+                    {
+                        "file": os.path.join(self.tmp_dir.name, "mkvtoolnix-x86_64-linux.tar.xz"),
+                        "url": "https://github.com/Jesseatgao/MKVToolNix-static-builds/releases/download/v47.0.0-mingw-w64-win32v1.0/mkvtoolnix-x86_64-linux.tar.xz",
+                        "sha1": "19b0c7fc20839693cc0929f092f74820783a9750"
+                    }
+                ]
+        
+                file_urls = [(f["file"], f["url"]) for f in files]
+        
+                with BDownloader(max_workers=20, progress='mill') as downloader:
+                    downloader.downloads(file_urls)
+                    downloader.wait_for_all()
+        
+                for f in files:
+                    hashf = hashlib.sha1()
+                    with open(f["file"], mode='rb') as fd:
+                        hashf.update(fd.read())
+                    file_sha1 = hashf.hexdigest()
+        
+                    self.assertEqual(f["sha1"], file_sha1)
+        
+        
+        if __name__ == '__main__':
+            unittest.main()
+        
+        ```
+        ### Usage: as a command-line script
+        
+        #### Synopsis
+        
+        ```
+        bdownload      url | -L URLS [URLS ...]
+                       [-O OUTPUT | -o OUTPUT [OUTPUT ...]] [-D DIR]
+                       [-p PROXY] [-n MAX_WORKERS] [-j MAX_PARALLEL_DOWNLOADS]
+                       [-J WORKERS_PER_DOWNLOAD] [-k MIN_SPLIT_SIZE] [-s CHUNK_SIZE]
+                       [-e COOKIE] [--user-agent USER_AGENT] [--referrer REFERRER]
+                       [--check-certificate {True,true,TRUE,False,false,FALSE}]
+                       [--ca-certificate CA_CERTIFICATE]
+                       [--certificate CERTIFICATE] [--private-key PRIVATE_KEY]
+                       [-P {mill,bar,none}] [--num-pools NUM_POOLS]
+                       [--pool-size POOL_SIZE] [-l {debug,info,warning,error,critical}]
+                       [-c | --no-continue] [-H HEADER] [-u USER_PASS] [--netrc-file NETRC_FILE]
+                       [-h]
+        ```
+        
+        #### Description
+        
+        `url`
+        
+            URL for the file to be downloaded, which can be either a single URL or TAB-separated composite URL 
+            pointing to the same file, e.g. `"https://www.afilelink.com/afile.tar.gz"`, 
+            `"https://chinshou.libccp.mil/luoxuan1981/panjuan-hangyi/tiqianbaozha-key-yasui/qianjunyifa/bengqiyijiao/i-manual/dashboy-basket/zhongzhenkong/xinghuo-xianghui/chunqiao-electronhive-midianfeng/zhenhudan-yasally/afile.tar.gz"`,
+            and `"https://www.afilelink.com/afile.tar.gz\thttps://nianpei.bpfatran.com/afile.tar.gz"`
+        
+        `-L URLS [URLS ...], --url URLS [URLS ...]`
+        
+            URL(s) for the files to be downloaded, each of which might contain TAB-separated URLs 
+            pointing to the same file, e.g. `-L https://yoursite.net/yourfile.7z`, 
+            `-L "https://yoursite01.net/thefile.7z\thttps://yoursite02.com/thefile.7z"`, 
+            or `--url "http://foo.cc/file1.zip" "http://bar.cc/file2.tgz\thttp://bar2.cc/file2.tgz"`
+        
+        `-O OUTPUT, --OUTPUT OUTPUT`
+        
+            a save-as file name (optionally with absolute or relative (to `-D DIR`) path), 
+            e.g. `-O afile.tar.gz https://www.afilelink.com/afile.tar.gz`
+        
+        `-o OUTPUT [OUTPUT ...], --output OUTPUT [OUTPUT ...]`
+        
+            one or more file names (optionally prefixed with relative (to `-D DIR`) or absolute paths), e.g. 
+            `-o file1.zip ~/file2.tgz`, paired with URLs specified by `--url` or `-L`
+        
+        `-D DIR, --dir DIR`
+        
+            directory in which to save the downloaded files [default: directory in which this App is running]
+        
+        `-p PROXY, --proxy PROXY`
+        
+            proxy either in the form of "`http://[user:pass@]host:port`" or "`socks5://[user:pass@]host:port`"
+        
+        `-n MAX_WORKERS, --max-workers MAX_WORKERS`
+        
+            number of worker threads [default: 20]
+        
+        `-j MAX_PARALLEL_DOWNLOADS, --max-parallel-downloads MAX_PARALLEL_DOWNLOADS`
+        
+            number of files downloading concurrently [default: 5]
+        
+        `-J WORKERS_PER_DOWNLOAD, --workers-per-download WORKERS_PER_DOWNLOAD`
+        
+            number of worker threads for every file downloading job [default: 4]
+        
+        `-k MIN_SPLIT_SIZE, --min-split-size MIN_SPLIT_SIZE`
+        
+            file split size in bytes, "1048576, 1024K or 2M" for example [default: 1M]
+        
+        `-s CHUNK_SIZE, --chunk-size CHUNK_SIZE`
+        
+            every request range size in bytes, "10240, 10K or 1M" for example [default: 100K]
+        
+        `-e COOKIE, --cookie COOKIE`
+        
+            cookies either in the form of a string (maybe whitespace- and/or semicolon- separated) 
+            like "`cookie_key=cookie_value cookie_key2=cookie_value2; cookie_key3=cookie_value3`", or a file, 
+            e.g. named "cookies.txt", in the Netscape cookie file format. NB the option `-D DIR` does not apply to the cookie file
+        
+        `--user-agent USER_AGENT`
+        
+            custom user agent
+        
+        `--referrer REFERRER`
+        
+            HTTP request header "Referer" that applies to all downloads. In particular, use `*` to tell the downloader
+            to take the request URL as the referrer per download [default: *]
+        
+        `--check-certificate {True,true,TRUE,False,false,FALSE}`
+        
+            whether to verify the server's TLS certificate or not [default: True]
+        
+        `--ca-certificate CA_CERTIFICATE`
+        
+            path to the preferred CA bundle file (.pem) or directory with certificates in PEM format of trusted CAs.
+            NB the directory must have been processed using the `c_rehash` utility from OpenSSL. Also, the cert files in the directory
+            each only contain one CA certificate
+        
+        `--certificate CERTIFICATE`
+        
+            path to a single file in PEM format containing the client certificate and optionally a chain of additional
+            certificates. If `--private-key` is not provided, then the file must contain the unencrypted private key as well
+        
+        `--private-key PRIVATE_KEY`
+        
+            path to a file containing the unencrypted private key to the client certificate
+        
+        `-P {mill,bar,none}, --progress {mill,bar,none}`
+        
+            progress indicator. To disable this feature, use `none`. [default: mill]
+        
+        `--num-pools NUM_POOLS`
+        
+            number of connection pools [default: 20]
+        
+        `--pool-size POOL_SIZE`
+        
+            max number of connections in the pool [default: 20]
+        
+        `-l {debug,info,warning,error,critical}, --log-level {debug,info,warning,error,critical}`
+        
+            logger level [default: warning]
+        
+        `-c, --continue`
+        
+            resume from the partially downloaded files. This is the default behavior
+        
+        `--no-continue`
+        
+            do not resume from last interruption, i.e. start the download from beginning
+        
+        `-H HEADER, --header HEADER`
+        
+            extra HTTP header, standard or custom, which can be repeated several times, e.g. 
+            '`-H "User-Agent: John Doe" -H "X-BD-Key: One Thousand And One Nights"`'. The headers take precedence over the ones 
+            specified by other parameters if conflict happens
+        
+        `-u USER_PASS, --user-pass USER_PASS`
+        
+            default HTTP Authentication for ALL the downloads in "`user:password`" format. Warning: don't use this option
+            if not all of the downloads need the authentication to avoid leaking credential, use the `--netrc-file` option instead
+        
+        `--netrc-file NETRC_FILE`
+        
+            a .netrc-like file for HTTP authentication, from which the 'default' entry, if present, takes precedence
+            over the `--user-pass` option
+        
+        `-h, --help`
+        
+            show help message and exit
+        
+        #### Examples
+        
+            bdownload https://www.afilelink.com/afile.tar.gz
+            bdownload -O /abspath/to/afile.tar.gz https://www.afilelink.com/afile.tar.gz
+            bdownload -O /abspath/to/a/dir/ https://www.afilelink.com/afile.tar.gz
+            bdownload -O /abspath/to/afile.tar.gz "https://www.afilelink.com/afile.tar.gz\thttps://nianpei.bpfatran.com/afile.tar.gz"
+            bdownload -D path/to/working_dir/ -O relpath/to/working_dir/alias_afile.tar.gz https://www.afilelink.com/afile.tar.gz
+            bdownload -D path/to/working/dir https://www.afilelink.com/afile.tar.gz
+            bdownload -o /abspath/to/file1.zip ~/file2.tgz -L "http://foo.cc/file1.zip" "http://bar.cc/file2.tgz\thttp://bar2.cc/file2.tgz"
+            bdownload -D path/to/working/dir -L "http://foo.cc/file1.zip" "http://bar.cc/file2.tgz\thttp://bar2.cc/file2.tgz"
+        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
@@ -21,453 +508,7 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Description-Content-Type: text/markdown
-
-## bdownload
-[![Latest Version](https://img.shields.io/pypi/v/bdownload.svg)](https://pypi.org/project/bdownload/)
-[![Build Status](https://travis-ci.com/Jesseatgao/bdownload.svg?branch=master)](https://travis-ci.com/Jesseatgao/bdownload)
-[![Supported Versions](https://img.shields.io/pypi/pyversions/bdownload.svg)](https://pypi.org/project/bdownload)
-
-A multi-threaded and multi-source aria2-like batch file downloading library for Python 2.7 and 3.6+
-
-> **:bulb:**\
-> See also [https://bdownload.readthedocs.io](https://bdownload.readthedocs.io) for API reference.
-
-### Installation
-
-* via PyPI
-
-    `pip install bdownload`
-
-* from within source directory locally
-
-    `pip install .`
-    
-    Note that you should `git clone` or download the source tarball (and unpack it of course) from the repository first 
-
-> **:bulb:**\
-> For Python2.7: since the version of 2022.5.18, `certifi` has dropped the support for Python2.x. To upgrade to the latest CA
-> certificates bundle, simply run:
-> 
-> `$ bdownload-upd-cacert-py2`
-
-### Usage: as a Python package
-
-#### Importing
-
-    `from bdownload import BDownloader, BDownloaderException`
-
-            or
-
-    `import bdownload`
-
-#### Signatures
-
-`
-class bdownload.BDownloader(max_workers=None, min_split_size=1024*1024, chunk_size=1024*100, proxy=None, cookies=None,
-                            user_agent=None, logger=None, progress='mill', num_pools=20, pool_maxsize=20, request_timeout=None,
-                            request_retries=None, status_forcelist=None, resumption_retries=None, continuation=True, referrer=None,
-                            check_certificate=True, ca_certificate=None, certificate=None)
-`
-
-    Create and initialize a `BDownloader` object for executing download jobs.
-  
-  * The `max_workers` parameter specifies the number of the parallel downloading threads, whose default value is 
-    determined by _#num_of_processor * 5_ if set to `None`.
-  
-  * `min_split_size` denotes the size in bytes of file pieces split to be downloaded in parallel, which defaults to 
-    1024*1024 bytes (i.e. 1MB).
-  
-  * The `chunk_size` parameter specifies the chunk size in bytes of every http range request, which will take a default 
-    value of 1024*100 (i.e. 100KB) if not provided.
-  
-  * `proxy` supports both HTTP and SOCKS proxies in the form of _http://[user:pass@]host:port_ and 
-    _socks5://[user:pass@]host:port_, respectively.
-  
-  * If `cookies` needs to be set, it must either take the form of _cookie_key=cookie_value_, with multiple pairs separated
-    by whitespace and/or semicolon if applicable, e.g. '_key1=val1 key2=val2;key3=val3_', be packed into a `dict`, or 
-    be an instance of `CookieJar`, i.e. `cookielib.CookieJar` for Python27, `http.cookiejar.CookieJar` for Python3.x or 
-    `RequestsCookieJar` from `requests`.
-    
-    Note that the `ValueError` exception will be raised when the `cookies` is of the `str` type and not in the valid format.
-  
-  * When `user_agent` is not given, it will default to '_bdownload/VERSION_', with _VERSION_ being replaced by the 
-    package's version number.
-  
-  * The `logger` parameter specifies an event logger. If `logger` is not `None`, it must be an object of class 
-    `logging.Logger` or of its customized subclass.  Otherwise, it will use a default module-level logger returned by 
-    `logging.getLogger(__name__)`.
-  
-  * `progress` determines the style of the progress bar displayed while downloading files. Possible values are `'mill'`,
-    `'bar'` and `'none''`. `'mill'` is the default. To disable this feature, e.g. while scripting or multi-instanced, 
-    set it to `'none'`.
-  
-  * The `num_pools` parameter has the same meaning as `num_pools` in `urllib3.PoolManager` and will eventually be passed
-    to it. Specifically, `num_pools` specifies the number of connection pools to cache.
-  
-  * `pool_maxsize` will be passed to the underlying `requests.adapters.HTTPAdapter`. It specifies the maximum number of 
-    connections to save that can be reused in the urllib3 connection pool.
-
-  * The `request_timeout` parameter specifies the timeouts for the internal `requests` session. The timeout value(s) 
-    as a float or `(connect, read)` tuple is intended for both the `connect` and the `read` timeouts, respectively.
-    If set to `None`, it will take a default value of `(3.05, 6)`.
-    
-  * `request_retries` specifies the maximum number of retry attempts allowed on exceptions and interested status codes
-    (i.e. `status_forcelist`) for the builtin Retry logic of `urllib3`. It will default to `download.URLLIB3_BUILTIN_RETRIES_ON_EXCEPTION`
-    if not given.
-    
-    NB: There are two retry mechanisms that jointly determine the total retries of a request. One is the above-mentioned
-    Retry logic that is built into `urllib3`, and the other is the extended high-level retry factor that is meant to 
-    complement the builtin retry mechanism. The total retries is bounded by the following formula:
-    `request_retries` * (_requests_extended_retries_factor_ + 1), where _requests_extended_retries_factor_ can be modified
-    through the module level function `bdownload.set_requests_retries_factor()`, and is initialized to 
-    `download.REQUESTS_EXTENDED_RETRIES_FACTOR` by default; Usually you don't want to change it.
-    
-  * `status_forcelist` specifies a set of HTTP status codes that a retry should be enforced on. The default set of status
-    codes shall be `download.URLLIB3_RETRY_STATUS_CODES` if not given.
-    
-  * The `resumption_retries` parameter specifies the maximum allowable number of retries on error at resuming the interrupted
-    download while streaming the request content. The default value of it is `download.REQUESTS_RETRIES_ON_STREAM_EXCEPTION` 
-    when not provided.
-    
-  * The `continuation` parameter specifies whether, if possible, to resume the partially downloaded files before, e.g. 
-    when the downloads had been terminated by the user by pressing `Ctrl-C`. When not present, it will default to `True`.
-  
-  * `referrer` specifies an HTTP request header `Referer` that applies to all downloads. If set to `'*'`, the request URL
-    shall be used as the referrer per download.
-
-  * The `check_certificate` parameter specifies whether to verify the server's TLS certificate or not. It defaults to `True`.
-
-  * `ca_certificate` specifies a path to the preferred CA bundle file (.pem) or directory with certificates in PEM format
-    of trusted CAs. If set to a path to a directory, the directory must have been processed using the `c_rehash` utility
-    supplied with OpenSSL, according to `requests`. NB the cert files in the directory each only contain one CA certificate.
-
-  * `certificate` specifies a client certificate. It has the same meaning as that of `cert` in `requests.request()`.
-
-`
-BDownloader.downloads(path_urls)
-`
-
-    Submit multiple downloading jobs at a time.
-  
-  * `path_urls` accepts a list of tuples of the form (_path_, _url_), where _path_ should be a pathname, probably prefixed
-    with absolute or relative paths, and _url_ should be a URL string, which may consist of multiple TAB-separated URLs 
-    pointing to the same file. A valid `path_urls`, for example, could be [('_/opt/files/bar.tar.bz2_', '_https://foo.cc/bar.tar.bz2_'),
-    ('_./sanguoshuowen.pdf_', '_https://bar.cc/sanguoshuowen.pdf\thttps://foo.cc/sanguoshuowen.pdf_'), 
-    ('_/**to**/**be**/created/_', '_https://flash.jiefang.rmy/lc-cl/gaozhuang/chelsia/rockspeaker.tar.gz_'), ('_/path/to/**existing**-dir_',
-    '_https://ghosthat.bar/foo/puretonecone81.xz\thttps://tpot.horn/foo/puretonecone81.xz\thttps://hawkhill.bar/foo/puretonecone81.xz_')].
-    
-    Note that `BDownloaderException` will be raised if the downloads were interrupted, e.g. by calling
-    `BDownloader.cancel()` in a `SIGINT` signal handler, in the process of submitting the download requests.
-
-  > **:warning:**\
-  > The method is not thread-safe, which means it should not be called at the same time in multiple threads
-  > with one instance.
-  >
-  > When multi-instanced (e.g. one instance per thread), the file paths specified in one instance should not overlap 
-  > those in another to avoid potential race conditions. File loss may occur, for example, if a failed download task 
-  > in one instance tries to delete a directory that is being accessed by some download tasks in other instances.
-  > However, this limitation doesn't apply to the file paths specified in a same instance.
-
-`
-BDownloader.download(path, url)
-`
-
-    Submit a single downloading job.
-  
-  * Similar to `BDownloader.downloads()`, in fact it is just a special case of which, with [(`path`, `url`)] composed of
-    the specified parameters as the input.
-    
-    Note that `BDownloaderException` will be raised if the download was interrupted, e.g. by calling
-    `BDownloader.cancel()` in a `SIGINT` signal handler, in the process of submitting the download request.
-    
-  > **:warning:**\
-  > The limitation on the method and the `path_name` parameter herein is the same as in `BDownloader.downloads()`.
-
-`
-BDownloader.wait_for_all()
-`
-
-    Wait for all the downloading jobs to complete. Returns a 2-tuple of lists (_succeeded_, _failed_).
-    The first list _succeeded_ contains the originally passed (_path_, _url_)s that completed successfully, while
-    the second list _failed_ contains the raised and cancelled ones.
-
-`
-BDownloader.results()
-`
-
-    Get both the succeeded and failed downloads when all done or interrupted by user. Return a 2-tuple of list
-    same as that returned by `BDownloader.wait_for_all()`.
-
-`
-BDownloader.result()
-`
-
-    Return the final download status. 0 for success, and -1 failure.
-
-`
-BDownloader.close()
-`
-
-    Shut down and perform the cleanup.
-
-`
-BDownloader.cancel(keyboard_interrupt=True)
-`
-
-    Cancel all the download jobs.
-
-  * `keyboard_interrupt` specifies whether the user hit the interrupt key (e.g. Ctrl-C).
-
-`
-bdownload.set_requests_retries_factor(retries)
-`
-
-    Set the retries factor that complements and extends the builtin retry mechanism of `urllib3`.
-
-  * The `retries` parameter specifies the maximum number of retries when a decorated method of `requests` raised an 
-    exception or returned any bad status code. It should take a value of at least `1`, or else nothing changes.
-
-#### Examples
-
-* [`movie-downloader`'s third-party programs downloader](https://github.com/Jesseatgao/movie-downloader/blob/32b775c89f273d0b34af6c713e9a9362039b805c/mdl/third_parties/__init__.py#L175)
-
-* [`bdownload`'s command-line utility](https://github.com/Jesseatgao/bdownload/blob/master/src/bdownload/cli.py)
-
-* [`bdownload`'s CACERT-updating utility](https://github.com/Jesseatgao/bdownload/blob/master/src/bdownload/utils.py)
-
-* Single file downloading
-
-```python
-
-import unittest
-import tempfile
-import os
-import hashlib
-
-from bdownload import BDownloader
-
-
-class TestBDownloader(unittest.TestCase):
-    def setUp(self):
-        self.tmp_dir = tempfile.TemporaryDirectory()
-
-    def tearDown(self):
-        self.tmp_dir.cleanup()
-
-    def test_bdownloader_download(self):
-        file_path = os.path.join(self.tmp_dir.name, "aria2-x86_64-win.zip")
-        file_url = "https://github.com/Jesseatgao/aria2-patched-static-build/releases/download/1.35.0-win-linux/aria2-x86_64-win.zip"
-        file_sha1_exp = "16835c5329450de7a172412b09464d36c549b493"
-
-        with BDownloader(max_workers=20, progress='mill') as downloader:
-            downloader.download(file_path, file_url)
-            downloader.wait_for_all()
-
-        hashf = hashlib.sha1()
-        with open(file_path, mode='rb') as f:
-            hashf.update(f.read())
-        file_sha1 = hashf.hexdigest()
-
-        self.assertEqual(file_sha1_exp, file_sha1)
-
-
-if __name__ == '__main__':
-    unittest.main()
-
-```
-
-* Batch file downloading
-
-```python
-
-import unittest
-import tempfile
-import os
-import hashlib
-
-from bdownload import BDownloader
-
-
-class TestBDownloader(unittest.TestCase):
-    def setUp(self):
-        self.tmp_dir = tempfile.TemporaryDirectory()
-
-    def tearDown(self):
-        self.tmp_dir.cleanup()
-
-    def test_bdownloader_downloads(self):
-        files = [
-            {
-                "file": os.path.join(self.tmp_dir.name, "aria2-x86_64-linux.tar.xz"),
-                "url": "https://github.com/Jesseatgao/aria2-patched-static-build/releases/download/1.35.0-win-linux/aria2-x86_64-linux.tar.xz",
-                "sha1": "d02dfdab7517e78a257f4403e502f1acc2a795e4"
-            },
-            {
-                "file": os.path.join(self.tmp_dir.name, "mkvtoolnix-x86_64-linux.tar.xz"),
-                "url": "https://github.com/Jesseatgao/MKVToolNix-static-builds/releases/download/v47.0.0-mingw-w64-win32v1.0/mkvtoolnix-x86_64-linux.tar.xz",
-                "sha1": "19b0c7fc20839693cc0929f092f74820783a9750"
-            }
-        ]
-
-        file_urls = [(f["file"], f["url"]) for f in files]
-
-        with BDownloader(max_workers=20, progress='mill') as downloader:
-            downloader.downloads(file_urls)
-            downloader.wait_for_all()
-
-        for f in files:
-            hashf = hashlib.sha1()
-            with open(f["file"], mode='rb') as fd:
-                hashf.update(fd.read())
-            file_sha1 = hashf.hexdigest()
-
-            self.assertEqual(f["sha1"], file_sha1)
-
-
-if __name__ == '__main__':
-    unittest.main()
-
-```
-### Usage: as a command-line script
-
-#### Synopsis
-
-```
-bdownload      url | -L URLS [URLS ...]
-               [-O OUTPUT | -o OUTPUT [OUTPUT ...]] [-D DIR]
-               [-p PROXY] [-n MAX_WORKERS] [-k MIN_SPLIT_SIZE]
-               [-s CHUNK_SIZE] [-e COOKIE] [--user-agent USER_AGENT]
-               [--referrer REFERRER]
-               [--check-certificate {True,true,TRUE,False,false,FALSE}]
-               [--ca-certificate CA_CERTIFICATE]
-               [--certificate CERTIFICATE] [--private-key PRIVATE_KEY]
-               [-P {mill,bar,none}] [--num-pools NUM_POOLS]
-               [--pool-size POOL_SIZE] [-l {debug,info,warning,error,critical}]
-               [-c | --no-continue]
-               [-h]
-```
-
-#### Description
-
-`url`
-
-    URL for the file to be downloaded, which can be either a single URL or TAB-separated composite URL 
-    pointing to the same file, e.g. `"https://www.afilelink.com/afile.tar.gz"`, 
-    `"https://chinshou.libccp.mil/luoxuan1981/panjuan-hangyi/tiqianbaozha-key-yasui/qianjunyifa/bengqiyijiao/i-manual/dashboy-basket/zhongzhenkong/xinghuo-xianghui/chunqiao-electronhive-midianfeng/zhenhudan-yasally/afile.tar.gz"`,
-    and `"https://www.afilelink.com/afile.tar.gz\thttps://nianpei.bpfatran.com/afile.tar.gz"`
-
-`-L URLS [URLS ...], --url URLS [URLS ...]`
-
-    URL(s) for the files to be downloaded, each of which might contain TAB-separated URLs 
-    pointing to the same file, e.g. `-L https://yoursite.net/yourfile.7z`, 
-    `-L "https://yoursite01.net/thefile.7z\thttps://yoursite02.com/thefile.7z"`, 
-    or `--url "http://foo.cc/file1.zip" "http://bar.cc/file2.tgz\thttp://bar2.cc/file2.tgz"`
-
-`-O OUTPUT, --OUTPUT OUTPUT`
-
-    a save-as file name (optionally with absolute or relative (to `-D DIR`) path), 
-    e.g. `-O afile.tar.gz https://www.afilelink.com/afile.tar.gz`
-
-`-o OUTPUT [OUTPUT ...], --output OUTPUT [OUTPUT ...]`
-
-    one or more file names (optionally prefixed with relative (to `-D DIR`) or absolute paths), e.g. 
-    `-o file1.zip ~/file2.tgz`, paired with URLs specified by `--url` or `-L`
-
-`-D DIR, --dir DIR`
-
-    directory in which to save the downloaded files [default: directory in which this App is running]
-
-`-p PROXY, --proxy PROXY`
-
-    proxy either in the form of "http://[user:pass@]host:port" or "socks5://[user:pass@]host:port"
-
-`-n MAX_WORKERS, --max-workers MAX_WORKERS`
-
-    number of worker threads [default: 20]
-
-`-k MIN_SPLIT_SIZE, --min-split-size MIN_SPLIT_SIZE`
-
-    file split size in bytes, "1048576, 1024K or 2M" for example [default: 1M]
-
-`-s CHUNK_SIZE, --chunk-size CHUNK_SIZE`
-
-    every request range size in bytes, "10240, 10K or 1M" for example [default: 100K]
-
-`-e COOKIE, --cookie COOKIE`
-
-    cookies either in the form of a string (maybe whitespace- and/or semicolon- separated) 
-    like "cookie_key=cookie_value cookie_key2=cookie_value2; cookie_key3=cookie_value3", or a file, 
-    e.g. named "cookies.txt", in the Netscape cookie file format. NB the option `-D DIR` does not apply to the cookie file
-
-`--user-agent USER_AGENT`
-
-    custom user agent
-
-`--referrer REFERRER`
-
-    HTTP request header "Referer" that applies to all downloads. In particular, use `*` to tell the downloader
-    to take the request URL as the referrer per download [default: *]
-
-`--check-certificate {True,true,TRUE,False,false,FALSE}`
-
-    whether to verify the server's TLS certificate or not [default: True]
-
-`--ca-certificate CA_CERTIFICATE`
-
-    path to the preferred CA bundle file (.pem) or directory with certificates in PEM format of trusted CAs.
-    NB the directory must have been processed using the `c_rehash` utility from OpenSSL. Also, the cert files in the directory
-    each only contain one CA certificate
-
-`--certificate CERTIFICATE`
-
-    path to a single file in PEM format containing the client certificate and optionally a chain of additional
-    certificates. If `--private-key` is not provided, then the file must contain the unencrypted private key as well
-
-`--private-key PRIVATE_KEY`
-
-    path to a file containing the unencrypted private key to the client certificate
-
-`-P {mill,bar,none}, --progress {mill,bar,none}`
-
-    progress indicator. To disable this feature, use `none`. [default: mill]
-
-`--num-pools NUM_POOLS`
-
-    number of connection pools [default: 20]
-
-`--pool-size POOL_SIZE`
-
-    max number of connections in the pool [default: 20]
-
-`-l {debug,info,warning,error,critical}, --log-level {debug,info,warning,error,critical}`
-
-    logger level [default: warning]
-
-`-c, --continue`
-
-    resume from the partially downloaded files. This is the default behavior
-
-`--no-continue`
-
-    do not resume from last interruption, i.e. start the download from beginning
-
-`-h, --help`
-
-    show help message and exit
-
-#### Examples
-
-    bdownload https://www.afilelink.com/afile.tar.gz
-    bdownload -O /abspath/to/afile.tar.gz https://www.afilelink.com/afile.tar.gz
-    bdownload -O /abspath/to/a/dir/ https://www.afilelink.com/afile.tar.gz
-    bdownload -O /abspath/to/afile.tar.gz "https://www.afilelink.com/afile.tar.gz\thttps://nianpei.bpfatran.com/afile.tar.gz"
-    bdownload -D path/to/working_dir/ -O relpath/to/working_dir/alias_afile.tar.gz https://www.afilelink.com/afile.tar.gz
-    bdownload -D path/to/working/dir https://www.afilelink.com/afile.tar.gz
-    bdownload -o /abspath/to/file1.zip ~/file2.tgz -L "http://foo.cc/file1.zip" "http://bar.cc/file2.tgz\thttp://bar2.cc/file2.tgz"
-    bdownload -D path/to/working/dir -L "http://foo.cc/file1.zip" "http://bar.cc/file2.tgz\thttp://bar2.cc/file2.tgz"
-
-
```

### Comparing `bdownload-0.1.8/README.md` & `bdownload-0.1.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -35,24 +35,29 @@
             or
 
     `import bdownload`
 
 #### Signatures
 
 `
-class bdownload.BDownloader(max_workers=None, min_split_size=1024*1024, chunk_size=1024*100, proxy=None, cookies=None,
-                            user_agent=None, logger=None, progress='mill', num_pools=20, pool_maxsize=20, request_timeout=None,
-                            request_retries=None, status_forcelist=None, resumption_retries=None, continuation=True, referrer=None,
-                            check_certificate=True, ca_certificate=None, certificate=None)
+class bdownload.BDownloader(max_workers=None, max_parallel_downloads=5, workers_per_download=4, min_split_size=1024*1024,
+                            chunk_size=1024*100, proxy=None, cookies=None, user_agent=None, logger=None, progress='mill',
+                            num_pools=20, pool_maxsize=20, request_timeout=None, request_retries=None, status_forcelist=None,
+                            resumption_retries=None, continuation=True, referrer=None, check_certificate=True, ca_certificate=None,
+                            certificate=None, auth=None, netrc=None, headers=None)
 `
 
     Create and initialize a `BDownloader` object for executing download jobs.
   
   * The `max_workers` parameter specifies the number of the parallel downloading threads, whose default value is 
     determined by _#num_of_processor * 5_ if set to `None`.
+
+  * `max_parallel_downloads` limits the number of files downloading concurrently. It has a default value of 5.
+
+  * `workers_per_download` sets the maximum number of worker threads for every file downloading job, which defaults to 4.
   
   * `min_split_size` denotes the size in bytes of file pieces split to be downloaded in parallel, which defaults to 
     1024*1024 bytes (i.e. 1MB).
   
   * The `chunk_size` parameter specifies the chunk size in bytes of every http range request, which will take a default 
     value of 1024*100 (i.e. 100KB) if not provided.
   
@@ -70,15 +75,15 @@
     package's version number.
   
   * The `logger` parameter specifies an event logger. If `logger` is not `None`, it must be an object of class 
     `logging.Logger` or of its customized subclass.  Otherwise, it will use a default module-level logger returned by 
     `logging.getLogger(__name__)`.
   
   * `progress` determines the style of the progress bar displayed while downloading files. Possible values are `'mill'`,
-    `'bar'` and `'none''`. `'mill'` is the default. To disable this feature, e.g. while scripting or multi-instanced, 
+    `'bar'` and `'none'`. `'mill'` is the default. To disable this feature, e.g. while scripting or multi-instanced, 
     set it to `'none'`.
   
   * The `num_pools` parameter has the same meaning as `num_pools` in `urllib3.PoolManager` and will eventually be passed
     to it. Specifically, `num_pools` specifies the number of connection pools to cache.
   
   * `pool_maxsize` will be passed to the underlying `requests.adapters.HTTPAdapter`. It specifies the maximum number of 
     connections to save that can be reused in the urllib3 connection pool.
@@ -115,53 +120,67 @@
 
   * `ca_certificate` specifies a path to the preferred CA bundle file (.pem) or directory with certificates in PEM format
     of trusted CAs. If set to a path to a directory, the directory must have been processed using the `c_rehash` utility
     supplied with OpenSSL, according to `requests`. NB the cert files in the directory each only contain one CA certificate.
 
   * `certificate` specifies a client certificate. It has the same meaning as that of `cert` in `requests.request()`.
 
+  * The `auth` parameter sets a (user, pass) tuple or Auth handler to enable Basic/Digest/Custom HTTP Authentication. 
+    It will be passed down to the underlying :class:`requests.Session` instance as the default authentication.
+    
+    > **:warning:**\
+      The `auth` will be applied to all the downloads for HTTP Authentication. Don't use this parameter, if not all of the
+      downloads need the authentication, to avoid leaking credential. Instead, use the `netrc` parameter for fine-grained
+      control over HTTP Authentication.
+
+  * `netrc` specifies a dictionary of ``'machine': (login, password)`` (or ``'machine': requests.auth.AuthBase``)
+    for HTTP Authentication, similar to the .netrc file format in spirit.
+
+  * `headers` specifies extra HTTP headers, standard or custom, for use in all of the requests made by the session. 
+    The headers take precedence over the ones specified by other parameters, e.g. `user_agent`, if conflict happens.
+
 `
 BDownloader.downloads(path_urls)
 `
 
     Submit multiple downloading jobs at a time.
   
   * `path_urls` accepts a list of tuples of the form (_path_, _url_), where _path_ should be a pathname, probably prefixed
     with absolute or relative paths, and _url_ should be a URL string, which may consist of multiple TAB-separated URLs 
     pointing to the same file. A valid `path_urls`, for example, could be [('_/opt/files/bar.tar.bz2_', '_https://foo.cc/bar.tar.bz2_'),
     ('_./sanguoshuowen.pdf_', '_https://bar.cc/sanguoshuowen.pdf\thttps://foo.cc/sanguoshuowen.pdf_'), 
     ('_/**to**/**be**/created/_', '_https://flash.jiefang.rmy/lc-cl/gaozhuang/chelsia/rockspeaker.tar.gz_'), ('_/path/to/**existing**-dir_',
     '_https://ghosthat.bar/foo/puretonecone81.xz\thttps://tpot.horn/foo/puretonecone81.xz\thttps://hawkhill.bar/foo/puretonecone81.xz_')].
     
-    Note that `BDownloaderException` will be raised if the downloads were interrupted, e.g. by calling
+    Note that `BDownloaderException` will be raised if the downloads were interrupted, e.g. by calling
     `BDownloader.cancel()` in a `SIGINT` signal handler, in the process of submitting the download requests.
 
-  > **:warning:**\
-  > The method is not thread-safe, which means it should not be called at the same time in multiple threads
-  > with one instance.
-  >
-  > When multi-instanced (e.g. one instance per thread), the file paths specified in one instance should not overlap 
-  > those in another to avoid potential race conditions. File loss may occur, for example, if a failed download task 
-  > in one instance tries to delete a directory that is being accessed by some download tasks in other instances.
-  > However, this limitation doesn't apply to the file paths specified in a same instance.
+    > **:warning:**\
+      The method is not thread-safe, which means it should not be called at the same time in multiple threads
+      with one instance.
+    > 
+    > When multi-instanced (e.g. one instance per thread), the file paths specified in one instance should not overlap 
+      those in another to avoid potential race conditions. File loss may occur, for example, if a failed download task 
+      in one instance tries to delete a directory that is being accessed by some download tasks in other instances.
+      However, this limitation doesn't apply to the file paths specified in a same instance.
 
 `
 BDownloader.download(path, url)
 `
 
     Submit a single downloading job.
   
   * Similar to `BDownloader.downloads()`, in fact it is just a special case of which, with [(`path`, `url`)] composed of
     the specified parameters as the input.
     
-    Note that `BDownloaderException` will be raised if the download was interrupted, e.g. by calling
+    Note that `BDownloaderException` will be raised if the download was interrupted, e.g. by calling
     `BDownloader.cancel()` in a `SIGINT` signal handler, in the process of submitting the download request.
     
-  > **:warning:**\
-  > The limitation on the method and the `path_name` parameter herein is the same as in `BDownloader.downloads()`.
+    > **:warning:**\
+      The limitation on the method and the `path_name` parameter herein is the same as in `BDownloader.downloads()`.
 
 `
 BDownloader.wait_for_all()
 `
 
     Wait for all the downloading jobs to complete. Returns a 2-tuple of lists (_succeeded_, _failed_).
     The first list _succeeded_ contains the originally passed (_path_, _url_)s that completed successfully, while
@@ -307,23 +326,23 @@
 ### Usage: as a command-line script
 
 #### Synopsis
 
 ```
 bdownload      url | -L URLS [URLS ...]
                [-O OUTPUT | -o OUTPUT [OUTPUT ...]] [-D DIR]
-               [-p PROXY] [-n MAX_WORKERS] [-k MIN_SPLIT_SIZE]
-               [-s CHUNK_SIZE] [-e COOKIE] [--user-agent USER_AGENT]
-               [--referrer REFERRER]
+               [-p PROXY] [-n MAX_WORKERS] [-j MAX_PARALLEL_DOWNLOADS]
+               [-J WORKERS_PER_DOWNLOAD] [-k MIN_SPLIT_SIZE] [-s CHUNK_SIZE]
+               [-e COOKIE] [--user-agent USER_AGENT] [--referrer REFERRER]
                [--check-certificate {True,true,TRUE,False,false,FALSE}]
                [--ca-certificate CA_CERTIFICATE]
                [--certificate CERTIFICATE] [--private-key PRIVATE_KEY]
                [-P {mill,bar,none}] [--num-pools NUM_POOLS]
                [--pool-size POOL_SIZE] [-l {debug,info,warning,error,critical}]
-               [-c | --no-continue]
+               [-c | --no-continue] [-H HEADER] [-u USER_PASS] [--netrc-file NETRC_FILE]
                [-h]
 ```
 
 #### Description
 
 `url`
 
@@ -351,32 +370,40 @@
 
 `-D DIR, --dir DIR`
 
     directory in which to save the downloaded files [default: directory in which this App is running]
 
 `-p PROXY, --proxy PROXY`
 
-    proxy either in the form of "http://[user:pass@]host:port" or "socks5://[user:pass@]host:port"
+    proxy either in the form of "`http://[user:pass@]host:port`" or "`socks5://[user:pass@]host:port`"
 
 `-n MAX_WORKERS, --max-workers MAX_WORKERS`
 
     number of worker threads [default: 20]
 
+`-j MAX_PARALLEL_DOWNLOADS, --max-parallel-downloads MAX_PARALLEL_DOWNLOADS`
+
+    number of files downloading concurrently [default: 5]
+
+`-J WORKERS_PER_DOWNLOAD, --workers-per-download WORKERS_PER_DOWNLOAD`
+
+    number of worker threads for every file downloading job [default: 4]
+
 `-k MIN_SPLIT_SIZE, --min-split-size MIN_SPLIT_SIZE`
 
     file split size in bytes, "1048576, 1024K or 2M" for example [default: 1M]
 
 `-s CHUNK_SIZE, --chunk-size CHUNK_SIZE`
 
     every request range size in bytes, "10240, 10K or 1M" for example [default: 100K]
 
 `-e COOKIE, --cookie COOKIE`
 
     cookies either in the form of a string (maybe whitespace- and/or semicolon- separated) 
-    like "cookie_key=cookie_value cookie_key2=cookie_value2; cookie_key3=cookie_value3", or a file, 
+    like "`cookie_key=cookie_value cookie_key2=cookie_value2; cookie_key3=cookie_value3`", or a file, 
     e.g. named "cookies.txt", in the Netscape cookie file format. NB the option `-D DIR` does not apply to the cookie file
 
 `--user-agent USER_AGENT`
 
     custom user agent
 
 `--referrer REFERRER`
@@ -423,14 +450,30 @@
 
     resume from the partially downloaded files. This is the default behavior
 
 `--no-continue`
 
     do not resume from last interruption, i.e. start the download from beginning
 
+`-H HEADER, --header HEADER`
+
+    extra HTTP header, standard or custom, which can be repeated several times, e.g. 
+    '`-H "User-Agent: John Doe" -H "X-BD-Key: One Thousand And One Nights"`'. The headers take precedence over the ones 
+    specified by other parameters if conflict happens
+
+`-u USER_PASS, --user-pass USER_PASS`
+
+    default HTTP Authentication for ALL the downloads in "`user:password`" format. Warning: don't use this option
+    if not all of the downloads need the authentication to avoid leaking credential, use the `--netrc-file` option instead
+
+`--netrc-file NETRC_FILE`
+
+    a .netrc-like file for HTTP authentication, from which the 'default' entry, if present, takes precedence
+    over the `--user-pass` option
+
 `-h, --help`
 
     show help message and exit
 
 #### Examples
 
     bdownload https://www.afilelink.com/afile.tar.gz
```

### Comparing `bdownload-0.1.8/setup.py` & `bdownload-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `bdownload-0.1.8/src/bdownload/cli.py` & `bdownload-0.1.9/src/bdownload/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,25 +11,28 @@
 from argparse import ArgumentParser, ArgumentTypeError
 from os.path import join, abspath, isfile
 import re
 from codecs import encode, decode
 import logging
 from functools import partial
 import signal
+import netrc
 
 from requests.cookies import cookielib
 
-from .download import BDownloader, COOKIE_STR_REGEX, BDownloaderException
+from .download import BDownloader, BDownloaderException, COOKIE_STR_REGEX, HTTP_HEADER_REGEX
 
 
-DEFAULT_MAX_WORKER = 20         # number of worker threads
-DEFAULT_MIN_SPLIT_SIZE = "1M"   # file split size in bytes[1M = 1024*1024]
-DEFAULT_CHUNK_SIZE = "100K"     # every request range size in bytes[1K = 1024]
-DEFAULT_NUM_POOLS = 20          # number of connection pools
-DEFAULT_POOL_SIZE = 20          # max number of connections in the pool
+DEFAULT_MAX_PARALLEL_DOWNLOADS = 5  # number of files downloading concurrently
+DEFAULT_WORKERS_PER_DOWNLOAD = 4    # number of worker threads for every file downloading job
+DEFAULT_MAX_WORKER = DEFAULT_MAX_PARALLEL_DOWNLOADS * DEFAULT_WORKERS_PER_DOWNLOAD  # number of worker threads
+DEFAULT_MIN_SPLIT_SIZE = "1M"       # file split size in bytes[1M = 1024*1024]
+DEFAULT_CHUNK_SIZE = "100K"         # every request range size in bytes[1K = 1024]
+DEFAULT_NUM_POOLS = 20              # number of connection pools
+DEFAULT_POOL_SIZE = 20              # max number of connections in the pool
 
 
 def _win32_utf8_argv():
     """Use ``kernel32.GetCommandLineW`` and ``shell32.CommandLineToArgvW`` to get ``sys.argv`` as a list of UTF-8 strings.
 
     Versions 2.5 and older of Python don't support Unicode ("mon€y röcks" for example) in ``sys.argv`` on Windows, with
     the underlying Windows API instead replacing multi-byte characters with '?'.
@@ -182,14 +185,32 @@
         if not COOKIE_STR_REGEX.match(cookies):
             msg = 'Cookie {!r} is not in valid format!'.format(cookies)
             raise ArgumentTypeError(msg)
 
         return cookies
 
 
+def _validate_http_header(header):
+    """Validate and normalize the HTTP request header."""
+    header = header.strip()
+    if not HTTP_HEADER_REGEX.match(header):
+        msg = 'HTTP header {!r} is not in valid format!'.format(header)
+        raise ArgumentTypeError(msg)
+
+    return header
+
+
+def _validate_netrc_file(file):
+    try:
+        netrc_auth = {machine: (login, password) for machine, (login, _, password) in netrc.netrc(file).hosts.items()}
+        return netrc_auth
+    except netrc.NetrcParseError as e:
+        raise ArgumentTypeError(str(e))
+
+
 def _arg_parser():
     parser = ArgumentParser()
 
     omeg = parser.add_mutually_exclusive_group()
     omeg.add_argument('-O', '--OUTPUT', dest='output', type=lambda f: [f],
                       help='a save-as file name (optionally with absolute or relative (to `-D DIR`) path), '
                            'e.g. `-O afile.tar.gz https://www.afilelink.com/afile.tar.gz`')
@@ -215,14 +236,20 @@
 
     parser.add_argument('-p', '--proxy', dest='proxy', default=None,
                         help='proxy either in the form of "http://[user:pass@]host:port" or "socks5://[user:pass@]host:port"')
 
     parser.add_argument('-n', '--max-workers', dest='max_workers', default=DEFAULT_MAX_WORKER, type=int,
                         help='number of worker threads [default: {}]'.format(DEFAULT_MAX_WORKER))
 
+    parser.add_argument('-j', '--max-parallel-downloads', dest='max_parallel_downloads', default=DEFAULT_MAX_PARALLEL_DOWNLOADS, type=int,
+                        help='number of files downloading concurrently [default: {}]'.format(DEFAULT_MAX_PARALLEL_DOWNLOADS))
+
+    parser.add_argument('-J', '--workers-per-download', dest='workers_per_download', default=DEFAULT_WORKERS_PER_DOWNLOAD, type=int,
+                        help='number of worker threads for every file downloading job [default: {}]'.format(DEFAULT_WORKERS_PER_DOWNLOAD))
+
     parser.add_argument('-k', '--min-split-size', dest='min_split_size', default=DEFAULT_MIN_SPLIT_SIZE, type=_normalize_bytes_num,
                         help='file split size in bytes, "1048576, 1024K or 2M" for example [default: {}]'.format(DEFAULT_MIN_SPLIT_SIZE))
 
     parser.add_argument('-s', '--chunk-size', dest='chunk_size', default=DEFAULT_CHUNK_SIZE, type=_normalize_bytes_num,
                         help='every request range size in bytes, "10240, 10K or 1M" for example [default: {}]'.format(DEFAULT_CHUNK_SIZE))
 
     parser.add_argument('-e', '--cookie', dest='cookie', default=None, type=_load_cookies,
@@ -268,14 +295,26 @@
 
     cmeg = parser.add_mutually_exclusive_group()
     cmeg.add_argument('-c', '--continue', dest='continuation', action='store_const', const=True,
                       help='resume from the partially downloaded files. This is the default behavior')
     cmeg.add_argument('--no-continue', dest='no_continue', action='store_const', const=True,
                       help='do not resume from last interruption, i.e. start the download from beginning')
 
+    parser.add_argument('-H', '--header', dest='header', action='append', type=_validate_http_header,
+                        help='extra HTTP header, standard or custom, which can be repeated several times, '
+                             'e.g. \'-H "User-Agent: John Doe" -H "X-BD-Key: One Thousand And One Nights"\'. '
+                             'The headers take precedence over the ones specified by other parameters if conflict happens.')
+    parser.add_argument('-u', '--user-pass', dest='user_pass',
+                        help='default HTTP Authentication for ALL the downloads in \'user:password\' format. '
+                             'Warning: don\'t use this option if not all of the downloads need the authentication '
+                             'to avoid leaking credential, use the \'--netrc-file\' option instead')
+    parser.add_argument('--netrc-file', dest='netrc_file', type=_validate_netrc_file,
+                        help='a .netrc-like file for HTTP authentication, from which the \'default\' entry, if present, '
+                             'takes precedence over the \'--user-pass\' option')
+
     return parser
 
 
 def _interrupt_handler(bdownloader, signum, frame):
     """The handler for the signals ``SIGINT`` and ``SIGQUIT``.
 
     Args:
@@ -348,29 +387,40 @@
     logging.basicConfig(level=log_level)
 
     continuation = True if args.continuation else False if args.no_continue else True
 
     check_certificate = True if args.check_certificate.lower() == 'true' else False
     client_certificate = (args.certificate, args.private_key) if args.certificate and args.private_key else args.certificate
 
+    headers = None if not args.header else \
+        {name.strip(): value.strip() for name, _, value in [header.partition(':') for header in args.header]}
+
+    default_auth = None
+    if args.user_pass:
+        user, _, passwd = args.user_pass.partition(":")
+        default_auth = (user, passwd)
+    if args.netrc_file and args.netrc_file.get('default'):
+        default_auth = args.netrc_file['default']
+
     urls = args.url if args.url else args.urls
     files = ['']*len(urls) if args.output is None else args.output+['']*(len(urls)-len(args.output))
     if len(files) > len(urls):
         print('The specified OUTPUTs and URLs don\'t align, extra OUTPUTs will be ignored: {!r}'.format(args.output[len(urls):]))
 
     path_files = [abspath(join(args.dir, f)) for f in files]
     path_urls = list(zip(path_files, urls))
 
     ignore_termination_signals()
     try:
-        with BDownloader(max_workers=args.max_workers, min_split_size=args.min_split_size, chunk_size=args.chunk_size,
-                         proxy=args.proxy, cookies=args.cookie, user_agent=args.user_agent, progress=args.progress,
-                         num_pools=args.num_pools, pool_maxsize=args.pool_size, continuation=continuation,
-                         referrer=args.referrer, check_certificate=check_certificate,
-                         ca_certificate=args.ca_certificate, certificate=client_certificate) as downloader:
+        with BDownloader(max_workers=args.max_workers, max_parallel_downloads=args.max_parallel_downloads,
+                         workers_per_download=args.workers_per_download, min_split_size=args.min_split_size,
+                         chunk_size=args.chunk_size, proxy=args.proxy, cookies=args.cookie, user_agent=args.user_agent,
+                         progress=args.progress, num_pools=args.num_pools, pool_maxsize=args.pool_size, continuation=continuation,
+                         referrer=args.referrer, check_certificate=check_certificate, ca_certificate=args.ca_certificate,
+                         certificate=client_certificate, auth=default_auth, netrc=args.netrc_file, headers=headers) as downloader:
             install_signal_handlers(downloader)
             downloader.downloads(path_urls)
             succeeded, failed = downloader.wait_for_all()
     except BDownloaderException as e:
         print(str(e))
         succeeded, failed = downloader.results()
```

### Comparing `bdownload-0.1.8/src/bdownload/download.py` & `bdownload-0.1.9/src/bdownload/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
 from distutils.dir_util import mkpath, remove_tree
 from distutils.errors import DistutilsFileError
 import requests
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 from requests import Session
+from requests.auth import AuthBase, HTTPBasicAuth, HTTPDigestAuth, extract_cookies_to_jar
 from requests.cookies import cookielib, RequestsCookieJar
 from clint.textui import progress as clint_progress
 
 
 here = os.path.dirname(os.path.abspath(__file__))
 with open(os.path.join(here, 'VERSION'), mode='r') as fd:
     __version__ = fd.read().strip()
@@ -70,20 +71,29 @@
 
 #: float: Default retry backoff factor.
 RETRY_BACKOFF_FACTOR = 0.1
 
 #: set: Default status codes to retry on intended for the underlying ``urllib3``.
 URLLIB3_RETRY_STATUS_CODES = frozenset([413, 429, 500, 502, 503, 504])
 
-COOKIE_STR_REGEX = re.compile(r'\s*(?:[^,; =]+=[^,; ]+\s*(?:$|\s+|;\s*))+\s*')
-"""A compiled regular expression object used to match the cookie string in the form of key/value pairs.
+#: set: Default status codes that should be avoided retrying on before handled
+RETRY_EXEMPT_STATUS_CODES = frozenset([401, 407])
+
+COOKIE_STR_REGEX = re.compile(r'^\s*(?:[^,; =]+=[^,; ]+\s*(?:$|\s+|;\s*))+\s*$')
+"""regex: A compiled regular expression object used to match the cookie string in the form of key/value pairs.
 
 See also :meth:`BDownloader.__init__()` for more details about `cookies`.
 """
 
+HTTP_HEADER_REGEX = re.compile(r'^\s*[a-zA-Z0-9_-]+:\s*[a-zA-Z0-9_ :;.,\\/"\'?!(){}[\]@<>=\-+*#$&`|~^%]*$')
+"""regex: A compiled regular expression object used to validate the HTTP request header in the ``'name: value'`` format.
+
+Refer to https://developers.cloudflare.com/rules/transform/request-header-modification/reference/header-format.
+"""
+
 _requests_extended_retries_factor = REQUESTS_EXTENDED_RETRIES_FACTOR
 """int: Number of retries that complements and extends the builtin `Retry` mechanism of ``urllib3``.
 
 This global variable is meant for the decorator :func:`retry_requests()`, and its value can be modified through the 
 module level function :func:`set_requests_retries_factor`. It is initialized to :const:`REQUESTS_EXTENDED_RETRIES_FACTOR`
 by default, and usually you don't want to change it.
 
@@ -124,22 +134,23 @@
     """
     global _requests_extended_retries_factor
 
     if retries > 0:
         _requests_extended_retries_factor = retries
 
 
-def retry_requests(exceptions, backoff_factor=0.1, logger=None):
+def retry_requests(exceptions, status_exemptlist=RETRY_EXEMPT_STATUS_CODES, backoff_factor=0.1, logger=None):
     """A decorator that retries calling the wrapped ``requests``' function using an exponential backoff on exception.
 
     The retry attempt will be activated in the event of `exceptions` being caught and for all the bad status codes (i.e.
-    codes ranging from 400 to 600).
+    codes ranging from 400 to 600) except the ones in `status_exemptlist`.
 
     Args:
         exceptions (:obj:`Exception` or :obj:`tuple` of :obj:`Exception`\ s): The exceptions to check against.
+        status_exemptlist (set of int): A set of HTTP status codes that the retry should be avoided.
         backoff_factor (float): The backoff factor to apply between retries.
         logger (logging.Logger): An event logger.
 
     Returns:
         The wrapper function.
 
     Raises:
@@ -169,15 +180,16 @@
             # e.g. by setting it to ``0`` directly. This behavior is intentionally not disabled.
             global _requests_extended_retries_factor
 
             ntries = 0
             while True:
                 try:
                     r = f(*args, **kwargs)  # `r` is an instance of the ``requests.Response`` object
-                    r.raise_for_status()
+                    if not (status_exemptlist and r.status_code in status_exemptlist):
+                        r.raise_for_status()
                     return r
                 except exceptions as e:
                     ntries += 1
                     if ntries > _requests_extended_retries_factor:
                         raise e
                     steps = random.randrange(0, 2**ntries)
                     backoff = steps * backoff_factor
@@ -202,15 +214,15 @@
         Retry of ``urllib3`` is enabled. Nevertheless, they together determine the number of the total retries.
         See :func:`requests_retry_session` for more information about their cooperation.
     """
     #: Default timeouts: the connect timeout value defaults to 3.05 seconds, and the read timeout 6 seconds.
     TIMEOUT = (3.05, 6)
 
     def __init__(self, timeout=None, proxy=None, cookies=None, user_agent=None, referrer=None, verify=True, cert=None,
-                 requester_cb=None):
+                 headers=None, auth=None, requester_cb=None):
         """Initialize the ``Session`` instance.
 
         The HTTP header ``User-Agent`` of the session is set to a default value of `bdownload/VERSION`, if not provided,
         with `VERSION` being replaced by the package's version number.
 
         Args:
             timeout (float or 2-tuple of float): Timeout value(s) as a float or ``(connect, read)`` tuple for both the
@@ -218,14 +230,16 @@
                 whole or any item thereof, it will take a default value from :attr:`TIMEOUT`, accordingly.
             proxy (str): Same as for :meth:`BDownloader.__init__()`.
             cookies (str, dict or CookieJar): Same as for :meth:`BDownloader.__init__()`.
             user_agent (str): Same as for :meth:`BDownloader.__init__()`.
             referrer (str): Same as for :meth:`BDownloader.__init__()`.
             verify (bool or str): Same as for :meth:`requests.request()`.
             cert (str or tuple): Same as for :meth:`requests.request()`.
+            headers (dict): Same meaning as in :meth:`BDownloader.__init__()`.
+            auth (tuple or :class:`requests.auth.AuthBase`): Same meaning as in :meth:`BDownloader.__init__()`.
             requester_cb (func): The callback function provided by the downloader that uses the instantiated
                 session object as the HTTP(S) requester. It will get called when making an HTTP GET request.
         """
         super(RequestsSessionWrapper, self).__init__()
 
         timeout = timeout or self.TIMEOUT
         if isinstance(timeout, tuple):
@@ -239,28 +253,32 @@
         else:  # float
             if timeout < 0:
                 timeout = self.TIMEOUT
 
         self.timeout = timeout
         self.requester_cb = requester_cb
 
+        if isinstance(headers, dict):
+            self.headers.update(headers)
+
         self.referrer = referrer.strip() if referrer is not None else referrer
         if self.referrer:
-            self.headers.update({'Referer': self.referrer})
+            self.headers['Referer'] = self.referrer
 
         default_user_agent = 'bdownload/{}'.format(__version__)
         self.user_agent = user_agent if user_agent and user_agent.strip() else default_user_agent
-        self.headers.update({'User-Agent': self.user_agent})
+        self.headers['User-Agent'] = self.user_agent
 
         if proxy is not None:
             self.proxies = dict(http=proxy, https=proxy)
         if cookies is not None:
             self.cookies = cookies if isinstance(cookies, (dict, cookielib.CookieJar)) else self._build_cookiejar_from_kvp(cookies)
         self.verify = verify
         self.cert = cert
+        self.auth = auth
 
     @retry_requests(requests.RequestException, backoff_factor=RETRY_BACKOFF_FACTOR)
     def get(self, url, **kwargs):
         """Wrapper around ``requests.Session``'s `get` method decorated with the :func:`retry_requests` decorator.
 
         Args:
             url: URL for the file to download from.
@@ -553,14 +571,51 @@
             self.width = mill_bar_len
 
             self.STREAM.write(mill_bar)
             self.STREAM.write('\n')
             self.STREAM.flush()
 
 
+class HTTPBasicAuthEx(HTTPBasicAuth):
+    """Attaches HTTP Basic Authentication to the given Request object.
+
+    This class is adapted from ``requests.auth.HTTPBasicAuth`` and ``requests.auth.HTTPDigestAuth``, with added support
+    for handling `Unauthorized` request on the response.
+
+    References:
+         https://github.com/psf/requests/blob/main/src/requests/auth.py
+    """
+    def __init__(self, username, password):
+        super(HTTPBasicAuthEx, self).__init__(username, password)
+
+    def handle_401(self, r, **kwargs):
+        """Takes the given response and tries basic-auth, if needed."""
+        if not 400 <= r.status_code < 500:
+            return r
+
+        s_auth = r.headers.get('www-authenticate', '')
+        if 'basic' in s_auth.lower():
+            # Consume content and release the original connection
+            # to allow our new request to reuse the same one.
+            r.content
+            r.close()
+            prep = r.request.copy()
+            extract_cookies_to_jar(prep._cookies, r.request, r.raw)
+            prep.prepare_cookies(prep._cookies)
+
+            prep = self.__call__(prep)
+            _r = r.connection.send(prep, **kwargs)
+            _r.history.append(r)
+            _r.request = prep
+
+            return _r
+
+        return r
+
+
 class BDownloader(object):
     """The class for executing and managing download jobs.
 
     The context of the current downloading job is structured as::
 
         ctx = {
             "total_size": 2000,  # total size of all the to-be-downloaded files, maybe inaccurate due to chunked transfer encoding
@@ -583,17 +638,17 @@
                                      # and updated on completion (SUCCEEDED, FAILED, CANCELLED) of every task (`Future`)
                     "resumable": True,
                     "resuming_from_intr": False,  # Are we resuming from keyboard interruption?
                     "download_state": "inprocess",
                     "cancelled_on_exception": False,
                     "orig_path_url": ('file1', 'url1\turl2\turl3'),  # (path, url) as a subparameter passed to :meth:`downloads`
                     "path_url": ('full_path_to_file1', 'url1\turl2\turl3'),  # (full_pathname, active_URLs)
-                    "urls":{"url1":{"accept_ranges": "bytes", "refcnt": 1, "interrupted": 2, "succeeded": -5},
-                            "url2":{"accept_ranges": "none", "refcnt": 0, "interrupted": 0, "succeeded": 0},
-                            "url3":{"accept_ranges": "bytes", "refcnt": 1, "interrupted": 0, "succeeded": -2}},
+                    "urls":{"url1":{"auth": None, "auth_header": {"Authorization": "Basic dXNlcjpwYXNz"}, "accept_ranges": "bytes", "refcnt": 1, "interrupted": 2, "succeeded": -5},
+                            "url2":{"auth": None, "auth_header": {"Authorization": "Digest username='user',realm=..."}, "accept_ranges": "none", "refcnt": 0, "interrupted": 0, "succeeded": 0},
+                            "url3":{"auth": None, "auth_header": {}, "accept_ranges": "bytes", "refcnt": 1, "interrupted": 0, "succeeded": -2}},
                     "alt_ranges": [("bytes=1000-1999", `ctx_range2_obj`)],  # task ranges stack
                     "worker_ranges": [("bytes=0-999", `ctx_range1_obj`)],  # active range downloading tasks
                     "active_workers": 1,  # number of active worker threads on ranges downloading of the file
                     "ranges_succeeded": 0,  # number of ranges successfully downloaded
                     "ranges":{
                         "bytes=0-999": {
                             "start": 0,  # start byte position
@@ -666,15 +721,15 @@
         self.close()
         return False
 
     def __init__(self, max_workers=None, max_parallel_downloads=5, workers_per_download=4, min_split_size=1024*1024,
                  chunk_size=1024*100, proxy=None, cookies=None, user_agent=None, logger=None, progress='mill',
                  num_pools=20, pool_maxsize=20, request_timeout=None, request_retries=None, status_forcelist=None,
                  resumption_retries=None, continuation=True, referrer=None, check_certificate=True, ca_certificate=None,
-                 certificate=None):
+                 certificate=None, auth=None, netrc=None, headers=None):
         """Create and initialize a :class:`BDownloader` object.
 
         Args:
             max_workers (int): The `max_workers` parameter specifies the number of the parallel downloading threads,
                 whose default value is determined by ``#num_of_processor * 5`` if set to `None`.
             max_parallel_downloads (int): `max_parallel_downloads` limits the number of files downloading concurrently.
                 It has a default value of 5.
@@ -735,14 +790,27 @@
                 certificate or not. It defaults to `True`.
             ca_certificate (str): The `ca_certificate` parameter specifies a path to the preferred CA bundle file (.pem)
                 or directory with certificates in PEM format of trusted CAs. If set to a path to a directory, the directory
                 must have been processed using the ``c_rehash`` utility supplied with OpenSSL, according to ``requests``.
                 NB the cert files in the directory each only contain one CA certificate.
             certificate (str or tuple): `certificate` specifies a client certificate. It has the same meaning as that of
                 `cert` in :meth:`requests.request()`.
+            auth (tuple or :class:`requests.auth.AuthBase`): The `auth` parameter sets a (user, pass) tuple or Auth handler
+                to enable Basic/Digest/Custom HTTP Authentication. It will be passed down to the underlying :class:`requests.Session`
+                instance as the default authentication.
+
+                Warning:
+                    The `auth` will be applied to all the downloads for HTTP Authentication. Don't use this parameter,
+                    if not all of the downloads need the authentication, to avoid leaking credential. Instead, use
+                    the **netrc** parameter for fine-grained control over HTTP Authentication.
+            netrc (dict): `netrc` specifies a dictionary of ``'machine': (login, password)`` (or ``'machine': requests.auth.AuthBase``)
+                for HTTP Authentication, similar to the .netrc file format in spirit.
+            headers(dict): `headers` specifies extra HTTP headers, standard or custom, for use in all of the requests
+                made by the session. The headers take precedence over the ones specified by other parameters, e.g. **user_agent**,
+                if conflict happens.
 
         Raises:
             ValueError: Raised when the `cookies` is of the :obj:`str` type and not in valid format.
         """
         if not resumption_retries or resumption_retries < 0:
             # Fall back on the defaults if None, 0 or a negative number is given
             resumption_retries = REQUESTS_RETRIES_ON_STREAM_EXCEPTION
@@ -750,16 +818,20 @@
 
         if not request_retries or request_retries < 0:
             # Fall back on the defaults if None, 0 or a negative number is given
             request_retries = URLLIB3_BUILTIN_RETRIES_ON_EXCEPTION
 
         verify = ca_certificate if check_certificate and ca_certificate else check_certificate
 
+        self.auth = auth
+        self.netrc = netrc
+
         session = RequestsSessionWrapper(timeout=request_timeout, proxy=proxy, cookies=cookies, user_agent=user_agent,
-                                         referrer=referrer, verify=verify, cert=certificate, requester_cb=self.raise_on_interrupted)
+                                         referrer=referrer, verify=verify, cert=certificate, headers=headers, auth=None,
+                                         requester_cb=self.raise_on_interrupted)
         self.requester = requests_retry_session(session=session, builtin_retries=request_retries,
                                                 backoff_factor=RETRY_BACKOFF_FACTOR,
                                                 status_forcelist=status_forcelist,
                                                 num_pools=num_pools, pool_maxsize=pool_maxsize)
 
         self.max_parallel_downloads = max_parallel_downloads
         self.workers_per_download = workers_per_download
@@ -921,17 +993,18 @@
                     ranges = self.calc_req_ranges(range_end - range_start + 1, self.chunk_size, range_start)
 
                     fd.seek(range_start)
 
                     for start, end in ranges:
                         req_range_new = "bytes={}-{}".format(start, end)
                         headers = {"Range": req_range_new}
+                        headers.update(ctx_file['urls'][url]['auth_header'])
 
                         try:
-                            r = self.requester.get(url, headers=headers, allow_redirects=True, stream=True)
+                            r = self.requester.get(url, headers=headers, allow_redirects=True, stream=True, auth=ctx_file['urls'][url]['auth'])
                             if r.status_code == requests.codes.partial:
                                 try:
                                     for chunk in r.iter_content(chunk_size=self._STREAM_CHUNK_SIZE):
                                         fd.write(chunk)
                                         ctx_range['offset'] += len(chunk)
 
                                         self.raise_on_interrupted()
@@ -1029,19 +1102,20 @@
                         req_range_new = "bytes={}-{}".format(range_start, '')
                         headers = {"Range": req_range_new}
                         status_code = requests.codes.partial
                     else:
                         range_start = ctx_range['start']
                         headers = {}
                         status_code = requests.codes.ok
+                    headers.update(ctx_file['urls'][url]['auth_header'])
 
                     fd.seek(range_start)
 
                     try:
-                        r = self.requester.get(url, headers=headers, allow_redirects=True, stream=True)
+                        r = self.requester.get(url, headers=headers, allow_redirects=True, stream=True, auth=ctx_file['urls'][url]['auth'])
                         if r.status_code == status_code:
                             try:
                                 for chunk in r.iter_content(chunk_size=self._STREAM_CHUNK_SIZE):
                                     fd.write(chunk)
                                     ctx_range['offset'] += len(chunk)
 
                                     if headers:
@@ -1319,30 +1393,58 @@
                     'resuming_from_intr': False, 'download_state': self.PENDING, 'cancelled_on_exception': False,
                     'orig_path_url': orig_path_url, 'path_url': None, 'urls': {}, 'ranges': {}, 'alt_ranges': [],
                     'worker_ranges': [], 'active_workers': 0, 'ranges_succeeded': 0}
 
         active_urls = []
         downloadable = False  # Must have at least one active URL to download the file
         for mirror_url in orig_urls:
+            # determine the URL-specific authentication
+            auth = None
+            parsed = urlparse(mirror_url)
+            if parsed.username and parsed.password:
+                auth = (parsed.username, parsed.password)
+            elif self.netrc:
+                auth = self.netrc.get(parsed.netloc)
+                if not auth and parsed.port:
+                    auth = self.netrc.get(parsed.hostname)
+            if not auth:
+                auth = self.auth
+
+            auth_up = None if isinstance(auth, AuthBase) else auth  # ('user', 'passwd')
+            auth_wx = auth if isinstance(auth, AuthBase) else None
+
             try:
-                with self.requester.get(mirror_url, allow_redirects=True, stream=True) as r:
+                with self.requester.get(mirror_url, allow_redirects=True, stream=True, auth=auth_wx) as r:
+                    if r.status_code == requests.codes.unauthorized and auth_up:
+                        r_auth = r.headers.get('www-authenticate', '').lower()
+                        if "digest" in r_auth:
+                            auth_wx = HTTPDigestAuth(*auth_up)
+                            auth_wx.init_per_thread_state()
+                            auth_wx._thread_local.num_401_calls = 0
+                            r = auth_wx.handle_401(r)
+                        elif "basic" in r_auth:
+                            auth_wx = HTTPBasicAuthEx(*auth_up)
+                            r = auth_wx.handle_401(r)
+
                     if r.status_code == requests.codes.ok:
                         file_len = int(r.headers.get('Content-Length', 0))
                         if file_len:
                             if not ctx_file['length']:
                                 ctx_file['length'] = file_len
                             else:
                                 if file_len != ctx_file['length']:
                                     self._logger.error("Error: the size of the file '%s' obtained from '%s' happened to "
                                                        "mismatch with that from others, download will continue but the "
                                                        "downloaded file may not be the intended one", file_name, mirror_url)
 
                                     continue
 
-                        ctx_url = ctx_file['urls'][mirror_url] = {'accept_ranges': "none", 'refcnt': 0, 'interrupted': 0,
+                        auth_header = {'Authorization': r.request.headers['Authorization']} if r.request.headers.get('Authorization') else {}
+                        ctx_url = ctx_file['urls'][mirror_url] = {'auth': auth_wx, 'auth_header': auth_header,
+                                                                  'accept_ranges': "none", 'refcnt': 0, 'interrupted': 0,
                                                                   'succeeded': 0}
 
                         accept_ranges = r.headers.get('Accept-Ranges')
                         if "bytes" == accept_ranges:
                             ctx_url['accept_ranges'] = accept_ranges
                             ctx_file['resumable'] = True
```

### Comparing `bdownload-0.1.8/src/bdownload/utils.py` & `bdownload-0.1.9/src/bdownload/utils.py`

 * *Files identical despite different names*

### Comparing `bdownload-0.1.8/tests/test_bdownloader.py` & `bdownload-0.1.9/tests/test_bdownloader.py`

 * *Files identical despite different names*

### Comparing `bdownload-0.1.8/tests/test_cli.py` & `bdownload-0.1.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bdownload-0.1.8/tests/test_multisource_download.py` & `bdownload-0.1.9/tests/test_multisource_download.py`

 * *Files identical despite different names*

### Comparing `bdownload-0.1.8/third_parties/setupext_janitor/janitor.py` & `bdownload-0.1.9/third_parties/setupext_janitor/janitor.py`

 * *Files identical despite different names*

### Comparing `bdownload-0.1.8/third_parties/setupext_janitor/README.rst` & `bdownload-0.1.9/third_parties/setupext_janitor/README.rst`

 * *Files identical despite different names*

