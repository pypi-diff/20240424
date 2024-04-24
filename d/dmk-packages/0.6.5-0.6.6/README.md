# Comparing `tmp/dmk_packages-0.6.5.tar.gz` & `tmp/dmk_packages-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmk_packages-0.6.5.tar", last modified: Tue Apr 23 05:17:44 2024, max compression
+gzip compressed data, was "dmk_packages-0.6.6.tar", last modified: Wed Apr 24 08:56:46 2024, max compression
```

## Comparing `dmk_packages-0.6.5.tar` & `dmk_packages-0.6.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-23 05:17:44.569694 dmk_packages-0.6.5/
--rw-r--r--   0 tommie     (501) staff       (20)    11347 2024-04-04 04:45:57.000000 dmk_packages-0.6.5/LICENSE
--rw-r--r--   0 tommie     (501) staff       (20)     1854 2024-04-23 05:17:44.569427 dmk_packages-0.6.5/PKG-INFO
--rw-r--r--   0 tommie     (501) staff       (20)     1365 2024-04-04 04:45:57.000000 dmk_packages-0.6.5/README.md
--rw-r--r--   0 tommie     (501) staff       (20)      584 2024-04-23 05:15:23.000000 dmk_packages-0.6.5/pyproject.toml
--rw-r--r--   0 tommie     (501) staff       (20)       38 2024-04-23 05:17:44.569752 dmk_packages-0.6.5/setup.cfg
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-23 05:17:44.563577 dmk_packages-0.6.5/src/
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-23 05:17:44.564953 dmk_packages-0.6.5/src/dmk_packages/
--rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.5/src/dmk_packages/__init__.py
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-23 05:17:44.568125 dmk_packages-0.6.5/src/dmk_packages/crawler/
--rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.5/src/dmk_packages/crawler/__init__.py
--rw-r--r--   0 tommie     (501) staff       (20)     3534 2024-04-23 05:13:00.000000 dmk_packages-0.6.5/src/dmk_packages/crawler/bigkinds.py
--rw-r--r--   0 tommie     (501) staff       (20)     6578 2024-04-23 05:13:33.000000 dmk_packages-0.6.5/src/dmk_packages/crawler/clien.py
--rw-r--r--   0 tommie     (501) staff       (20)     6600 2024-04-23 05:13:33.000000 dmk_packages-0.6.5/src/dmk_packages/crawler/fnguide.py
--rw-r--r--   0 tommie     (501) staff       (20)     2321 2024-04-04 04:45:57.000000 dmk_packages-0.6.5/src/dmk_packages/crawler/naver_blog.py
--rw-r--r--   0 tommie     (501) staff       (20)    15349 2024-04-04 04:45:57.000000 dmk_packages-0.6.5/src/dmk_packages/crawler/naver_search_volume.py
--rw-r--r--   0 tommie     (501) staff       (20)     1382 2024-04-23 05:13:33.000000 dmk_packages-0.6.5/src/dmk_packages/crawler/pdf_to_text.py
--rw-r--r--   0 tommie     (501) staff       (20)    13362 2024-04-23 05:01:14.000000 dmk_packages-0.6.5/src/dmk_packages/crawler/youtube.py
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-23 05:17:44.568713 dmk_packages-0.6.5/src/dmk_packages/database/
--rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.5/src/dmk_packages/database/__init__.py
--rw-r--r--   0 tommie     (501) staff       (20)     3057 2024-04-04 04:45:57.000000 dmk_packages-0.6.5/src/dmk_packages/database/database.py
--rw-r--r--   0 tommie     (501) staff       (20)     1895 2024-04-04 04:45:57.000000 dmk_packages-0.6.5/src/dmk_packages/naver_datalab.py
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-23 05:17:44.569117 dmk_packages-0.6.5/src/dmk_packages.egg-info/
--rw-r--r--   0 tommie     (501) staff       (20)     1854 2024-04-23 05:17:44.000000 dmk_packages-0.6.5/src/dmk_packages.egg-info/PKG-INFO
--rw-r--r--   0 tommie     (501) staff       (20)      677 2024-04-23 05:17:44.000000 dmk_packages-0.6.5/src/dmk_packages.egg-info/SOURCES.txt
--rw-r--r--   0 tommie     (501) staff       (20)        1 2024-04-23 05:17:44.000000 dmk_packages-0.6.5/src/dmk_packages.egg-info/dependency_links.txt
--rw-r--r--   0 tommie     (501) staff       (20)       41 2024-04-23 05:17:44.000000 dmk_packages-0.6.5/src/dmk_packages.egg-info/requires.txt
--rw-r--r--   0 tommie     (501) staff       (20)       13 2024-04-23 05:17:44.000000 dmk_packages-0.6.5/src/dmk_packages.egg-info/top_level.txt
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-24 08:56:46.002235 dmk_packages-0.6.6/
+-rw-r--r--   0 tommie     (501) staff       (20)    11347 2024-04-04 04:45:57.000000 dmk_packages-0.6.6/LICENSE
+-rw-r--r--   0 tommie     (501) staff       (20)     1854 2024-04-24 08:56:46.002006 dmk_packages-0.6.6/PKG-INFO
+-rw-r--r--   0 tommie     (501) staff       (20)     1365 2024-04-04 04:45:57.000000 dmk_packages-0.6.6/README.md
+-rw-r--r--   0 tommie     (501) staff       (20)      584 2024-04-24 08:53:14.000000 dmk_packages-0.6.6/pyproject.toml
+-rw-r--r--   0 tommie     (501) staff       (20)       38 2024-04-24 08:56:46.002282 dmk_packages-0.6.6/setup.cfg
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-24 08:56:45.996546 dmk_packages-0.6.6/src/
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-24 08:56:45.997665 dmk_packages-0.6.6/src/dmk_packages/
+-rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.6/src/dmk_packages/__init__.py
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-24 08:56:46.000952 dmk_packages-0.6.6/src/dmk_packages/crawler/
+-rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.6/src/dmk_packages/crawler/__init__.py
+-rw-r--r--   0 tommie     (501) staff       (20)     3534 2024-04-24 08:52:39.000000 dmk_packages-0.6.6/src/dmk_packages/crawler/bigkinds.py
+-rw-r--r--   0 tommie     (501) staff       (20)     6580 2024-04-24 08:53:08.000000 dmk_packages-0.6.6/src/dmk_packages/crawler/clien.py
+-rw-r--r--   0 tommie     (501) staff       (20)     6600 2024-04-24 08:52:39.000000 dmk_packages-0.6.6/src/dmk_packages/crawler/fnguide.py
+-rw-r--r--   0 tommie     (501) staff       (20)     2321 2024-04-04 04:45:57.000000 dmk_packages-0.6.6/src/dmk_packages/crawler/naver_blog.py
+-rw-r--r--   0 tommie     (501) staff       (20)    15349 2024-04-04 04:45:57.000000 dmk_packages-0.6.6/src/dmk_packages/crawler/naver_search_volume.py
+-rw-r--r--   0 tommie     (501) staff       (20)     1382 2024-04-24 08:52:39.000000 dmk_packages-0.6.6/src/dmk_packages/crawler/pdf_to_text.py
+-rw-r--r--   0 tommie     (501) staff       (20)    13362 2024-04-23 05:01:14.000000 dmk_packages-0.6.6/src/dmk_packages/crawler/youtube.py
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-24 08:56:46.001451 dmk_packages-0.6.6/src/dmk_packages/database/
+-rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.6/src/dmk_packages/database/__init__.py
+-rw-r--r--   0 tommie     (501) staff       (20)     3057 2024-04-04 04:45:57.000000 dmk_packages-0.6.6/src/dmk_packages/database/database.py
+-rw-r--r--   0 tommie     (501) staff       (20)     1895 2024-04-04 04:45:57.000000 dmk_packages-0.6.6/src/dmk_packages/naver_datalab.py
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-24 08:56:46.001745 dmk_packages-0.6.6/src/dmk_packages.egg-info/
+-rw-r--r--   0 tommie     (501) staff       (20)     1854 2024-04-24 08:56:45.000000 dmk_packages-0.6.6/src/dmk_packages.egg-info/PKG-INFO
+-rw-r--r--   0 tommie     (501) staff       (20)      677 2024-04-24 08:56:45.000000 dmk_packages-0.6.6/src/dmk_packages.egg-info/SOURCES.txt
+-rw-r--r--   0 tommie     (501) staff       (20)        1 2024-04-24 08:56:45.000000 dmk_packages-0.6.6/src/dmk_packages.egg-info/dependency_links.txt
+-rw-r--r--   0 tommie     (501) staff       (20)       41 2024-04-24 08:56:45.000000 dmk_packages-0.6.6/src/dmk_packages.egg-info/requires.txt
+-rw-r--r--   0 tommie     (501) staff       (20)       13 2024-04-24 08:56:45.000000 dmk_packages-0.6.6/src/dmk_packages.egg-info/top_level.txt
```

### Comparing `dmk_packages-0.6.5/LICENSE` & `dmk_packages-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.5/PKG-INFO` & `dmk_packages-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmk_packages
-Version: 0.6.5
+Version: 0.6.6
 Summary: Common packages for DataMKTKorea
 Author-email: DataMarketingKorea <infra@datamarketing.co.kr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dmk_packages-0.6.5/README.md` & `dmk_packages-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.5/pyproject.toml` & `dmk_packages-0.6.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmk_packages"
-version = "0.6.5"
+version = "0.6.6"
 authors = [{ name = "DataMarketingKorea", email = "infra@datamarketing.co.kr" }]
 description = "Common packages for DataMKTKorea"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = ["SQLAlchemy", "python-dotenv", "psycopg2-binary"]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `dmk_packages-0.6.5/src/dmk_packages/crawler/bigkinds.py` & `dmk_packages-0.6.6/src/dmk_packages/crawler/bigkinds.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.5/src/dmk_packages/crawler/clien.py` & `dmk_packages-0.6.6/src/dmk_packages/crawler/clien.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         """
         items = soup.select(".list_item.symph_row.jirum")
         results = []
 
         for item in items:
             board_sn = int(item["data-board-sn"])
             _regist_date = pendulum.parse(item.select_one(".timestamp").text)
-            regist_date = _regist_date.add(hours=9)
+            regist_date = _regist_date.add(hours=18)
 
             title = item.select_one(".subject_fixed").text
             if "헤드라인 모음" in title:
                 continue
 
             if self._min_board_sn <= board_sn <= self._max_board_sn:
                 continue
@@ -122,15 +122,15 @@
         pages = soup.select(".board-nav-page")
         if len(pages) <= 1:
             return None
         next_btn_exists = bool(soup.select_one(".board-nav-next"))
 
         last_item = soup.select(".list_item.symph_row.jirum")[-1]
         last_item_timestamp = pendulum.parse(last_item.select_one(".timestamp").text)
-        last_item_timestamp = last_item_timestamp.add(hours=9)
+        last_item_timestamp = last_item_timestamp.add(hours=18)
 
         if self._date_from > last_item_timestamp:
             return None
 
         for idx, page in enumerate(pages):
             if "active" in page.get("class", []):
                 if next_btn_exists or idx + 1 < len(pages):
```

### Comparing `dmk_packages-0.6.5/src/dmk_packages/crawler/fnguide.py` & `dmk_packages-0.6.6/src/dmk_packages/crawler/fnguide.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.5/src/dmk_packages/crawler/naver_blog.py` & `dmk_packages-0.6.6/src/dmk_packages/crawler/naver_blog.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.5/src/dmk_packages/crawler/naver_search_volume.py` & `dmk_packages-0.6.6/src/dmk_packages/crawler/naver_search_volume.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.5/src/dmk_packages/crawler/pdf_to_text.py` & `dmk_packages-0.6.6/src/dmk_packages/crawler/pdf_to_text.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.5/src/dmk_packages/crawler/youtube.py` & `dmk_packages-0.6.6/src/dmk_packages/crawler/youtube.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.5/src/dmk_packages/database/database.py` & `dmk_packages-0.6.6/src/dmk_packages/database/database.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.5/src/dmk_packages/naver_datalab.py` & `dmk_packages-0.6.6/src/dmk_packages/naver_datalab.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.5/src/dmk_packages.egg-info/PKG-INFO` & `dmk_packages-0.6.6/src/dmk_packages.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmk_packages
-Version: 0.6.5
+Version: 0.6.6
 Summary: Common packages for DataMKTKorea
 Author-email: DataMarketingKorea <infra@datamarketing.co.kr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dmk_packages-0.6.5/src/dmk_packages.egg-info/SOURCES.txt` & `dmk_packages-0.6.6/src/dmk_packages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

